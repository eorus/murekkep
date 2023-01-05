---
title: Ubuntu 8.04 Hardy Heron Alpha 4’deki yenilikler
author: Fatih
type: post
date: 2008-02-02T15:21:47+00:00
url: /ubuntu-804-hardy-heron-alpha-4deki-yenilikler/
categories:
  - Masaüstü
tags:
  - açık kaynak
  - linux
  - ubuntu

---
Bugün **[Ubuntu 8.04][1]**&#8216;ün yeni alpha sürümü [**çıktı**][2]. Henüz stabil olmayan bu sürümde bir çok yenilik dikkatimi çekti. Eğer herhangi bir sorununuz yoksa ve bazı şeyleri göze alıyorsanız kurmanızda fayda var, onun dışında kararlı bir sürüm olmadığını belirtmekte fayda var. Çünkü Ubuntu&#8217;nun alpha sürümleri her ne kadar beraberinde yenilikler getirse de bazen çok kararsız olabiliyorlar. Nihai sürüm Nisan ayında çıkacaktır. Gelelim **Ubuntu 8.04 Hardy Heron Alpha 4**&#8216;deki yeniliklere:

  * Bu sürümde **Xorg**&#8216;ün son sürümü olan **7.3** numaralı sürüm de dahil. Yeni Xorg otomatik olarak sizin tüm çevre birimlerini ayarlıyor ve hiç bir şey yapmanıza gerek kalmıyor. Bu son sürümde çevre birimlerini çok daha iyi tanıyabiliyor(Örneğin otomatik olarak Laptop ekran kartlarını ayarlayıp gerekli çözünürlüğe getirmek gibi)
  * **Alpha 4**&#8216;de Linux çekirdeğin son sürümü olan **2.6.24-rc8** de dahil. Yeni çekirdek demek yeni yenilikler ve daha kararlı bir sistem demektir. Ayrıca Amd64 işlemcilerinde **dynticks** sayesinde tıpkı diğer bilgisayarlardaki gibi güç tüketimi konusunda iyileştirmeler vardır. 
  * Ayrıca [Ubuntu 8.04 Alpha 4][2]&#8216;de **PulseAudio** öntanımlı olarak etkinleştirilmiş bir şekilde geliyor. Peki PulseAudio nedir ? **PulseAudio** bir **ses sunucusu**. Bu ses sunucusu basitce ses uygulamaları için proxy işlemini görüyor. Bu da size daha gelişmiş ayarlar imkanı sunuyor. Örneğin bir başka makineden başka bir makine&#8217;ye ses aktarımı, sample format&#8217;ı dilediğince değiştirme ya da **her uygulama için özel bir ses seviyesi** belirlemek gibi. PulseAudio&#8217;nun özelliklerinden biri de **Linux,Solaris,FreeBSD,Windows,**.. gibi bir çok işletim sisteminde çalışmasıdır. 
  * Alpha 4&#8217;deki başka bir yenilik ise **PolicyKit**&#8216;dir. Nedir efendim bu PolicyKit peki ? PolicyKit size kısaca bazı uygulamaları daha değişik yetkilerle kullanımına izin veriyor. Bildiğimiz **Sudo** uygulaması gibi. Fakat bundaki önemli fark ise kullanıcıyıa sudo&#8217;daki gibi tüm root yetkilerini vermek yerine sadece bir kısım haklar vermektir. **Sudo&#8217;da kullanıcı tamamen root hakları ile herşeyi yapabiliyordu, fakat PolicyKit ile bunu yapamayacak**_(Biz nasıl ayarlaydıysak artık)_. Daha güvenli olmuş oluyor bir nevi.
  * **Ubuntu 8.04 Alpha 4**&#8216;de yeni uygulamalar da boy göstermiyor değil. Bunlardan en önemlisi **Firefox 3 Beta 2**&#8216;dir. Bu Firefox sürümü bize çok daha iyi bir arayüz getiriyor. GTK&#8217; kütüphanelerini de kullandığı için diğer GTK uygulamalarına benziyor. Artık sanki başka bir işletim sisteminin programıymış gibi bize yabancı gelmeyecektir. Nasıl göründüğünü merak ediyorsanız **Fox and Penguin** adlı yazıya bakmanızı tavsiye ederim Onun dışında tipik Firefox yenilikleri de geliyor ki, o da apayrı bir konu. 
  * Torrent için artık adam akıllı bir uygulama da gelmiş bulunmakta bu son sürümde. Eski, işlevsiz ve çirkin arayüzlü Gnome BitTorrent(kusura bakmayın ama cidden öyleydi) yerine bir çok işletim sisteminde çalışan, minimalist bir program olan [**Transmission**][3] geliyor. 
  * Yeni uygulamalar arasında **Vinagre VNC** istemcisi de öntanımlı olarak geliyor. Daha önceki xvnc4viewer uygulamasının yerine kullanılacaktır. Vinagre VNC sayesinde bir den çok sanal makineyi aynı bilgisayar&#8217;da kullanabileceksinz, başka VNC sunucularını Avahi sayesinde bulabileceksiniz ve sık takip ediğiniz bu bağlantıları takip edebileceksiniz.(_En üsteki resim aslında Vinagre ile çalıştırılan bir Ubuntu 8.04 resmidir._)
  * Bitmedi, **Brasero** da bundan sonra Nautilus&#8217;a ilaveten yeni bir cd/dvd yazma programı olacaktır. Mono ile yazılan bu uygulama daha önceki **Serpentine** uygulamasının yerini alacaktır.Bunların dışında **GVFS**, **GnomeVFS**&#8216;in yerini almıştır. **Gnome System Monitor** uygulamasında da iyileştirmeler mevcut. Ayrıca **ufw** adında konsol&#8217;dan çalıştırılabilen bir Firefwall da mevcut bu yeni sürümde. 

Gördüğünüz gibi bir sürü yeni özellik yeni sürümde gelmiş bulunmakta. İlgilenenler Ubuntu sunucularından son sürümü indirebilirler.

 [1]: https://www.murekkep.org/ubuntu-804-hardy-heron-429
 [2]: http://www.ubuntu.com/testing/hardy/alpha4
 [3]: http://www.transmissionbt.com/