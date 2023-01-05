---
title: Microsoft Surface RT Dokunmatik Hassasiyetini Arttırma
author: bkazar
type: post
date: 2013-01-27T10:49:13+00:00
url: /microsoft-surface-rt-dokunmatik-hassasiyetini-arttirma/
featured_image: /wp-content/uploads/2012/11/microsoft-surface-rt-100x100.jpg
categories:
  - Mobil
tags:
  - microsoft
  - tablet

---
Windows’un ilk sürümünden bu yana kullanıcılar performansı arttırmak, kendi tercihlerine göre düzenlemek için Registry ayarlarını değiştirdiler. Peki her Windows cihaz, özellikle de yeni **Windows 8** işletim sisteminde Registry ayarları değiştirilebilir mi? Tabi ki evet.

Bu yazımızda birkaç registry ayarını değiştirerek Windows 8 ile çalışan Microsoft Surface RT tabletinizin dokunmatik ekran hassasiyetini nasıl arttıracağınızı anlatacağız. Aslına bakarsanız hassasiyet demek çok da doğru değil. Bu ayarlarla tablet ekranına dokunduğunuz an ile tabletin dokunuşu algılama süresini azaltacağız.

Lafı çok fazla uzatmadan konumuza geçelim. Ancak başlamadan belirtelim, registry ayarlarını değiştirmek geri dönülmez hatalara neden olabilir. Riski göze alıp bu işlemi yapın.

### Windows 8 Microsoft Surface RT Dokunmatik Hassasiyetini Arttırma

&nbsp;

  * **<img class="wp-image-9461 alignright" alt="microsoft-surface-rt" src="https://www.murekkep.org/wp-content/uploads/2012/11/microsoft-surface-rt-400x310.jpg" width="288" height="223" srcset="https://www.murekkep.org/wp-content/uploads/2012/11/microsoft-surface-rt-400x310.jpg 400w, https://www.murekkep.org/wp-content/uploads/2012/11/microsoft-surface-rt-50x38.jpg 50w, https://www.murekkep.org/wp-content/uploads/2012/11/microsoft-surface-rt-160x125.jpg 160w, https://www.murekkep.org/wp-content/uploads/2012/11/microsoft-surface-rt.jpg 764w" sizes="(max-width: 288px) 100vw, 288px" />**Arama alanına **regedit** yazın ve ilk sonuca tıklayın
  * **HKEY\_LOCAL\_MACHINE\SOFTWARE\Microsoft\Tou  
    chPredict ion** sekmesini takip edin
  * **“****latency****”** ve **“****sample time****”** değerlerin**i** **8** yerine **2** **yapın**
  * Registry’den çıkın ve tableti yeniden başlatın

Gizmodo ve XDA Developers forumlarında bu ipucunu uygulayanların geri dönüşleri tamamen olumlu. Bu işlemin batarya ömrünü düşürmediği de ayrıca belirtilmiş. Bir Microsoft RT tabletim olmadığından bizzat yapıp sonuçları paylaşamıyorum, kusuruma bakmayın =)