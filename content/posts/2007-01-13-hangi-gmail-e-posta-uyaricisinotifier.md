---
title: Hangi Gmail e-posta uyarıcısını(notifier) kullanmalıyım ?
author: Fatih
type: post
date: 2007-01-13T13:18:26+00:00
url: /hangi-gmail-e-posta-uyaricisinotifier/
dsq_thread_id:
  - 968643110
categories:
  - Google
tags:
  - linux

---
Daha önce yazdığım yazılarımda da belirtiğim gibi Gmail&#8217;e geçtim. Gmail kullanan çok, ve web üzerinden olsun, ya da kendi bilgisayarındaki e-posta istemcisi ile olsun her zaman yeni e-postalar geldi mi, geldiyse ne kadar, hangi klasöre diye sorular gelir. Bunu öğrenmek için de piyasa&#8217;da bir çok Gmail bildirici programları var, ingilizce adıyla notifier. Bu yüzden de benim işimi görecek bir bildirici şart. Bu işi yapan bir çok program ve eklentiler mevcut. Bir kaç tanesini denedim, izlenimlerim aşağıdaki gibi. İlk önce Mail-watcher ile başlıyayım:

<!--more-->

<span style="font-weight: bold">1. Mail-Watcher(Xfce-eklentisi)</span>

Xfce&#8217;in paneli için hazırlanan bir eklenti. Hazır <a title="Xfce" target="blank_" href="https://www.xfce.org/">Xfce</a> kullanıyorken, pacman vasıtasıyla kurdum. Unstable deposunda kendisi mevcut. Kurduktan sonra panel&#8217;e ekledim ve sağ tıklayarak <span style="font-style: italic">properties</span>&#8216;den gereken ayarlarımı yaptım. Add butonuna tıklayarak hesap ekliyorsunuz. İstediğiniz kadar ekleyebilirsiniz. Ayarlardan, belirli aralıklarda bakmasını sağlayabilirsiniz. Ben bunu 3 dakika yaptım.Simgenin üstüne tıklayınca neler olacağını da ayarlayabilirsiniz. Burada Firefox&#8217;da yeni bir sekme açıp, gmail.com&#8217;a gitmesini yazdım. Ve yeni gelen e-postalar için de bir komut yazabilirsiniz. Örneğin <span style="font-style: italic; background-color: #c0c0c0">aplay /home/fatih/ses.wav</span> gibi, böylelikle Gmail&#8217;inize yeni e-postalar gelince seçtiğiniz ses çalacak. Zenity gibi araçlar da kullanabilirsiniz.

Sadece Gmail deyip geçmeyelim.Daha fazlası var, desteklenen protokoller aşağıdaki gibi:  
<br style="font-weight: bold" /> 

<ul type="disc">
  <li>
    IMAP (SSL/TLS)
  </li>
  <li>
    POP3 (SSL/TLS)
  </li>
  <li>
    GMail mailbox (HTTPS)
  </li>
  <li>
    Mbox mail spool (yerel)
  </li>
  <li>
    Maildir mail spool (yerel)
  </li>
  <li>
    MH-Maildir mail spool (yerel)
  </li>
</ul>

Uzun zaman önce Exim4, Mutt, Fetchmail, Procmail dörtlüsünü kullanıyordum. Örneğin Fetchmail kurulu bir bilgisayarda, Mutt kullanıyorsanız, bu eklenti sayesinde de yerel e-postalarınızdan haberdar olabilirsiniz. Benim için önemli olan tabi burada Gmail. Eklentinin kendi simgeleri aslında işinizi görür, ama bari gmail kullanıyoruz, ona uygun bir şey olsun dedim. Biraz neti aradım ve kırmızı bir simge buldum. Gimp ile de gri bir layer çektim üzerine. Eğer yeni e-postanız yoksa, o zaman gri şekilde gözüküyor. Ama yeni e-postalarınız geldiyse bunu kırmızı gmail simgesi ile gösteriyor.

Bir de eklentiyi istediğiniz yere koymakta serbestsiniz. Ben yukarı sağ köşeye yerleştirdim. Sağ tıklayarak özelliklerine giderseniz, Log diye bir bölüm daha görürsünüz. Burada çıkan hataları sizin için tutuyor.

Mail-watcher ana sayfası: https://spuriousinterrupt.org/projects/mailwatch

<span style="font-weight: bold">2. Checkgmail</span>

Checkgmail, Gtk ile yazılmış bir yazılım. Kendisi tray&#8217;e yerleşiyor, yeni e-postaları simge rengini değiştirerek ve anlık ileti çıkararak bildiriyor. Simgenin üzerine sağ tıklayınca size basit ve gerekli olan işlemlerin menüsü çıkıyor. Örneğin yeni bir e-posta yazmak için sağ tıklayarak <span style="background-color: #c0c0c0">Compose mail</span>&#8216;e tıklıyorsunuz. Sizin için ayrı bir pencere açılıyor, ve gmail hesabınızla e-postanızı yazıyorsunuz. <span style="background-color: #c0c0c0">Check mail</span>&#8216;e tıklayarak da istediğiniz zaman yeni e-posta geldi mi gelmedi mi diye öğrenebilirsiniz. Yeni gelen e-postalar için kişisel komutlar atabiliyorsunuz. Örneğin bir ses parçasını çalması gibi. Tray&#8217;e yerleşmenin bence en büyük avantajı <span style="font-style: italic">Kcheckgmail, Mailwatcher</span> gibi programlar gibi tek bir masaüstü yöneticisine bağlı olmuyorsunuz. Yani tray özelliğini destekleyen her masaüstü yöneticisinde kullanabilirsiniz. <span style="font-style: italic">Flux, Gnome, Kde, Xfce&#8230;</span> hiç fark etmiyor.

Sağ tıklayarak ayarlar tıklayarak, gerekli olan ayarlarını yapıyorsunuz. Gmail adınızı ve şifresini, kaç dakikada bir bakacağını, yeni gelen e-postalar için ne yapacağı, gibi bir sürü özelliği var. Ayrıca eğer etiket(label) kullanıyorsanız, etiketlerinizi ayrı zaman dilimlerinde bakmanızı sağlayabilir. Bunun en güzel yanı ise, mail-listelerinize üye iseniz, etiketleyip sadece her 30 dk bir bakmasını sağlayabilirsiniz. Kullandığınız dili de ayarlayabilirsiniz. Liste&#8217;e Türkçe göremedim malesef. Feed adress diye bir seçenek var, henüz ne işe yaradığını çözemedim. Bilen varsa, buraya yazabilir. Bunun haricinde, tray&#8217;deki simgeyi isteğinize göre değiştirebilirsiniz. Simgenin arka plan rengini değiştirmek de mevcut. Ben bunu hafif bir yeşil yaptım. Başka bir özellik ise, Gmail&#8217;in kişisel alanlara sağladı hizmeti de bu eklenti sayesinde kullanabilirsiniz. Birden fazla hesaba da izin veriyor.

En güzel yanı ise, yeni gelen e-postalarını nasıl bildirdiğidir. Yukarıda bahsettiğim gibi anlık bir ileti çıkıyor.

Bu anlık iletiden sonra üzerine geldiğinize bir çok işlem yapabileceğinizi görüyorsunuz. Spam olarak işaretleyebilirsiniz, silebilirsiniz, okumuş olarak işaretleyebilirsiniz, arşivinize ekleyebilirsiniz. Kimden geldiğini ve kaç tane e-posta geldiğini de gösteriyor. Küçük bir rapor gibi.

Checkgmail ana sayfası : <a title="https://checkgmail.sourceforge.net/" target="blank_" href="https://checkgmail.sourceforge.net/">https://checkgmail.sourceforge.net/</a>

<span style="font-weight: bold">3. Gmail Checker</span>

Gmail Checker bir Firefox eklentisi. Bir çok eklenti mevcut bu alanda, ama en sade olanı <span style="font-weight: bold">Gmail Checker,</span> Gmail ismini ve şifrenizi yazıyorsunuz o kadar. Simge sağ alt köşede yerini alıyor. Tek bir ayar kısmı var, o da kaç dakikada bir bakacağını söylüyor. Varsayılan olarak 15 dk, ben bunu 2 dk diye değiştirdim. Ayrıca üzerinde sol-tıklama yaparsanız da e-postalara bakıyor. Bir de, örneğin 4 tane e-posta geldi. Simgenin üzerine sağ tıklayınca size liste halinde gösteriyor. Hanisini okumak istiyorsanız onu açıyor. Ama dikkat edin, arka planda bir sekme olarak açmıyor, direkt kullandığınız sayfada açıyor.

Gmail Checker için eklenti sayfası : https://addons.mozilla.org/firefox/3179/

 <span style="font-weight: bold">4. Diğer uyarıcılar</span>

Bunun haricinde bir çok uyarıcı daha var. Onlara da bakabilirsiniz. Kde için de <a title="kcheckgmail" target="blank_" href="https://sf.net/projects/kcheckgmail">kcheckgmail</a> uygulaması var. Kcheckgmail ise tahminimce checkgmail&#8217;in kde&#8217;ye uyarlanmış hali. Bilmiyorum bunu, kullananlar varsa, buraya yazabilirler. Firefox için de eklentiler mevcut. Küçük bir simge olarak durum çubuğuna yerleşen eklentiler var :Gmail Manager, Gmail Notifier. Bu iki eklenti de ben&#8217;de çalışmadığı için deneyemedim. Ama Gmail Manager&#8217;in çok kapsamlı olduğunu biliyorum.

 <span style="font-weight: bold">5. Sonuç</span>

Birinci sırada tartışmasız Checkgmail var. Gerek sağladı özellikler, gerekse tasarım ve kullanabilirlik açısından en iyisi. Ayrıca Masaüstü yöneticisine bağlı olmaması da büyük bir avantaj. İkinci sırada ise Mail-Watcher var. Xfce&#8217;a direkt entegreli olduğundan kolayca kullanabiliyorsunuz. Ayrıca sadece Gmail değil de Pop ve İmap desteği olduğu için de ek bir avantajı var. Fakat yazı Gmail ile ilgili olduğu için ilgilendirmiyor bizi şimdilik. Üçüncü sırada ise en sade ve en basiti olan Gmail Checker geliyor. Hiç bir paket yüklemeniz gerekmiyor, sadece 10-20kb büyüklüğünde bir eklenti. Eksiği ise, Firefox&#8217;a bağlı olmanız ve hemen hemen hiç özelliği olmaması.