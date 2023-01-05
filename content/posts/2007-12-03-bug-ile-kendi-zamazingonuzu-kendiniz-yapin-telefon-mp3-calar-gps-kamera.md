---
title: BUG ile kendi zamazingonuzu kendiniz yapın(telefon,mp3-çalar,gps,kamera)
author: Fatih
type: post
date: 2007-12-03T14:33:28+00:00
url: /bug-ile-kendi-zamazingonuzu-kendiniz-yapin-telefon-mp3-calar-gps-kamera/
dsq_thread_id:
  - 954290972
categories:
  - Teknoloji
tags:
  - açık kaynak
  - linux
  - telefon
  - yazılım

---
Evet başlığı doğru okudunuz. Aslında saydıklarım çok basit şeyler. Çok daha gelişmiş, aklınızı iyi çalıştırırsanız harika aletler yapılabilecek bir ortam var karşınıza. Openmoko hakkında bir şeyler karalamıştım zamanımda. Bu trend önümüzdeki yıllar da devam edeceği çok aşikar. Bugün Turker&#8217;in paylaştığı yazılara göz gezdirirken, Buglabs&#8217;ın çıkartığı BUG adındaki alete gözüm takıldı. Bu nedir peki ? 

Bug iki kısımdan oluşuyor. Birincisi **Bugbase** diğerleri de **Bugmodules** yani bileşenleri. Cüzdan şeklinde kare dikdörtgen bir alet düşünün. 

<center>
</center>

Bu alet tamamen açık kaynak. Yani donanım&#8217;a ait tüm spesifikasyonlar,api&#8217;ler, devreler belli. Onun dışında güzel olan yani ise içinde barındırdığı yazılım da açık-kaynak. Bu da tabiki Linux. Bugbase diye adlandırılan alet aslında bilgisayar gibi bir şey. **128 mb Ram, Cpu, dahili wifi, doldurulabilen pilleri, usb,ethernet girişleri, hafıza kartı girişi** vs&#8230;(sitesinde ayrıntılı şekilde spesifikasyonları var.) Bu girişler dışında üst kısmında da 4 tane ana giriş var. İşte bu boşluklara da bizim Bugmoduls adındaki bileşenler yerleştiriliyor. Nedir bu **Bugmodules** denen şeyler:

<center>
</center>

Şu an itibariyle 4 seçiti var. **GPS, Dokunmatik-renkli ekran, Dijitalkamera/video ve Hareket Sensoru.** Bu moduler de aletin yarısı büyüklüğünde. Örneğin tam 4 tane ekran alıp Bugbase&#8217;in üzerine yerleştirebilirsiniz. Ya da sadece bir tane Gps ve Dijitalkamera olabilir. Böyle şeyler nedense beni çok heyecanladırıyor. İşin güzelliği ise bunun uygulanabilirliğinde. Kısaca aklıma gelen ilk fikirler:

  * Sadece Gps modülü ve Kamera olacak. Bunu da arabanın önüne, yani mangalın arka kısmına yerleştirilecek. Araba çalındığında gps ile yerini belirtecek, fotoğraf çekecek ve içindeki hafıza&#8217;ya kayıt edecek. Ardından ilk bulduğu wifi bağlantısında internet ile bağlanacak ve GPS ile Fotoğraf bilgileri ile birlikte sizlere bildirecek. 
  * Kamera ve Hareket sensörü takılı olacak. Bunu da mağaza&#8217;nın içine koyacaksınız. Olur da hırsız girerse, fotoğrafı çekecek. Yine istenilince içindeki wifi bağlantısı ile iletişim kurularak bu resimle elde edilebilecek. 
  * Gps modülü ve dokunatik-ekran takılı olacak. Koşu yaparken ne kadar hızla ne kadar süre koştuğunuzu Gps vasıtasıyla verileri alabiliyorsunuz, bu verileri güzel bir şekilde izlemeyi ve değerlendirmeyi de dokunmatik ekran ile yapılıyor. 

İleride farklı bileşenler de çıkması bekleniyor, **örneğin ses çıkış giriş modülü, 2 kat daha büyük olan ekran bileşeni, küçük q-klavye**,&#8230;  
[  
Robert Scoble][1]&#8216;nin çektiği bir video var, izlerseniz çok daha iyi anlayacaksınız ne demek istediğimi(video&#8217;da ne gibi alanlarda kullanabileceği hakkında yorumlar da var)

<center>
  <embed style="width:400px; height:326px;" id="VideoPlayback" type="application/x-shockwave-flash" src="http://video.google.com/googleplayer.swf?docId=-1932063822649530376&#038;hl=en" flashvars="" />
  
  <br />
</center>

Yani düşünün bir, tamamen **açık kaynak**, hem donanımı hem de yazılımı, tamamen gelişimlere açık, istediğiniz gibi ortamlar yaratabiliyorsunuz, lego taşları gibi yapıştırıp değişik işler yapmanızı sağlayabilir. Benim aklıma gelmeyen binlerce fikir vardır kesinlikle. Çünkü donanımı da az da olsa siz **tasarlayabiliyorsunuz**. Örneğin sitelerinde de şu örneği vermişler:

> For example, with BUG, you can easily assemble and program a GPS + digital camera device that automatically publishes geo-tagged photos as a web service. Integrating with an online photo-sharing service like Flickr is only a few more lines of code away, and now you have your own real-time, connected traffic-enabled mobile Webcam!

Gördüğünüz gibi akla gelmeyecek işler yapmamız mümkün. Bunu bir de güzel bir pazarlama ve iyi bir fiyat&#8217;a satabilirlerse gelecekte özellikle gençlerin gözdesi olabilir. Örneğin bunlardan bir tane bizim ellimizde olsa, ne yapardınız ? Fikirlerinizi bekliyorum.

 [1]: http://scobleizer.com/