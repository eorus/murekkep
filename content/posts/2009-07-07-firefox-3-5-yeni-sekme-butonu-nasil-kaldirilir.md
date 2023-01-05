---
title: Firefox 3.5 Yeni Sekme Butonu Nasıl Kaldırılır?
author: Alper
type: post
date: 2009-07-07T10:13:35+00:00
url: /firefox-3-5-yeni-sekme-butonu-nasil-kaldirilir/
post-thumb:
  - https://www.murekkep.org/mini/foxmini.jpg
dsq_thread_id:
  - 949206781
categories:
  - Masaüstü
tags:
  - firefox
  - internet
  - internet tarayıcı
  - yazılım

---
[Firefox 3.5 resmi olarak duyuruldu][1]{.broken_link}. Firefox 3.5 ile gelen birçok yenilik arasında sık kullandığımız alanlarda görsel değişimleri de gözlemlemekteyiz. Bunların en başında ve hemen dikkatinizi çeken muhtemelen yeni sekme yaratmak için konulan yeni sekme butonu olmuştur. Henüz dikkatinizi çekmediyse firefox 3.5 içerisinde açtığınız sekmelerde en sağdakinin yan tarafında &#8220;+&#8221; şeklinde iliştirilmiş olan küçük ikondan bahsediyorum. 

Firefox her zaman kullanıcı tarafından düzenlenebilir bir internet tarayıcısı olmuştur. Açık kaynak kodlu ve isteğinize en güzel cevap verecek şekilde kolayca düzenlenebilen firefox için bu durumu da isteğimize göre kullanabilir ya da kaldırabiliriz. 

Öncelikle aşağıda örnek resmini verdiğim **firefox 3.5 yeni sekme** butonunu kullanmayı ya da tutmayı düşünüyor musunuz? Ya da kullanışlı buldunuz mu?

Sekmelerin sonuna yerleşen &#8220;**+**&#8221; ikonu bir bakıma iyi düşünülmüş. Firefox ile yeni tanışan ve sekme açmak istediklerinde yeni sekme yaratabileceklerini düşündüren basit bir çözüm olmuş. Ancak [firefox klavye kısayollarına][2]{.broken_link} aşina bir insansanız muhtemelen **yeni sekme açmak** için global tuş kombinasyonu **ctrl + t** çoktan hayatınıza girmiştir. Eğer siz de benim gibi **firefox 3.5 yeni sekme butonunu kaldırmayı** düşünenlerdenseniz, aşağıdaki küçük düzenleme ile bu işlemi gerçekleştirebilirsiniz. 

Yapmanız gereken kullandığınız sistemde firefox profil dizinine gitmek. Bu dizin içerisinde **chrome** klasörü altındaki **userChrome.css** dosyasını düzenlemek olacaktır. Eğer daha önce bir düzenleme yapmadıysanız dosyanın ismini userChrome-example.css şeklinde görebilirsiniz. Yeniden isimlendirip **userChrome.css** şekline getirebilirsiniz. Akabinde ilgili dosyayı açıp en son satıra aşağıdaki bilgileri eklemeniz yeterli olacaktır. 

**.tabs-newtab-button {display: none;}**

Açık olan firefox 3.5 oturumunu kapatıp tekrar açtığınızda **firefox 3.5** ile gelen yeni sekme butonu artık olmayacaktır.

 [1]: https://www.murekkep.org/firefox-3-5-resmi-duyurusu-yapildi-3462
 [2]: https://www.murekkep.org/firefox-klavye-kisayollari-261