---
title: Linux Masaüstünüzdeki Resimlerinizi Flickr Düzenleyici (DFO) ile Organize Edin
author: Alper
type: post
date: 2007-08-08T13:41:12+00:00
url: /linux-masaustunuzdeki-resimlerinizi-flickr-duzenleyici-dfo-ile-organize-edin/
dsq_thread_id:
  - 197137724
categories:
  - Masaüstü
tags:
  - bilişim
  - fotoğraf paylaşım
  - linux
  - yazılım

---
> _Birincisi Linux altında hemen hemen hiç bir tane karşı tarafa yükleme yapacak program yok. Her seferinde Picasa’ya gidip, site üzerinden yüklemek işime gelmiyordu, hoşuma da gitmiyordu. Hoş F-spot var, fakat o da adam gibi çalışmıyor ve çok hantal. Oysa Flickr için yüzlerce betik,program var._

Yukarıdaki yazı [Mürekkep][1] yazarı Sevgili Fatih&#8217;in üç gün önce kendi blogu Arslanlar Şehri&#8217;ndeki serzenişinden küçük bir alıntıydı. Konunun öncesine bakarsak Fatih, Picasa ve Flickr&#8217;yi masaya yatırmış. Uzun ve faydalı bir yazı ile birçok açıdan bu iki siteyi karşılaştırmıştı. **[Picasa vs. Flickr][2]{.broken_link}**. Daha önceki sohbetlerimizde hep Picasa&#8217;ya masaüstünden erişim için düzgün bir program bulamama derdimiz vardı. Buna nazaran Fatih&#8217;in bahsettiği gibi Flickr için çok sayıda betik, program var. Ben de bunlardan bir tanesi olan [**Desktop Flickr Organizer**][3]&#8216;dan (DFO) bahsedeceğim.

<p style="text-align: center">
  <p>
    DFO bir mono uygulaması olup linux üzerinde sadece gnome masaüstünde çalışıyor. Sitesinde kurulum için Ubuntu Feisty baz alınmış ve mono bağımlılıkları için <em>mono, libmono-sqlite2.0-cil, libgconf2.0-cil, gtk-sharp2</em> paketlerinin kurulması gerektiği belirtilmiş. Archlinux üzerinde mono paketi kurulu olduğu için DFO&#8217;nun run.sh betiğini &#8220;<strong>sh run.sh</strong>&#8221; olarak çalıştırmam yeterli oldu. Sonuçta mono kurulu bir Gnome masaüstünde herhangi başka bir kurulum gerekmeden çalıştırıp kullanabiliyorsunuz. İçerik olarak DFO&#8217;nun en güzel tarafı basit olması ve neredeyse birebir Flickr&#8217;nin kendi web aracı olan Organizr&#8217;ye benzemesi diyebilirim. Yeni set yaratma, düzenleme, etiketleri, tanımları ve resim için izin haklarını düzenleme gibi <a href="https://www.flickr.com/help/organizr/" class="broken_link">Organizr</a> ile ne yapabiliyorsanız hemen hemen hepsini DFO aracılığı ile masaüstünüzden yapabiliyorsunuz. (Komple bir seti silme ya da set içerisindeki resimlerinizi tekrar belli bir sıraya koyma işlemini yapamıyorsunuz)
  </p>
  
  <p>
    DFO dışında Flickr için Linux masaüstünde kullanabileceğiniz diğer alternatiflere bakacak olursak;
  </p>
  
  <ul>
    <li>
      <a href="https://nozell.com/blog/archives/2004/09/04/flickr-upload-for-gnomes-nautilus/" class="broken_link">Flickr Upload (Nautilus için)</a>
    </li>
    <li>
      FlickrUploadr
    </li>
    <li>
      <a href="https://search.cpan.org/~cpb/Flickr-Upload/flickr_upload">Flickr_Upload (Terminalden)</a>
    </li>
    <li>
      jUploadr (Java tabanlı)
    </li>
  </ul>

 [1]: https://www.murekkep.org/
 [2]: https://www.murekkep.org/picasa-vs-flickr-hangisi-daha-iyi-254
 [3]: https://code.google.com/p/dfo/