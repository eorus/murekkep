---
title: Archlinux 0.8 Voodoo Duyuruldu
author: Alper
type: post
date: 2007-04-01T09:49:59+00:00
url: /archlinux-08-voodoo-duyuruldu/
dsq_thread_id:
  - 197136918
categories:
  - Masaüstü
tags:
  - bilişim
  - internet
  - linux

---
Dün indirdim ve kurdum. Kurulumla ilgili bazı değişiklikler var. Ama kullanıcı tarafını pek etkilemiyor. Daha doğrusu kullanıcının yapması gerekenler konusunda **hwdetect** kolaylığını yerleştiriyor. Hwdetect tüm kuruluma girmiş artık. Yani base paketler yüklendikten sonra sistem konfigürasyonu (rc.conf,fstab,mkinitcpio vs..) kısmından önce hwdetect devreye giriyor. Sistem ile ilgili sorular soruyor. Bundan sonra **/etc/rc.conf** kısmına girdiğinizde MODULES=(&#8230;) satırına bir bakıyorsunuz sizin için donanımınızda tespit edilen ama hwdetect tarafından otomatik yüklenmeyecek modülleri eklemiş. Bunun yanısıra /etc/mkinitcpio.conf içerisinde otomatik modül ve hook yönetimini görüyoruz. Kurulumda locale.gen ayarlanabiliyor. Kernel 2.4 ile ilgili herşey tamamen kaldırılmış.

Root şifresi kurulumdan sonra belirlenmiyor artık. Sistem konfigürasyonu ayarlama kısmında Root şifresi belirleme alanı koymuşlar. Oradan belirliyorsunuz. Base install bittikten sonra root şifresiyle açıp gene bildik yolla user ekliyorsunuz. Yeni iso ile kurulum sırasında herhangi bir sorunla karşılaşmadım.

Haber duyurusu : <http://www.archlinux.org/news/305/> 

Lapis forum üzerindeki başlığa buradan bakabilirsiniz. Ayrıca yakın zamanda kurulum ayrıntılarıyla Lapis Wiki üzerindeki Archlinux Belgeleri de güncellenecektir.

**Tahminimce Archlinux&#8217;un 1 Nisan şakası** :)

Archlinux 5 yıl boyunca **Arch** olarak anıldıktan sonra bugün itibariyle ismini **Arklinux** olarak değiştirdi. Bu değişikliğin nedeni olarak, geçen zaman içerisinde, insanların Archlinux ile Arklinux&#8217;u isim benzerliği ve telaffuzundan dolayı karıştırmaları gösteriliyor.

<http://www.archlinux.org/news/307/>