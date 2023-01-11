---
title: 'Firefox İpucu : Aramalarınız Yeni Sekmede Açılsın'
author: Alper
type: post
date: 2007-04-26T19:35:10+00:00
url: /firefox-ipucu-aramalariniz-yeni-sekmede-acilsin/
dsq_thread_id:
  - 197137111
categories:
  - Masaüstü
tags:
  - firefox
  - internet
  - yazılım

---
Birkaç gün önce sizlere [Firefox Klavye Kısayolları][1]{.broken_link}&#8216;ndan bahsetmiştik. Oldukça kullanışlı kısayolları küçük bir eklenti sayesinde ipucu olarak görebiliyordunuz. Bunlardan bir tanesi de Ctrl +K tuş kombinasyonu ile arama kısmına geçmek şeklindeydi. Çoğumuzun araması varsayılan olarak [Google][2] şeklindedir. Diyelim kısayol ile buraya bir arama kriteri girdiniz ve aramanızı yapacaksınız. Yapacağınız arama bulunduğunuz mevcut sekmede / sayfada açılacaktır. Bunun yeni sekmede açılması için aşağıdaki gibi bir değişiklik yapmak yeterli olacaktır.

Önce adres kısmına &#8220;**about:config** yazarak firefox konfigürasyon ekranına gidiyoruz. Ardından aşağıdaki anahtarı çağıracağız.

<pre>browser.search.openintab</pre>

Yapmanız gereken üzerine çift tıklayıp **false** olan değeri **true** yapmak olacaktır. Bundan sonra aramalarınız yeni sekmede açılır. Bir diğer alternatif yol ise arama kısmına yazdıktan sonra enter yerine &#8220;**alt+enter**&#8221; ile aramanızı yapmak olabilir.

 [1]: https://www.murekkep.org/firefox-klavye-kisayollari-261
 [2]: https://www.google.com.tr