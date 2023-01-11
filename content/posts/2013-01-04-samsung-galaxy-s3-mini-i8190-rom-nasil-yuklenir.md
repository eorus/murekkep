---
title: Samsung Galaxy S3 Mini i8190 Android 4.1.2 Resmi ROM Nasıl Yüklenir?
author: bkazar
type: post
date: 2013-01-04T19:19:33+00:00
url: /samsung-galaxy-s3-mini-i8190-rom-nasil-yuklenir/
featured_image: /wp-content/uploads/2012/10/galaxy_s3_mini_3-100x100.jpg
dsq_thread_id:
  - 1008443083
categories:
  - Mobil
tags:
  - android
  - samsung

---
Samsung Galaxy S3 Mini modeli için (**i8190**) Endonezya’da OTA olarak Android 4.1.2 güncellemesini almaya başladı. Yakında ülkemizdeki S3 Mini kullanıcıları da bu güncellemeyi alacaklardır. Fakat en yenisi ilk sizde olsun istiyorsanız aşağıda anlatacağımız basamakları takip ederek **Samsung Galaxy S3 Mini** akıllı telefonunuza Android 4.1.2 ROM’unu manuel olarak yükleyebilirsiniz. GS3 Mini şu anda Android 4.1 ROM ile çalışıyor, yani yükleyeceğiniz küçük bir güncelleme olacak. Daha önce hiç ROM yükleme işlemi yapmadıysanız mümkün olduğunca çok okuyup bu işe başlamanızı tavsiye ederiz. Ayrıca olası bir aksaklık tamamen sizlerin sorumluluğundadır. Biz yalnızca bilgilendirme amaçlı olarak bu yazıyı hazırladık. Öncelikle belirtmek istediğimiz şey şu, yükleyeceğiniz A**ndroid 4.1.2 resmi ROM** olacağı için herhangi bir **garanti problemi yaşamayacaksınız**. Her neyse Galaxy S3 Mini Android 4.1.2 ROM yükleme işlemine başlamak için **genelde** öncelikle cihazınızı root’lamanız gerekiyor. Bu konu hakkında internette birçok bilgi veren yazı bulabilirsiniz. Fakat biz Samsung tarafından yayınlanan resmi ROM yükleyeceğimizden Galaxy S3 Mini telefonunuzu **root etmeye gerek yok**.

<img class="aligncenter size-large wp-image-8539" alt="galaxy_s3_mini_3" src="https://www.murekkep.org/wp-content/uploads/2012/10/galaxy_s3_mini_3-400x266.jpg" width="400" height="266" srcset="https://www.murekkep.org/wp-content/uploads/2012/10/galaxy_s3_mini_3-400x266.jpg 400w, https://www.murekkep.org/wp-content/uploads/2012/10/galaxy_s3_mini_3-50x33.jpg 50w, https://www.murekkep.org/wp-content/uploads/2012/10/galaxy_s3_mini_3-187x125.jpg 187w, https://www.murekkep.org/wp-content/uploads/2012/10/galaxy_s3_mini_3.jpg 680w" sizes="(max-width: 400px) 100vw, 400px" /> 

### Samsung Galaxy S3 Mini i8190 ROM Yükleme

Bu rehberde yükleyeceğimiz rom resmi Jelly Bean 4.1.2 I8190DXALL3 olacak. İşlemlere başlamadan önce telefonunuzdaki kişisel bilgilerinizi yedeklemenizi tavsiye ederiz. Ayrıca Samsung KIES senkronizasyon yazılımını da yüklemelisiniz. Ardından Galaxy S3 Mini üzerinde **USB Debugging** özelliğini aktive etmelisiniz. Bunun için;

**_Ayarlar>Uygulamalar>Geliştirme Seçenekleri>USB Hata Giderme_** adımlarını izlemeniz yeterli. Ardından akıllı telefonunuza erişebilmek için **_Odin_** adlı programı indirmeniz gerekiyor. Onu da buradan indirebilirsiniz; **_[Odin İndir>][1]{.broken_link}_**

Son olarak her ihtimale karşı bataryanızın %60 ve üstünde dolu olmasına dikkat ederek işe başlayabilirsiniz.

  1. Önce bilgisayarınıza [KIES][2] indirin ve kurun. Gerekli driver’ları size sağlayacaktır.
  2. Güncelleme dosyasını **_buradan_** indirin.
  3. İndirdiğiniz dosyaları bilgisayarınıza çıkartın.
  4. [**Odin**][1]{.broken_link} uygulamasını indirip kurun.
  5. Odin’i bilgisayarınızda açın.
  6. Telefonunuzu kapatıp download modunda açın.
  7. Galaxy S3 Mini Download modu **_Ses Kısma+Home+Güç_** tuşlarına aynı anda basarak açılıyor.
  8. Download modundaki akıllı telefonunuzu **Odin açıkken** bilgisayarınıza USB ile bağlayın.
  9. Telefon ve bilgisayar bağlandığında Odin size bir uyarı verecektir.
 10. Uyarı verse de vermese de Odin üzerindeki **ID:COM** kısmının sarı olup olmadığını kontrol edin.
 11. Eğer sarı olmadıysa driver’ları cihazınızdan yükleyip buraya kadarki adımları tekrarlayın.
 12. Odin üzerinden **_PDA_**kısmını seçin.
 13. Güncelleme dosyasını seçip **start**’a basın.
 14. Odin’de başka değişiklik yapmayın.
 15. Yükleme bittikten sonra Odin uygulamasında **pass** ve ardından **restart** uyarılarını göreceksiniz.
 16. Akıllı telefonunuz kendini yeniden başlattıktan sonra USB bağlantısını kesebilirsiniz.

Olur da kurulum esnasında Odin kilitlenirse programı kapatın, USB kablosunu çıkartıp S3 Mini’yi yeniden başlatın. Bataryayı çıkarıp yeniden takın ve işlemlere ilk basamaktan başlayın. Ayrıca işlem sonunda **Galaxy S3 Mini** sürekli yeniden başlarsa (boot loop) bu kez cihazı **recovery mod**’unda başlatmanız gerekecek. Bunun için **_Home+Ses Açma + Güç_** düğmelerine basılı tutmanız gerekiyor. Açılan menüden **_Wipe data factory reset_** ve **_wipe cache partition_** seçeneklerini seçip, **_+++go back+++_** ve **_reboot system now_** dediğinizde sistemin sorunsuz çalışıyor olması lazım.

ROM yükleme işlemleri ister custom ister resmi olarak üretici tarafından sunuluyor olsun nispeten “tehlikeli” işlemlerdir. Sonuçta cihazınızı yöneten esas dosyaların olduğu kısmı silip yeniden yüklüyorsunuz. Olası bir hatada geri dönüşü olmayan sonuçlarla karşılaşabilirsiniz. Üstelik resmi olmayan ROM yükleme yaptıktan sonra akıllı telefon ya da cihazınız her neyse, garanti kapsamı dışında kalmaktadır. Bu yüzden riskleri göz önünde bulundurarak bu işe girin. Eğer yine de yapacağım deyip yaptıysanız, Android 4.1.2 ROM yüklenmiş Galaxy S3 Mini cihazınızı güle güle kullanın=)

 [1]: https://ul.to/xt4607xx
 [2]: https://www.samsungapps.com/venus/about/onPc.as?COUNTRY_CODE=TUR&_isAppsDep=Y