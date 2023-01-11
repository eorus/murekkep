---
title: Favicon nedir?
author: Alper
type: post
date: 2009-01-10T21:32:14+00:00
url: /favicon-nedir/
dsq_thread_id:
  - 969850904
categories:
  - Teknoloji
tags:
  - internet tarayıcı

---
[Google Favicon][1] yenilendiği haberini duyurduktan sonra faviconu biraz daha ayrıntılı anlatmak gerektiğini düşünüyorum. 

**Favicon** adı üstünde bir ikondur. Internet tarayıcılarında bir web sayfasını açtığınızda adres çubuğunda beliren resimdir. Bu resimler **16&#215;16** boyutunda olup ***.ico** dosya uzantısına sahiptirler. [Mürekkep.Org][2] için adres çubuğundaki &#8220;m&#8221; harfi ya da önceki yazıda bahsettiğimiz gibi **Google Favicon**&#8216;u bunu yansıtmada en güzel örnektir diyebiliriz. 

<!--more-->

  
Web siteniz için favicon yapmak istiyorsanız bu hiçte zor değildir. Elbette kullanmayı bildikten sonra Gimp, Photoshop gibi uygulamalar bu konuda size yardımcı olacaktır. Ama bunun için çok güzel bir site bulunuyor. [Favicon.cc][3] sitesine uğrayıp kolay bir şekilde kendi faviconunuzu oluşturabilirsiniz. 

[][4]

Peki bir favicon oluşturdunuz ve elinizde **favicon.ico** olarak bir dosya mevcut. Tabi belirtmek lazım bu dosyanın formatı **PNG** veya **GIF** şeklinde olabiliyor. Bunu sitenize nasıl yerleştireceksiniz? 

Oluşturduğunuz favicon.ico dosyasını ftp ile kök dizine koyuyorsunuz. (örn: www.murekkep.org/favicon.gif) Sonra sitenin index dosyasına aşağıdaki kodu **head** kısmından sonra ama **/head** kısmından önce gelecek şekilde ekliyorsunuz. 

[sourcecode language=&#8217;html&#8217;] 

<link rel="shortcut icon" href="https://www.murekkep.org/favicon.gif" />
[/sourcecode]
  
Wordpress için ise admin panelinde tema düzenleme kısmına girip header.php dosyasını açıyoruz. /head satırının hemen üstüne aşağıdaki satırı ekliyoruz.  
[sourcecode language=&#8217;php&#8217;] <link rel="shortcut icon" href="<?php bloginfo('template_directory'); ?/>/favicon.ico&#8221; />

  
[/sourcecode]

Hepsi bu kadar. Detaylar için [W3C][5] sayfasına WordPress için Codex&#8217;e bakabilirsiniz.

 [1]: https://www.murekkep.org/google-favicon-yenilendi-774
 [2]: https://www.murekkep.org
 [3]: https://www.favicon.cc/
 [4]: https://www.favicon.cc
 [5]: https://www.w3.org/2005/10/howto-favicon