---
title: Murekkep.org’da Host ve Tema değişikliği
author: Fatih
type: post
date: 2007-01-29T15:46:11+00:00
url: /murekkeporgda-host-ve-tema-degisikligi/
dsq_thread_id:
  - 197136456
categories:
  - Google
tags:
  - tema
  - wordpress

---
Fark etmişinizdir bir kaç gündür siteyi başka bir yere yönlendirmiştik. Bunun sebebi de Host değişikliği yapmak üzereydik. Ayrıca domain&#8217;i de bir yerden başka bir yere taşıyacağımızdan bunu yapmaya karar verdik. Geçiş sorunsuz bir şekilde gerçekleşti, ayrıca temayı da değiştirmeye karar verdik. <strike>Bundan sonra <a href="https://cavemonkey50.com/code/clean-and-mean/" title="Clean and Mean" target="_blank" class="broken_link">Clean and Mean</a> temasını kullanıyoruz</strike>. Açıkcası K2&#8217;nin bir kaç yerde hatalı olması, ve bize biraz şişik gelmesi bizi bu yöne itti. Ayrıca yeni tema&#8217;da genişlik de artı, bu sayede yazıları artık daha rahat okuyabilirsiniz. Bu aralar düzenlemeler yaptığımız için son hali biraz daha farklı olacaktır.

Bundan sonra Murekkep.org <a href="https://www.dreamhost.com/" target="_blank">Dreamhost</a> kullanıyor. Sorunsuz bir host değişikliği olsun diye, murekkep.org&#8217;u murekkep.arsln.org&#8217;a taşıdık 4-5 günlüğüne. Bu süreç içinde yazılarımız, sizden gelen yorumlarımız da bu veritabanına aktarılacaktı. Bu sayede sitenin devamı da sağlanıyordu. Ayrıca Murekkep.org&#8217;dan murekkep.arsln.org&#8217;a yönlendirme de yaptığımız için, adres çubuğundaki değişiklik haricinde başka bir şey fark etmemiş olmanız gerekiyor. Bu süreç içinde izlediğimiz yollar şu şekildeydi

  1. Murekkep.arsln.org&#8217;da bir veritabanı oluşturup, murekkep.org&#8217;daki veritabanını oraya taşımak. Ayrıca murekkep.org dizinindeki tüm dosyalar da oraya aktarıldı.
  2. Murekkep.org murekkep.arsln.org&#8217;a yönlendirildi
  3. İpowerweb&#8217;den Dreamhost&#8217;a alan adının transferi için . Madem tüm alanı oraya taşıyoruz, domaini de oraya taşıyalım ve sorun çıkmasın istedik. Her şey tek yerden
  4. Transfer gerçekleştikten sonra, ssh ile tüm dosyaları Murekkep.Org&#8217;a taşımak. Arsln.org&#8217;da Dreamhost&#8217;da olduğu için ve ikisi de aynı makinede olduğu için tüm dosyaları shell&#8217;den kopyaladık. Bu 5 sn bile sürmedi.
  5. Murekkep.arsln.org&#8217;daki veritabanını murekkep.org&#8217;a taşımak.

Bu kadar, sizin de gördüğünüz gibi herhangi bir sorun yok şu an. 1 gün sonra murekkep.arsln.org&#8217;daki tüm dosyaları ve veritabanını da sileceğiz. Dreamhost&#8217;a geçmemizin bir çok sebebi var. Sağladı özellikleri çok iyi : **200gb** alan, **2TB** bandwith, **sınırsız domain**, **sınırsız subdomain**, **ssh** desteği, vs &#8230; ayrıca Destek kısımları da çok iyi , <a href="https://discussion.dreamhost.com/" target="_blank" class="broken_link">forum</a>, <a href="https://wiki.dreamhost.com" target="_blank" class="broken_link">wiki</a> gibi yerler bakıp aradığınız şeylere bakabilirsiniz. Forumlarında soru sorabilirsiniz, baktınız olmadı, direkt destek hattına mail attıp sorununuzu izah edebilirsiniz. Yabancı şirket olduğundan, tek eksik yönü ingilizce bilmeniz gerekmektedir.

Hepsi bu kadar. Dreamhostu sizlere de tavsiye ederiz. Ayrıca şunu da ekliyeyim, PR değeri 0 iken birden 4&#8217;e yükseliverdi. Neden böyle olduğunu bilmiyoruz. Site&#8217;de gördüğünüz sorunlar olursa bize <a href="https://www.murekkep.org/iletisim/" target="_blank">bildirirseniz</a> seviniriz. Geçmiş olsun ve hayırlı, nice güzel yazılara &#8230;