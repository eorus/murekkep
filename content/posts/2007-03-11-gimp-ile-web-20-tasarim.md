---
title: Gimp ile Web 2.0 Tasarım
author: Alper
type: post
date: 2007-03-11T08:44:13+00:00
url: /gimp-ile-web-20-tasarim/
dsq_thread_id:
  - 197136766
categories:
  - Masaüstü
tags:
  - linux
  - yazılım

---
Geçen Pazar günü itibariyle, daha önce okuduğum, notlar aldığım ve üzerinde gerçekten oldukça amatörce uğraştığım Gimp ile belirli şeyler oluşturma konusunda ciddi bir adım atmıştım. Yukarıda gördüğünüz gölgeli Murekkep.Org yazısını ve [tag]web 2.0[/tag] ile klasik haline gelen yıldız çerçeveli kısmı oluşturdum. Nihayet haftasonu geldi ve hafta boyunca yazmayı düşündüğüm bu yazıyı hayata geçirebilirim. Tabi ara teşvik olarak Volkan Karakuş&#8217;un photoshop üzerinde uygulayıp güzel bir makaleye dönüştürdüğü &#8220;Web 2.0 Sticker (etiket) Yapımı&#8221; yazısını unutmamak gerekir. Photoshop ile nasıl için faydalanabilirsiniz. Bayağı uzun bir yazı olacak, o yüzden başlayalım :

<!--more-->

**1. Arkaplan Oluşturma** 

Gimp&#8217;i açıyoruz. Yeni bir layer oluştur dedikten sonra aşağıdaki gibi genişliğini ve yüksekliğini belirtmemiz gereken yeni resim oluşturma kısmı geliyor. Burada ben header resmi olarak düşündüğüm için 980 genişlik ile 150 yükseklik verdim. Bunun dışında varsayılan gelen ayarlar dışında sadece &#8220;**Advanced Options**&#8221; içerisinde Fill with kısmını &#8220;**White**&#8221; olarak belirliyoruz.

<p style="text-align: center">
  <p>
    Ve karşımıza arka planı beyaz olan 980&#215;150 boyutunda bir layer çıkıyor.
  </p>
  
  <p style="text-align: center">
    <p>
      Üstüne yazımızı yazmadan önce arkaplanı gradient editör ile istediğimiz şeffaflığa getireceğiz. Bunun için Gimp kanallarından gradient butonunu seçiyoruz. <strong>FG to BG (RGB)</strong> Foreground to Background geçiş şeklini seçtikten sonra alt kısımdan yeni gradient oluşturma butonuna basıyoruz ve karşımıza gradient editör çıkıyor.
    </p>
    
    <p>
      Gimp burada oluşturduğumuz gradient için geçişlerin nasıl olacağını ve hangi renkleri kullanacağımızı belirlememizi istiyor. Açılan Gradient Editor&#8217;de önce bir isim verelim. Adı &#8220;Arkaplan Geçişi&#8221; olsun. Sonra resmin içerisinde bir yere sağ tıklayın ve “Split segments at midpoint&#8221; seçin. Bunu yaptıktan sonra alt kısımda 3 siyah 2 beyaz üçgen olduğunu göreceksiniz. Şimdi görmüş olduğunuz o iki beyaz üçgenden soldakine çift tıklayın ve seçtiğinize emin olun. Bu beyaz üçgene sağ tıklayın ve “<strong>Left Endpoint’s Color</strong>” seçin. Buradan sol kısım, sol taraf için geçiş renginizi belirleyin. Ben <span style="font-size: 0.8em; color: #cdeb8b">#CDEB8B</span> seçtim. Şimdi aynı beyaz üçgene gene sağ tıklayın ve “<strong>Right Endpoint’s Color</strong>” seçin. Buradan da sol kısım, sağ taraf için renginizi belirleyin. Ben beyaz #FFFFFF seçtim. Aynı işlemi sağ taraftaki kısma da uygulayın. Yani sağ taraftaki beyaz üçgene çift tıklayın, sol ve sağ renkleri belirleyin. Ben sağ tarafı tamamen beyaz seçtim. Yani hem Left hem de Right Endpoint&#8217;s Color kısımlarına #FFFFFF verdim. Sonuçta resimdeki gibi bir durumun oluşması gerekiyor. Ancak burada renk seçimini belirli oynamalarla istediğiniz gibi belirliyorsunuz. Kaydet butonuna basıp Gradient Editör&#8217;den çıkın.
    </p>
    
    <p>
      Bu aşamada elimizde Gimp&#8217;in hazır gradientleri dışında kendi renklerimiz ve geçişlerimizle oluşmuş bir gradient var. Bunu hazırladığımız 980&#215;150 beyaz arkaplana uygulamak için Gimp butonlarının olduğu sol kısımdan gradient tool seçimini yapıyoruz.
    </p>
    
    <p style="text-align: center">
      <p>
        Hemen alt kısımda, oluşturduğumuz gradientin renklerini göreceksiniz (reverse kutusunun yanı). Orada seçili olduğuna emin olun. Bu aşamada fareniz ile beyaz arkaplanın üzerine bu gradienti atıyorsunuz. Eğer benim istediğim gibi yukarıdan aşağı doğru gelmesini istiyorsanız, layerın orta kısmında üstten aşağı doğru bir seçim yapabilirsiniz.
      </p>
      
      <p style="text-align: center">
        <p>
          Böyle bir seçim yaptığınızda sonuç aşağıdaki gibi olacaktır. Ancak tavsiyem ilk uğraşınızda elinizden geldiği kadar farklı yöntemler denemeniz olacaktır. Yani farenizi sol üstten sağ alta doğru çekebilirsiniz. Ya da daha farklı bölgede daha küçük bir alana uygulayabilirsiniz. Böylelikle gözünüze en hoş gelecek arkaplanı denemelerle oluşturabilirsiniz.
        </p>
        
        <p style="text-align: center" align="left">
          <p>
            <strong>2. Arkaplana Metin Ekleme</strong>
          </p>
          
          <p>
            Arkaplanımızı oluşturduk. Şimdi arkaplan üzerine metin koyacağız. Bu gerçekten işin oldukça kolay kısımlarından birisi. Gimp butonlarından <strong>&#8220;T&#8221;</strong> şeklinde gözüken metin ekleme aracını seçin. Seçtiğiniz zaman alt kısımda yazıtipi, yazıtipi boyutu ve yazının rengini belirlemek için renk paletini göreceksiniz. Eminim daha güzel yazıtipleri vardır. Ben başlangıç için <strong>&#8220;Arial Bold&#8221;</strong> seçtim ve yazıtipi boyutunu <strong>&#8220;60&#8221;</strong> olarak belirledim. Rengini de <a href="http://digg.com/" title="Digg">Digg</a> mavisi olan <span style="font-size: 0.8em; color: #356aa0">#356AA0</span> şeklinde belirledim.
          </p>
          
          <p>
            Bu belirlemelerinizi yaptıktan sonra yukarıda oluşturduğumuz arkaplan üzerine tıklayın. Metin yazma kutusu karşınıza çıkacaktır. Metninizi yazarken arkaplanda gözükecektir. Metnin yeri konusunda endişelenmeyin. İstediğiniz her zaman yukarı uçları ok şeklinde artı butonuyla (move) yerini değiştirebilirsiniz. <strong>&#8220;Mürekkep.Org&#8221;</strong> yazdık. Aşağıdaki gibi bir görüntü oluştu.
          </p>
          
          <p style="text-align: center">
            <p>
              Şimdi oluşturduğumuz bu metne gölgeleme vereceğiz. Bunun için öncelikle Gimp kanallarında görülen yeni metin kısmını <strong>&#8220;duplicate layer&#8221; </strong>yapıp bir kopyasını oluşturacağız. Bu bizim üzerinde gölgeleme çalışacağımız layerımız olacak. Aşağıdaki resimde &#8220;Mürekkep.Org&#8221; yazan kısma sağ tıklayıp duplicate layer yaptım. Soldaki resim önceki halini, sağdaki ise bir kopyasının oluşmuş halini gösteriyor.
            </p>
            
            <p style="text-align: center">
              <p>
                Bu aşamadan sonra gölgeleme ile ilgili anlatacaklarım yeni oluşturduğumuz kopyalanmış layer üzerinden olacak. Şimdi bu şekilde seçiliyken arkaplan resmimizin menüsünden sırayla <strong>Layer > Transform > Flip Vertically</strong> seçiyoruz. Kopyalanmış metnin ters döndüğünü göreceksiniz. Burada soldaki butonlardan <strong>&#8220;move&#8221;</strong> butonunu seçip, ikinci ters dönmüş metni ana metnin alt kısmına doğru getiriyoruz. Harflerin uçlarının birbirine dokunduğundan ve tam denk geldiğinden emin olun.
              </p>
              
              <p>
                Şimdi gimp kanallarında yeni kopyalanmış layer adının üzerine sağ tıklayın. <strong>&#8220;Add Layer Mask&#8221;</strong> seçin. Karşınıza ilk seçenek (<strong>White/Full Opacity</strong>) seçili gelecektir. Tamam diyip kapatmış olun. Bu aşamada Yukarıda Gradient butonunu seçerek nasıl fare ile geçiş verdiğimizden bahsetmiştik. Aynsını yapın. Yani gradient aracını seçin. Bu sefer yeni bir gradient oluşturmanıza gerek yok. Hazır Gimp gradientlerinden <strong>FG to Transparent</strong> seçili olsun ve siyah renki alın. Farenizi ters olan metin üzerinde aşağı yukarı oynatarak gölgelemeyi verin. Gölgeleme dozu size kalmış tabii ki. Sonuç olarak bende aşağıdaki gibi bir durum oluştu.
              </p>
              
              <p style="text-align: center">
                <p>
                  <strong>3.Etiket (Sticker) Ekleme</strong>
                </p>
                
                <p>
                  Arkaplanı hazırladık. Metnimizi ekledik. Şimdi [tag]web 2.0[/tag] ile görmeye başladığımız kenarı yıldızlı ve içerisinde beta gibi birşey yazacak etiketi oluşturmak. İşe koyulmadan önce Gimp kanallarından arkaplanı seçiyoruz ki tüm alan seçili olsun. Sonra sırasıyla <strong>Filters > Render > Gfig</strong> seçimini yapıyoruz. Karşımıza oluşturduğumuz arkaplan ve metin ile beraber çalışabileceğimiz bir alan çıkıyor. Üstteki ikonlardan yıldız olanı seçiyoruz. Seçimi yaptıktan sonra sağ kısımda yıldız için ayarlayabileceğimiz özellikler çıkacak. Önce sides kısmını 12 &#8211; 13 gibi bir değer ile değiştiriyoruz. Bu oluşacak yıldızın kenar sayısını ifade ediyor. Browse ile daha küçük bir nokta seçiyoruz. Renk olarak ise ben Flickr rengi olan <span style="font-size: 0.8em; color: #ff0084">#FF0084</span> pembesini seçtim. Fill kısmında &#8220;<strong>Color Fill</strong>&#8221; seçiyoruz. Böylelikle yıldızın kenarlarını da pembe yapacağız. Şimdi yıldızı metnin yanında oluşturun. Yer konusu olarak endişeniz olmasın, istediğiniz zaman yerini değiştirebilirsiniz. Yukarıdaki butonlarda yanyana iki tane buton bulunuyor. Bir tanesi &#8220;<strong>Move an object</strong>&#8221; diğeri ise &#8220;<strong>Move a single point</strong>&#8220;. Yıldızı bir obje olarak düşünün, objenin komple yer değiştirmesi için birinciyi, obje üzerindeki kısımlarla oynamak için ikinciyi kullanacaksınız. Önemli olan açıkçası ikinci olan &#8220;Move a single point&#8221;. Resimde de gördüğünüz gibi yıldız oluştuktan sonra üzerinde üç tane siyah nokta beliriyor. Her nokta ayrı bir amaca hizmet veriyor. Bir tanesi yıldız kenarlarını dik ya da yayvan yaparken, bir diğeri yıldızın çerçevesini küçültüyor. Burası tamamen size kalmış durumda. Bir miktar oynama ile beğeninize göre bir sonuç oluşacaktır. Aşağıda Gfig ekranından çıkmış haliyle arkaplan gözüküyor.
                </p>
                
                <p style="text-align: center">
                  <p>
                    Şimdi önce Gimp butonlarından belirli bölgeyi seçme butonunu seçiyoruz. Ve bununla oluşan yıldızın üzerine tıklayıp seçili olmasını sağlıyoruz. Yıldızın iç kısmına gradient ile gölge atacağız. Bunu yukarıda anlatmıştım. Aynı işlemi yıldız içerisine uyguluyoruz. İç kısmın rengini gene pembe seçiyorum. Sonra seçili haldeyken komple yıldıza gölge vermek için <strong>Script-Fu > Shadow > Drop Shadow</strong> kısmından varsayılan gelen değerleri dikkate alıp tamam diyorum. Burada alt,üst gölge ve gölge rengini siz belirleyebilirsiniz. Gölge rengi siyah gelmişti aynı şekilde kullandım. Son gelinen nokta aşağıdaki gibi gözüküyor.
                  </p>
                  
                  <p align="center">
                    <p>
                      Yapılacak fazla bir iş kalmadı Yıldızın içine birşeyler yazmak lazım. Ben çok moda olan <strong>Beta</strong> yazısını yazmayacağım. Onun yerine <strong>Yeni</strong> yazacağım. Yukarıda belirttiğim şekilde <strong>&#8220;T&#8221;</strong> butonu ile metin ekleme yapıp, boyutunu ayarlayıp yıldız içerisine yazmak istediğiniz metni ekliyorsunuz. Burada yapacağımız tek ek işlem, eklenen yazının çaprazlama şekilde yerleşmesi olacaktır. Metni ekledikten sonra <strong>Rotate</strong> butonu ile yazıyı döndürebilirsiniz. Böylelike oluşturmak istediğimiz çalışmanın son hali aşağıdaki gibi oluşuyor.
                    </p>
                    
                    <p style="text-align: center">
                      <p>
                        Evet, bitti. Biraz uzun oldu belki ama en azından benim gibi nasıl yapabilirim diye etrafa bakan arkadaşlara faydası dokunacaktır. Buraya eklediğim resimler olsun, anlatım şekli olsun, eğer hatalı gördüğünüz ya da eklemek istediğiniz kısımlar varsa mutlaka belirtiniz. Benim de ilk defa denediğim birşey olduğundan sürç-i lisan ettiysek affola / Alper.
                      </p>
                      
                      <p>
                        http://www.gimp.org/
                      </p>