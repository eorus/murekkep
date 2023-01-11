---
title: Nexus 7’yi Android 4.1.2’ye Manuel Olarak Yükseltmek
author: bkazar
type: post
date: 2012-10-10T17:38:51+00:00
url: /nexus-7yi-android-4-1-2ye-manuel-olarak-yukseltme/
featured_image: /wp-content/uploads/2012/10/nexus-7-android-412-100x100.jpg
dsq_thread_id:
  - 948749265
categories:
  - Mobil
tags:
  - android

---
Android 4.1.2 güncellemesi Nexus 7 tabletleri yavaş yavaş sollamaya başladı. Eğer tabletinize güncelleme hala gelmediyse umutsuzluğa kapılmayın. Bu yazımızda birkaç dakikada tabletinizin yazılımını nasıl güncelleyeceğinizi anlattık. Fakat baştan belirtmeliyiz ki bu nispeten bilgili kullanıcıların yapabileceği türden bir işlem ve eğer güvenmiyorsanız bu işe hiç kalkışmamanızı tavsiye ederiz.

Anlatacağımız işlem kesinlikle hiçbir değişiklik yapılmamış Nexus 7 tabletleri içindir ve kısacık da olsa birkaç komut yazılarak yapılmakta. Yapacağımız hiçbir değişiklik -güncellemenin kendisi dışında- kalıcı değildir.

**Dikkat: Bu işlem teknik olarak yeterli bilgiye sahip kullanıcıları hedeflemektedir. Riski göze alarak bu işlemleri yapmanız tavsiye edilir.**

<a href="https://www.murekkep.org/nexus-7yi-android-4-1-2ye-manuel-olarak-yukseltme-8510/nexus-7-android-412" rel="attachment wp-att-8512"><img class="alignnone size-full wp-image-8512" title="nexus-7-android-412" src="https://www.murekkep.org/wp-content/uploads/2012/10/nexus-7-android-412.jpg" alt="nexus-7-android-412" width="680" height="383" srcset="https://www.murekkep.org/wp-content/uploads/2012/10/nexus-7-android-412.jpg 680w, https://www.murekkep.org/wp-content/uploads/2012/10/nexus-7-android-412-400x225.jpg 400w, https://www.murekkep.org/wp-content/uploads/2012/10/nexus-7-android-412-50x28.jpg 50w, https://www.murekkep.org/wp-content/uploads/2012/10/nexus-7-android-412-221x125.jpg 221w" sizes="(max-width: 680px) 100vw, 680px" /></a>

**Gerekli Dosyalar**

  * Tamamen stok halde hiçbir değişiklik yapılmamış, Android 4.1.1 yüklü, build JRO03D bir Nexus 7. (Ayarlar > Cihaz Hakkında kısmından kontrol edebilirsiniz. Farklı bir build numarasına sahipseniz farklı bir işlem yapmanız gerekebilir)
  * ADB yükleme dosyalarını içeren zip dosyası. (Windows, Mac ve Linux için)
  * [Google’dan Android 4.1.2 yükseltme paketi.][1]{.broken_link} (31MB)

**İşlem**

  1. ADB yüklenebilir dosyaları içeren zip dosyasını bilgisayarınızda bir klasöre çıkartın
  2. Google üzerinden indirdiğiniz update.zip dosyasını aynı klasöre kopyalayın fakat zip dosyasını açmayın.
  3. Nexus 7 üzerinden Ayarlar > Geliştirme ayarları kısmına gelin ve seçeneği açık (on) konumuna getirin. Ardından USB sorun gidermeyi açın. (USB Debugging. Debugging menüsü altında)
  4. Nexus 7’yi kapatın
  5. Ses açma + Ses kısma + güç düğmelerine aynı anda basarak Bootloader’ı çalıştırın.
  6. Menü yüklendikten sonra Nexus 7’nizi bilgisayarınıza bağlayın.
  7. “Kurtarma Modu/ Recovery Mode” seçmek için ses tuşlarını kullanın ve seçimi yapmak için güç düğmesine basın.
  8. Kırmızı bir ünlem işaretiyle Android logosu ekranda göründüğünde sırayla güç düğmesi, ses kısma ve ses açma düğmesine basın. Bu sırayı takip ederek bastığınız tuşların hiçbirini bırakmayın, işlem sonunda hepsine basılı olacak. Yalnızca sıralamaya dikkat etmelisiniz. Menü açıldığında düğmeleri bırakabilirsiniz.
  9.  Menü üzerinden “apply update from ADB” seçeneğine gelmek için ses düğmelerini kullanın ve seçmek için güç düğmesine basın.
 10. Bilgisayarınızdan “komut istemi” yani DOS açın.
 11. Komut satırını kullanarak ADB yüklenebilir dosyalarını ve güncelleme dosyasını Nexus 7’mize yönlendireceğiz.
 12. Windows için:  
    _adb.exe sideload 03a4eaf95f73.signed-nakasi-JZO54K-from-JRO03D.03a4eaf9.zip_  
    Mac için:  
    _./adb-mac sideload 03a4eaf95f73.signed-nakasi-JZO54K-from-JRO03D.03a4eaf9.zip_  
    Linux için:  
    _./adb sideload 03a4eaf95f73.signed-nakasi-JZO54K-from-JRO03D.03a4eaf9.zip_  
    yazıyoruz.
 13. Güncellemenin yüklenmeye başlaması lazım. Bittiği aman “reboot system now” seçeneğini seçin.
 14. Nexus 7’niz artık Android 4.1.2 ile çalışıyor, tadını çıkarın.

 [1]: https://android.clients.google.com/packages/ota/google_nakasi/03a4eaf95f73.signed-nakasi-JZO54K-from-JRO03D.03a4eaf9.zip "android 4.1.2 yükleme"