---
title: Linux Üzerinde Flash Plugin 9
author: Alper
type: post
date: 2006-10-23T05:44:19+00:00
url: /linux-uzerinde-flash-plugin-9/
dsq_thread_id:
  - 197135924
categories:
  - Masaüstü
tags:
  - açık kaynak
  - bilişim
  - linux

---
Bilindiği üzere [Adobe][1]{.broken_link}, Flash Player 9 [duyurusunu][2]{.broken_link} yaptı. Her ne kadar beta sürüm olsa da gayet düzgün çalıştığını söyleyebilirim. Linux dağıtımları için flashplugin paketleri oluşmamış olsa dahi birkaç kısa adımda yeni flash sürümünü nasıl çalıştırabileceğinizi anlatacağım. Yapılacak işlemler oldukça basit. Kısaca kurulu olan (dağıtımınızın paket yöneticisi ile yüklediğiniz) flashplugini kaldırıyorsunuz. Yerine indirdiğiniz flash player 9 dosyasını /plugins altına atıyorsunuz.

  * Kurulu olan Flashplugini, dağıtımınızın paket yöneticisi ile kaldırıyorsunuz.
  * [Buradan][3]{.broken_link} Download Installer for Linux (GZ, 2.48 MB) olan dosyayı indiriyorsunuz ve arşivi herhangi bir dizine açıyorsunuz.
  * Mozilla pluginlerinin kurulduğu dizini örnek olarak /opt/mozilla/lib/plugins/ olduğunu varsayıyoruz. Bu dağıtıma göre değişebilir. Genelde /usr/lib/firefox/plugins şeklindedir.
  * İndirdiğiniz ve açtığınız arşivdeki **libflashplayer.so** dosyasını plugins dizini (örn./opt/mozilla/lib/plugins/) altına atıyoruz.
  * Açık olan firefox varsa kapatıyoruz ve tekrar açıyoruz. Adres kısmına about:plugins yazıyoruz. Burada Shokwave Flash olarak gözüken kısımda yazan sürüm numarasının 9.0.xxx şeklinde gözüktüğüne kanaat getiriyoruz.

Hepsi bu kadar. Test etmek için Macromedia Flash Player 8 ve üzeri isteyen bir siteye gidin. Örnek: https://www.cnbce.com/

 [1]: https://www.adobe.com/
 [2]: https://labs.adobe.com/technologies/flashplayer9/
 [3]: https://labs.adobe.com/downloads/flashplayer9.html