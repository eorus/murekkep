---
title: HTC HD2 Windows Mobile 6.5 Yerine Android Yükleme
author: bkazar
type: post
date: 2013-01-15T16:02:44+00:00
url: /htc-hd2-windows-mobile-6-5-yerine-android-yukleme/
featured_image: /wp-content/uploads/2013/01/htc-hd2-100x100.jpg
dsq_thread_id:
  - 1027225683
categories:
  - Mobil
tags:
  - android
  - htc

---
Her yeni işletim sistemi gibi **Windows Mobile 6.5** de ilk çıktığında yer yerinden oynamıştı. Zaten gerçekten de başarılı bir işletim sistemiydi kendi dönemine göre. Akıllı telefonların piyasaya yeni çıktığı zamanlardı. Windows Mobile 6.5 kullanan en başarılı telefonlardan biri _HTC HD2_ modeliydi. Şimdi donanımsal olarak çok güçlü bir telefon olmasa da HTC HD2 kullanmaya devam etmek için geçerli bir sebep Android yüklenebilmesi. Evet hem de en beğenilen sürümlerinden olan Android 4 Ice Cream Sandwich. Günümüzde hala bu telefonu kullanan ve daha güncel bir hale getirmek isteyenleriniz varsa işte size mükemmel bir yazı.

### Windows Mobile 6.5 yerine Android Ice Cream Sandwich

Yaptığım araştırmalara, okuduğum bir sürü rehbere göre internette bu telefonu çok seven ve bırakmak istemeyen bir topluluk var. Bunun nedeni de, harika HTC HD2’nin iOS dışında hemen hemen tüm işletim sistemlerini destekliyor olması. Yanlış duymadınız bu “eski” kalmış telefon Linux, Windows Mobile 6.5, Android 2, Android 4 ve Windows 7 çalıştırabiliyor.

HTC HD2 üzerine Android yüklemek için iki seçeneğiniz var **tethered** ve **untethered**. İki versiyonun çalışma açısından tek farkı telefonun açılıp kapanması. Tethered sürümde telefonunuzda iki adet işletim sistemi bulunuyor eski Windows Mobile 6.5 ve yükleyeceğiniz Android. Untethered olanında ise yalnızca yükleyeceğiniz yeni işletim sistemi çalışıyor. Belki diğer akıllı telefon modellerine de bu işlem uygulanabilir, denemek lazım.

<img class="aligncenter size-full wp-image-10937" alt="htc-hd2" src="https://www.murekkep.org/wp-content/uploads/2013/01/htc-hd2.jpg" width="380" height="368" srcset="https://www.murekkep.org/wp-content/uploads/2013/01/htc-hd2.jpg 380w, https://www.murekkep.org/wp-content/uploads/2013/01/htc-hd2-50x48.jpg 50w, https://www.murekkep.org/wp-content/uploads/2013/01/htc-hd2-103x100.jpg 103w, https://www.murekkep.org/wp-content/uploads/2013/01/htc-hd2-206x200.jpg 206w, https://www.murekkep.org/wp-content/uploads/2013/01/htc-hd2-314x305.jpg 314w" sizes="(max-width: 380px) 100vw, 380px" /> 

Daha fazla bilgi vermeden belirteyim, bu bir **yükleme rehberi değildir**. Size sadece bunu nasıl yükleyeceğinize dair bir tekniği anlatıyorum. Ayrıca telefonunuzun ROM bilgileriyle oynayacağınızdan çöp olma ihtimali de var.

Eğer yapacağınız işlemlerden emin değilseniz sizin için de en doğru yöntem her iki işletim sistemini de SD karta yükleme olacaktır. Her iki işletim istemini de bulunduracağınızdan işler ters gittiğinde anında geri dönebilirsiniz.

**ROM Seçimi**

Yapacağınız ilk şey kendinize en uygun ROM seçeneğini bulmak. Birçok forumun hazırladığı değişik ROM yükleme seçenekleri bulunuyor. Fakat bir tavsiye isterseniz CyanogenMod yüklemeniz gerçek Android deneyimini yaşamak için en doğru seçim olur.

**Hazırlık Aşaması**

SD kart ile ikinci bir işletim sistemi yüklemek için öncelikle HTC HD2 telefonunuzu Windows Mobile 6.5 yüklü haliyle çalıştırıp **bootloader** programları yüklemeniz ve çalıştırmanız gerekiyor. Birkaç aşamada anlatacak olursam;

  * Windows Active Sync indirin ve bilgisayarınıza kurun.
  * Download BIOS Hack Tool ([**HSPL: 2.08.HSPL**][1]{.broken_link}) – bu işlemin en riskli aşaması, biraz daha araştırmanızı tavsiye ederim.
  * Buradaki siteden en son sürüm Radio kontrolcüsünü yükleyin. ([**Bu Sayfadan Sürüm Seçin**][2]{.broken_link})
  * Ardından [**boot loader**][3]{.broken_link} uygulamayı yükleyin. Yeni işletim sistemini yüklemeniz için gerekli
  * İstediğiniz Android sürümünü tavsiye olarak CyanogenMod 9 yükleyin ([**NexusHD2-ICS-CM9-SD_v1.4.7z**][4].).
  * Sıkıştırılmış dosyaları SD kartınıza çıkartın
  * Telefonunuzu yeniden başlatın

Yukarıdaki basamaklarla zaten işlem son derece kolay. Belirtmeden geçemeyeceğim bir şey var; hem telefonda hem de bilgisayarda Microsoft Active Sync açık olmadan BIOS hack çalışmıyor. Tüm işlemlerin gerçekleşmesi yaklaşık 15 dakika sürüyor.

**Sonuç**

HTC HD2 telefonlarına Windows Mobile 6.5 yerine Android yükleyen kullanıcıların belirttiği değişik bir durum mevcut. WP 6.5 ile fotoğraf çekerken kamerada yeşil ve bulanık görüntüler oluyorken aynı kamera Android ile takır takır çalışıyor. Telefonun kullanışlılığı, dokunmatik ekran hassasiyeti gerçekten artmış. Gerçekten modern teknolojiyi takip etmek için telefonunuza ROM yüklemeyi düşünebilirsiniz. Alacağınız riskleri unutmayın.

  * Kaynak 1: http://forum.xda-developers.com/
  * **Kaynak 2:** http://forum.xda-developers.com/showthread.php?t=1437463

 [1]: http://forum.xda-developers.com/showthread.php?p=5279234
 [2]: http://forum.xda-developers.com/showthread.php?t=611787
 [3]: http://forum.xda-developers.com/showthread.php?t=893618
 [4]: https://sites.google.com/site/nexushd2android/nexushd2-ics-cm9/v1-4/download-sd