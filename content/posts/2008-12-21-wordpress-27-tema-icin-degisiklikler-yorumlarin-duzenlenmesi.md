---
title: WordPress 2.7 Tema için Değişiklikler, Yorumların Düzenlenmesi
author: Alper
type: post
date: 2008-12-21T13:28:29+00:00
url: /wordpress-27-tema-icin-degisiklikler-yorumlarin-duzenlenmesi/
dsq_thread_id:
  - 948909624
categories:
  - Teknoloji
tags:
  - tema
  - wordpress

---
Yazı dizisinin bu sefer ki durağı WordPress 2.7 üzerinde yorumlar (comments) kısmının düzenlenmesi ve WordPress 2.7&#8217;e uygun hale getirilmesinin anlatımı olacak. WordPress 2.7 bloglama hayatımıza bir sürü görsel ve altyapısal zenginlik getirdi. Biz de bunu [WordPress 2.7 Tema ve Yönetim Paneli Yenilikleri][1] altında incelemeye alıyoruz. Bu zenginliklerin ya da değişikliklerin en yoğun olduğu yer yeni yorum fonksiyonlarının eklenmesiyle comments.php dosyasında yaşanıyor. Katmanlı (threaded) ve sayfalanmış (paged) yorumlar. Blogunuzu WordPress 2.7&#8217;e yükselttikten sonra temanız normal bir şekilde çalışmaya devam edebilir. Ancak WordPress 2.7  ile ilgili gelen yeniliklere sahip olmak istiyorsanız öncelikle temanızı bu yönde değiştirmeniz gerekmektedir. Comments.php dosyasını düzenlemeye başlayalım.  
<!--more-->

  
**Şifre Koruma Denetlemesi**

Daha önceki wordpress sürümlerinde kullanılan bu kod içerisinde çok küçük değişiklikler olmuş. Bu değişiklik ileride olabilecek yükseltmelere uyumlu olması açısından önem taşıyor. Aşağıdaki kodu comments.php dosyasının en üstüne yerleştiriyoruz.

[code=&#8217;php&#8217;]  
< ?php // Do not delete these lines if (!empty($\_SERVER['SCRIPT\_FILENAME']) && 'comments.php' == basename($\_SERVER['SCRIPT\_FILENAME'])) die ('Please do not load this page directly. Thanks!'); if ( post\_password\_required() ) { echo ' 

<p class="nocomments">
  This post is password protected. Enter the password to view comments.&#8217;;<br /> return;<br /> }
</p>

?>  
[/code]

**Yeni Yorum Döngüsü (comment loop)**

WordPress 2.7 ile birlikte hayata geçen yeni bir fonksiyon ile yorum döngüsündeki karmaşada son bulmuş oluyor. wp\_list\_comments() fonksiyonu ve beraberinde getirdiği argümanları ile bu kısmı oldukça kolay bir hale getiriyor. Kanımca ileride tema geliştiricilerin işini epeyce kolaylaştıracak. Önce codexte belirtildiği gibi buradaki kodun eskiden nasıl olduğuna bakalım.Böylelikle aradaki farkı daha iyi gözlemleyebiliriz.

[code=&#8217;php&#8217;]  
if ($comments) :  
< ?php $comment\_count = get\_comment\_count($post->ID); echo $comment\_count[&#8216;approved&#8217;]; ?> Comments

<ul class="commentlist">
  < ?php foreach( $comments as $comment ) : // stuff to display the comment in an LI here endforeach; ?>
</ul>

< ?php else : if ('open' == $post->comment_status) :  
// If comments are open, but there are no comments.  
else :  
// comments are closed  
endif;  
endif;  
[/code]

Şimdi WordPress 2.7 yorum döngüsünde kullanacağımız kodun basit haline göz atalım. Yukarıdaki karmaşadan eser yok. Çok daha anlaşılır. Aşağıdaki kısım Murekkep üzerinde kullandığımız comments.php dosyasından geri izlemeler (trackbacks) kısmı çıkartılarak alınmıştır. Burada tüm yükü  yukarıda bahsettiğimiz gibi wp\_list\_comments() fonksiyonu çekiyor. Siz kendi argümanlarınızı ya da basit halini (avatar ve type=comment vs.. çıkararak) yerleştirerek kullanabilirsiniz. Tüm katmanlı (threaded) yorumlar bu fonksiyon üzerinden üretiliyor.Yeni olarak çok fazla olan yorumlarda &#8220;yorum sayfalama&#8221; diyebileceğimiz navigasyon eklemesi var. Sayfalama için yorum sayı limitini yönetici panelindeki ayarlar &#8211; tartışma kısmından değiştirebiliyorsunuz.

[code=&#8217;php&#8217;]  
< ?php if ( have_comments() ) : ?>

### Yazı Hakkında Yapılmış Yorumlar

**< ?php comments_number('Henüz yorum yapılmamış', 'Bir yorum yapılmış', '% yorum yapılmış' );?> | &#8220;< ?php the_title(); ?>&#8221;**

<div class="navigation">
  <div class="alignleft">
    < ?php previous_comments_link() ?>
  </div>
  
  <div class="alignright">
    < ?php next_comments_link() ?>
  </div></p>
</div>

<ol class="commentlist">
  < ?php wp_list_comments('type=comment&avatar_size=32'); ?>
</ol>

<div class="navigation">
  <div class="alignleft">
    < ?php previous_comments_link() ?>
  </div>
  
  <div class="alignright">
    < ?php next_comments_link() ?>
  </div></p>
</div>

< ?php else : // this is displayed if there are no comments so far ?>

< ?php if ('open' == $post->comment_status) : ?>  
<!-- If comments are open, but there are no comments. -->

< ?php else : // comments are closed ?>  
<!-- If comments are closed. -->

<p class="nocomments">
  Bu yazı için yorumlar kapanmıştır.
</p>

< ?php endif; ?>  
< ?php endif; ?>  
[/code]

**Javascript Yorum Fonksiyonu**

Temanızı WordPress 2.7 ile gelen özelliklere adapte etmeniz ve yukarıda belirttiğimiz katmanlı yorum özelliklerinin gelmesi için javascript fonksiyonunun ilgili yere eklenmesi gerekmektedir. Bunun için header.php dosyasını açıyoruz ve wp_head() satırını buluyoruz. Hemen üstüne aşağıdaki kodu ekliyoruz.

[code=&#8217;php&#8217;]  
< ?php if ( is\_singular() ) wp\_enqueue_script( 'comment-reply' ); ?>  
[/code]

Bu kod ile beraber yorumlarda cevapla linkinin doğru bir şekilde çalışmasını sağlıyoruz. Ama bu tek başına yeterli olmayacağından scriptin doğru çalışması için comments.php dosyası içerisinde yorum formu kısmına aşağıdaki kodu eklememiz gerekiyor. 

[code=&#8217;php&#8217;]  
< ?php comment\_id\_fields(); ?>  
[/code]  
Aşağıda örnek olması açısından yorum formu kodunun bittiği yere yani yorumunuzu gönderin (submit) ifadesinin sonlandığı yerin hemen altına ekliyoruz. 

[code=&#8217;php&#8217;]

<input name="submit" type="submit" id="submit" tabindex="5" value="Yorumu Gönder" />  
< ?php comment\_id\_fields(); ?>  
[/code]

Yukarıda bahsettiğimiz javascriptin doğru çalışması ve cevapla linkinin geçerli olması için tüm yorum metin yazma alanının bir div ile çerçevelenmesi gerekiyor. Böylelikle ihtiyacı olan yerlere doğru bir şekilde bakıp doğru kaynaklara ulaşmasını sağlıyoruz. Bazı eski temalarda ve varsayılanlar dahil bu kısım div etiketi olmadan yer alabiliyordu.  
[code=&#8217;html&#8217;]  
<a id="respond"></a>  
[/code]  
Şimdi bunu artık bir DIV etiketi ile çerçeveliyoruz. Ve &#8220;Yorumunuzu buradan bırakabilirsiniz&#8221; kısmı için aşağıdaki yorum başlığı kodunu kullanıyoruz. 

[code=&#8217;php&#8217;]  
< ?php comment\_form\_title(); ?>  
[/code]

Son olarak aynı DIV çerçevesi içerisinde cevapla linkine tıklandığında bu cevaplamayı iptal etmek için gereken parametreleri ekliyoruz. 

[code=&#8217;php&#8217;]

<div id="cancel-comment-reply">
  <small>< ?php cancel_comment_reply_link() ?></small>
</div>

[/code]

Tüm bunları büyük resimde görmemiz gerekirse aşağıdaki gibi tablo oluşacaktır. 

[code=&#8217;php&#8217;]

<div id="respond">
  <h3 style=margin-bottom:5px;">< ?php comment_form_title( 'Buradan yorumunuzu bırakabilirsiniz', 'Yorumunuzu bırakın %s' ); ?></h3> 
  
  <div id="cancel-comment-reply">
    <small>< ?php cancel_comment_reply_link(); ?></small>
  </div>
  
  <p>
    [/code]
  </p>
  
  <p>
    Dikkat ettiyseniz en baştaki div için etiketi kapatmadık. Bunun kapandığı kısım comments.php içerisinde en altta comment id fileds kısmından sonra form etiketini kapattıktan sonra olacaktır.
  </p>
  
  <p>
    [code=&#8217;php&#8217;]
  </p>
  
  <p>
    <input name="submit" type="submit" id="submit" tabindex="5" value="Yorumu Gönder" /><br /> < ?php comment_id_fields(); ?>
  </p>
  
  <p>
    < ?php do_action('comment_form', $post->ID); ?>
  </p>
  
  <div class="clear">
  </div>
</div>

[/code]

Böyle parça parça hangi elementlerin nerelere geldiğini aktarmaya çalıştım. comments.php dosyası için büyük resme bakabilmeniz ve yorumlayabilmeniz açısından [Murekkep.Org][2] üzerinde kullandığımız **comments.php** dosyasına buradan bakabilirsiniz. En azından yukarıda bahsetmek istediklerimizin tam olarak nereye nasıl entegre olduklanını görmeniz açısından faydalı olacaktır. 

Tüm bu işlemleri yaptıktan sonra esas yapılması gereken ve yapmazsanız katmanlı yorumları aktif etmemiş olacağınız kısmı anlatalım. WordPress yönetim panelinizden aşağıdaki gibi ayarlar &#8211; tartışma kısmından **&#8220;katmanlı yorumlara izin ver&#8221;** çentik koyarak aktif etmeniz gerekmektedir. 

Evet katmanlı (threaded) yorumları ve yorum dosyasını wordpress 2.7 için düzenlemek ilk etapta bu işlemleri gerektiriyor. Geçen hafta içerisinde yaptığımız değişiklikler aşamasında faydalandığımız kaynaklar aşağıdaki gibidir. Yeni katmanlı yorumların css düzenlemesi için özellikle son link olan <a href="https://cdharrison.com/2008/12/threaded-comments/" target="_blank">Stylizing Threaded/Nested Comments in WordPress 2.7</a>&#8216;e bakmanızı öneririz.

  * <a href="https://ottodestruct.com/blog/2008/09/29/wordpress-27-comments-enhancements" target="_blank">WordPress 2.7 Comments Enhancements</a>
  * WordPress 2.7 Comment Threading
  * Migrating Plugins and Themes to 2.7/Enhanced Comment Display
  * <a href="https://cdharrison.com/2008/12/threaded-comments/" target="_blank">Stylizing Threaded/Nested Comments in WordPress 2.7</a>

Umarım anlatımda eksikliklerimiz ya da aktarırken atladığımız unsurlar yoktur. Eğer varsa düzeltmek için görüşlerinizi bekliyoruz. WordPress 2.7&#8217;de yorumlar kısmını temanızda düzenlerken bir sorunla karşılaşmanız durumunda ya da bu yazıya ekleme yapmak isterseniz yorumlarınızı her zaman bekliyoruz.

 [1]: https://www.murekkep.org/wordpress-27-tema-ve-yonetim-paneli-yenilikleri-597
 [2]: https://www.murekkep.org/