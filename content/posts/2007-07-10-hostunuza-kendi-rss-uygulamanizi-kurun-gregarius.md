---
title: 'Hostunuza kendi Rss uygulamanızı kurun: Gregarius'
author: Fatih
type: post
date: 2007-07-10T17:22:40+00:00
url: /hostunuza-kendi-rss-uygulamanizi-kurun-gregarius/
dsq_thread_id:
  - 197137561
categories:
  - Teknoloji
tags:
  - internet

---
Google Reader gibi bir uygulama&#8217;yı kendi alanınıza kurmanız mümkün. Neden derseniz, Google&#8217;a güvenmiyor olabilirsiniz, **Google Reader**&#8216;i sevmiyor olabilirsiniz, ya da kendinize ait web üzerinden ulaşılabilen bir uygulama istiyor olabilirsiniz. Bu sayede tüm bilgiler kendi hostunuzda olduğu için her şey kendi elinizde olacaktır. Bu yüzden **Gregarius** güzel bir şey. Gregarius açık kaynak kodlu bir uygulama ve esnek yapısı yüzünden küçük eklemeler sayesinde istediğiniz şekle girebilme özelliğine de sahip.

<center>
</center>Kurmak aslında biraz el işi ile çok kolay gelebilir size. En son paketi indirin ve web alanınızda gereken yere yerleştirin. Paketi açıktan sonra içinde 

**dbinit.php.sample** adında bir dosya görmüş olacaksınız. Bu dosyayı **dbinit.php** olarak kopyalayın ve içine şu şekilde doldurun:

`<br />
< ? php<br />
define ('DBTYPE','mysql');<br />
define ('DBNAME','greg');<br />
define ('DBUNAME','greg');<br />
define ('DBPASS', 'ŞİFRE');<br />
define ('DBSERVER', 'mysql.murekkep.org');<br />
? ><br />
` 

Burada **DBTYPE** veritabanı tipini gösteriyor, ben Dreamhost kullandığım için mysql kullandım. Dreamhost panelinden de greg(**DBNAME**) adında bir veritabanı oluşturudm, ve bu veritabanına giriş yapabilen greg(**DBUNAME**) adında bir kullanıcı oluşturdum. Şifreyi(**DBPASS**) belirledikten sonra veritabanını bulunduğu alanı da belirtim. Benimki mysql.murekkep.org(**DBSERVER**) üzerinde olduğu için onu yazdım.

Bu dbinit.php dosyasını doğru bir şekilde kurduktan sonra Gregarius&#8217;un da içinde bulunduğu kök dizinini web tarayıcısından açınız. WordPress benzeri bir kurulum sayfası gelebilir. Evet hepsi bu kadar. Daha fazlası yok. Gregarius açık kaynaklı olması yüzünden temalar ve eklentiler de destekliyor. Bunları kendi sitesinden temin edebilirsiniz. Denemek için de demo sürümünü kullanabilirsiniz.