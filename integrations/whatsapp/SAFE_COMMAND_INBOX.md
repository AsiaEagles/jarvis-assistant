# Kişisel WhatsApp ile Jarvis — güvenli seçenekler

## Önemli sınır
WhatsApp Messenger kişisel hesapları için genel kullanıma açık, resmi bir bot API'si bulunmuyor. WhatsApp'ın resmi otomasyon ürünü WhatsApp Business Platform'dur ve şartları kişisel kullanım için değil, işletmelerin yetkili iş amaçlı kullanımı için düzenlenmiştir. Resmî yardım sayfaları yetkisiz otomatik/bulk mesajlaşmanın hesabın kısıtlanmasına yol açabileceğini belirtiyor.

Kaynaklar:
- WhatsApp'ın yetkisiz otomatik mesajlaşma hakkındaki yardım sayfası: https://faq.whatsapp.com/5957850900902049/
- WhatsApp'ın kullanım şartları: https://www.whatsapp.com/legal/terms-of-service
- WhatsApp Business Platform SSS: https://whatsappbusiness.com/resources/faq/
- WhatsApp Business Platform şartları: https://www.whatsapp.com/legal/WhatsApp-Terms-for-WhatsApp-Business-Platform

## Seçenekler

### A — Ücretsiz ve en düşük risk (önerilen ilk aşama)
1. WhatsApp'ta gelen komutu seçip kopyala.
2. Jarvis panelindeki **Komut kutusu**na yapıştır.
3. Jarvis yalnızca desteklediği basit komutları yerel olarak işler.
4. Görev ekleme gibi değişiklikleri panelde sen görürsün; mesaj göndermez ve WhatsApp hesabına bağlanmaz.

Artısı: ücretsiz, kişisel hesabını değiştirmez, oturum çerezi veya QR kodu paylaşımı gerektirmez.
Eksisi: WhatsApp'tan Jarvis'e otomatik aktarım yoktur.

### B — Resmî WhatsApp Business Platform
İşletme amaçlı ve uygun bir WhatsApp Business hesabı gerektirir; kişisel WhatsApp hesabına doğrudan bağlanma yolu değildir. Ücretlendirme ve uygunluk kuralları vardır. Kişisel kullanım için bu projede önerilmiyor.

### C — WhatsApp Web'i otomatik okuyan üçüncü taraf araçlar
Önerilmiyor. Resmî olmayan oturum otomasyonu/mesaj kazıma; hesap kısıtlaması, gizlilik ve güvenlik riski doğurabilir. QR oturumunu, çerezleri veya telefon doğrulama kodunu üçüncü taraflara verme.

## İlk sürümün komutları
- `yardım` — desteklenen komutları göster.
- `görev ekle: market alışverişi` — panelin görev listesine bir görev ekler.
- `mesaj taslağı: Yarın 10'da arayacağım` — mesaj taslağını hazırlar; göndermez.
- `takvim` — demo takvim bilgisini gösterir.

Bu sürüm yalnızca tarayıcıdaki demo arayüzünü değiştirir. Komutlar sunucuya gönderilmez, WhatsApp'tan otomatik mesaj okunmaz ve gerçek takvime erişilmez.
