# iPhone: kişisel WhatsApp → Jarvis

## Gerçekçi sınır
iOS, WhatsApp Messenger'ın gelen mesajlarını başka bir uygulamaya genel bir otomasyon tetikleyicisi olarak açmaz. Apple Shortcuts, bir kısayolun Paylaşım Sayfası üzerinden başka bir uygulamadan içerik almasını destekler; bu, WhatsApp'ın her mesajı otomatik olarak Jarvis'e aktardığı anlamına gelmez. Kullanıcı bir mesajı/ içeriği özellikle paylaşmalı ve kısayolu çalıştırmalıdır.

Kaynaklar:
- Apple: kısayolları başka bir uygulamanın Paylaşım Sayfasından çalıştırma: https://support.apple.com/guide/shortcuts/apd163eb9f95/ios
- Apple: kısayol girdisi türleri: https://support.apple.com/guide/shortcuts/apd7644168e1/ios
- WhatsApp kullanım şartları: https://www.whatsapp.com/legal/terms-of-service
- WhatsApp: otomatik veya toplu mesajlaşma uygulama yasağına dair rehber: https://faq.whatsapp.com/361005896189245/

## Önerilen ücretsiz akış
1. iPhone'da **Kestirmeler (Shortcuts)** uygulamasını aç.
2. Yeni bir kısayol oluştur; adını **Jarvis'e aktar** koy.
3. Kısayol ayrıntılarında **Paylaşım Sayfasında Göster (Show in Share Sheet)** seçeneğini aç.
4. Kabul edilen giriş olarak **Metin (Text)** seç. WhatsApp, bazı mesaj türlerini veya sürümlerinde metni paylaşım sayfasına aktarmayabilir; bu yüzden önce basit bir metinle test et.
5. Eylem olarak **Panoya Kopyala (Copy to Clipboard)** ekle.
6. Ardından **Uygulamayı Aç (Open App)** eylemiyle Safari'yi veya Jarvis'in web panelini aç. (Kısayol içeriği otomatik aktarmıyorsa Jarvis komut kutusuna kendin yapıştır.)
7. WhatsApp'ta desteklenen bir mesajı paylaşma/iletme ekranından kısayolu çalıştır; Jarvis panelinde metni yapıştır ve **Komutu işle**ye bas.

Bu akış gelen tüm mesajları otomatik izlemez. Kullanıcının seçip paylaşması gerekir. Bazı WhatsApp içerik türlerinde metin paylaşımı görünmeyebilir; o durumda metni kopyalayıp Kestirme'yi ayrıca çalıştır.

## Güvenlik
- WhatsApp QR kodunu, oturum çerezlerini veya doğrulama kodunu hiçbir servise verme.
- Gelen mesajları otomatik komut olarak körü körüne çalıştırma. Para transferi, silme, mesaj gönderme, dosya açma gibi hassas işlemlerde ayrı onay gerektir.
- Mesaj metni kişisel bilgi içerebilir; bunu herkese açık URL parametresine veya herkese açık depoya koyma.
- Bu akış yerel panoyu ve kullanıcının seçtiği metni kullanır; WhatsApp'a otomatik giriş yapmaz, gelen mesajları taramaz ve otomatik mesaj göndermez.

## Tam otomasyon için
Kişisel WhatsApp + iPhone kombinasyonunda, tüm gelen mesajları güvenli ve ücretsiz biçimde otomatik algılayan desteklenen bir yol doğrulanmış değildir. Böyle bir özellik temel ihtiyaçsa WhatsApp dışı bir kanal (ör. Telegram botu) ya da uygun şartlarda resmî bir iş entegrasyonu ayrı değerlendirilmelidir. Bu seçenekler kişisel WhatsApp'ı otomatik izliyormuş gibi sunulmamalıdır.
