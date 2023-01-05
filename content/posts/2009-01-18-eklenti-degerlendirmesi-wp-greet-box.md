---
title: 'Eklenti Değerlendirmesi : WP Greet Box'
author: Alper
type: post
date: 2009-01-18T12:19:27+00:00
url: /eklenti-degerlendirmesi-wp-greet-box/
dsq_thread_id:
  - 955367339
categories:
  - Teknoloji
tags:
  - wordpress

---
[Wp Greet Box][1] **WordPress** eklentisini bugün Weblogtoolscollection üzerindeki değerlendirmesini gördükten sonra [Mürekkep.Org][2] üzerinde kullanmaya başladık. Hem kullanmayanlara bilgi olması hem de bu değerlendirmenin Türkçeleştirilmesini sağlamak amacıyla sizlerle paylaşmak istiyoruz. <!--more-->

Öncelikle **Wp Greet Box** nedir? Bu eklenti özetle websitenize, günlüğünüze gelen ziyaretçilere, geldikleri yönlendiriciye bağlı olarak bir hoşgeldin mesajı gösteriyor. Örneğin eğer bir [Digg][3] kullanıcısı Digg üzerinden sitenize gelmişse buna dair bir mesaj ile karşılaşıyor ve yazıyı Digg&#8217;e eklemesi için bir link oluyor. Veya [Twitter][4] üzerinden gelen bir kullanıcıya ilgili yazıyı twit etmesi ve Twitter&#8217;a aktarmasını sağlayan linki veriyor. Bunun dışında ilk defa sitenizi ziyaret edenlere (herhangi bir yönlendirici olmaksızın direkt siteye girenler) sitenizi takip etmeleri **RSS** beslemesine abone olmaları yönünde bir yazı çıkarıyor. 

Tüm bu yönlendirici bağlantılara göre hedeflenmiş tavsiyeler okuyucuların ilgisini çeken ve sitenize bağlı kalmalarına yardımcı oluyor. **Mürekkep.Org** üzerinde uygulamaya başladığımız WP Greet Box için **Google** üzerinden arama yaparak gelen okuyuculara yönelik çıkan mesaj aşağıdaki gibidir. 

<span style="color: rgb(128, 0, 0);"><strong>WP Greet Box Özellikleri</strong></span>

  * Sitenize yönlendirmeyi sağlayan bağlantılara göre ziyaretçilere farklı hoşgeldin mesajları göstermek. Bu hoşgeldin ya da merhaba mesajlarını her şekilde düzenleyebiliyorsunuz. Mesaj eklemek, düzenlemek veya silmek.
  * Bu karşılama mesajları otomatik olarak yazının üst kısmına yerleşiyor. WordPress tema dosyanızda değişiklik yapmanıza gerek kalmıyor. 
  * Bu karşılama mesajını otomatik olarak yazının üstüne ya da altına koyabiliyor.
  * Karşılama mesajı ziyaretçiler tarafından kapatılabilir özelliğe sahip. 
  * Büyük arama motorlarından ziyaretçilerin aradıkları kelimeleri saptayıp bunları karşılama mesajı altında ilgili yazılar şeklinde gösterebiliyor.
  * Eğer gelen ziyaretçi herhangi bir yönlendirici kriterine tabi değilse o zaman varsayılan bir karşılama mesajı gösteriyor. 
  * Eğer ziyaretçinin JavaScript&#8217;i aktif değilse gene varsayılan bir karşılama mesajı gösteriyor.
  * Ön planda AJAX karşılama mesajı wordpress bellek yönetimi eklentileriyle (WP Super Cache gibi) uyumlu ve aynı zamanda WPMU ile çalışabiliyor.
  * Belli bir zaman aşımı uygulaması ile gelen ziyaretçileri unutabiliyor. Böylelikle devamlı ziyaretçilere karşılama mesajı göstermiyor.
  * Belirli kurallar koyup yönlendirici siteleri bu işin dışında tutabiliyoruz. Böylelikle buralardan gelen ziyaretçilere karşılama mesajı gösterilmiyor. 
  * Karşılama mesajının her alanı için CSS ile düzenlenebilir özelliği. Mesaj kutusunu ve içeriğini hem CSS hem de HTML kullanarak düzenleyebiliyorsunuz.
  * Halihazırda birçok yönlendirici site varsayılan olarak eklenmiş durumda ama bunların dışında listede görmedikleriniz varsa kolayca kendi yönlendirici sitenizi ekleyebiliyorsunuz. 
      * blinklist.com
      * blogmarks.com
      * del.icio.us
      * delicious.com
      * digg.com
      * diigo.com
      * facebook.com
      * flickr.com
      * furl.com
      * google.*
      * ma.gnolia.com
      * mister-wong.com
      * myspace.com
      * netvibes.com
      * newsvine.com
      * reddit.com
      * search.live.com
      * search.msn.com
      * search.yahoo.com
      * simpy.com
      * stumbleupon.com
      * technorati.com
      * twitter.com
      * youtube.com

<span style="color: rgb(128, 0, 0);"><strong>Değerlendirme :</strong></span>

**WP Greet Box** dolu bir şekilde gelen bir eklenti. Hemen herşey düşünülmüş. Kurulumu kolay. **WordPress 2.7** içerisinden eklentilerin yüklenme kısmından kolayca yüklenip aktifleştirilebiliyor. 

İlk aktifleştirdiğinizde tüm yönlendirici siteler varsayılan olarak geliyor. Varsayılanlar dışında tutulanlarda hemen altında gösteriliyor. Açıkçası ben şu anda geldiği gibi kullanıyorum. Hatta wordpress temanızda bile düzenleme yapmak istemezseniz yazınızını üst kısmına çok güzel bir şekilde yerleşiyor. Bu kısmı değiştirmek isterseniz ki ben böyle yaptım. Aşağıda anlattığımız gibi düzeltebilirsiniz. 

Bunun için **single.php** dosyasını düzenlemek üzere açın. Burada başlığın altı olabilir ya da yazının herhangi bir kısmına artık nereye koymak istiyorsanız aşağıdaki kodu eklemeniz yeterli. Tabi eğer böyle yapacaksanız ayarlarından otomatik ekle kısmını inaktif hale getirmeniz gerekiyor. 

[code=&#8217;php&#8217;]  
< ?php if(function\_exists('wp\_greet\_box')){wp\_greet_box();} ?>  
[/code]

İlgili yazıları gösterdiğinden bahsetmiştik. Ben bunu devre dışı bıraktım. Çünkü zaten her yazının altın YARPP eklentisinin otomatik olarak yerleştirdiği ilişkili yazılar kısmını kullanıyorum. 

Özetle eğer böyle bir karşılama mesajı düşünüyorsanız WP Greet Box bu işlevi gayet güzel yerine getiren kriterlere sahip. Kullanımı kolay ve karşılama mesajlarını her şekilde düzenleme imkanı sağlıyor. 

WP Greet Box eklentisini yeni kullanmaya başladık. Siz günlüğünüzde bu eklentiyi kullanıyor musunuz? Kullanmaya başladığınız zamandan itibaren ziyaretçilerinizden gelen tepkiler nasıl? Sitenizin ziyaretçi bağlılığına bir katkıda bulundu mu? Ve son olarak eklentinin sağladıkları dışında olmasını düşündüğünüz yeni özellikler neler olabilir. 

**WordPress Eklenti Dizini** : [Wp Greet Box Eklentisi][5]  
**Weblogtoolscollection Yazısı** : Plugin Review: WP Greet Box

 [1]: http://wordpress.org/extend/plugins/wp-greet-box/other_notes/
 [2]: https://www.murekkep.org
 [3]: http://www.digg.com
 [4]: http://www.twitter.com
 [5]: http://wordpress.org/extend/plugins/wp-greet-box/