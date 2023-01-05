---
title: WordPress 2.7 Yazar Yorumlarını Stillemek
author: Alper
type: post
date: 2008-12-22T07:56:26+00:00
url: /wordpress-27-yazar-yorumlarini-stillemek/
categories:
  - Teknoloji
tags:
  - wordpress

---
WordPress 2.7 yükseltmesinden sonra comments.php dosyasındaki değişkiliklere göz atmaya devam ediyoruz. Ana değişiklikler açısından [WordPress 2.7 Tema için Değişiklikler, Yorumların Düzenlenmesi][1] başlığı altında yeni yorum düzeninden ve değişikliklerin nasıl olduğundan bahsetmiştik. Şimdi ise blog üzerinde **yazıyı yazan (author)** kişinin yorumda bulunması durumunda yazar yorumlarının farklı şekilde gösterilmesi için neler yapılması gerektiğini anlatacağız.  
<!--more-->

  
Wordpress 2.7 Yorum Düzeni değişiminde yeni fonksiyon olan ve birçok görevi üstlenen wp\_list\_comments() &#8216;den ve altyapının ne şekilde değiştiğinden bahsetmiştik. Aslında burada gene wp\_list\_comments() fonksiyonundan kaynaklanan bir durum var. Eğer yazının yazarı tarafından yorum yapılmışsa wordpress otomatik olarak &#8220;**bypostauthor**&#8221; sınıfını **&#8220;li&#8221;** etiketi etrafına yerleştiriyor. Böyle olunca temanız için daha önce kullandığınız css stili geçersiz duruma geliyor. Muhtemelen **li.author** olan css sınıfı **li.bypostauthor** olarak değişiyor. 

Mürekkep üzerinde örnek olarak denediğim stil aşağıdaki gibi kırmızı çerçeveyle belirtilmiş yazar yorumları şeklindedir. Bunu bir örnek olarak düşünürsek, ilgili sınıfı kullanarak istediğiniz stili uygulayabilirsiniz. 

[code=&#8217;css&#8217;]  
ol.commentlist li.bypostauthor { border: 3px solid #CC0033; }  
[/code]

Aynı zamanda wordpress, 2.7 ile kayıtlı kullanıcıların yorumlarınıda ayrıca stilleyebilmenizi sağlıyor. Bunun içinde **li.byuser** sınıfını kullanabilirsiniz. 

[code=&#8217;css&#8217;]  
ol.commentlist li.byuser { Buraya Css geliyor. }  
[/code]

 [1]: https://www.murekkep.org/wordpress-27-tema-icin-degisiklikler-yorumlarin-duzenlenmesi-608