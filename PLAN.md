# Jarvis — Uygulama Planı

## Hedef
Ücretsiz araçlarla başlayıp web paneli ve WhatsApp üzerinden kullanılabilen kişisel bir asistan oluşturmak.

## Aşamalar

### 1. Güvenli prototip
- Türkçe, mobil uyumlu web paneli.
- Örnek görevler ve takvim verileri yalnızca demo amaçlıdır.
- Henüz gerçek hesaplara bağlanmaz.

### 2. Apple Calendar
- Önce yalnızca takvim etkinliklerini okuma.
- macOS üzerinde yerel köprü veya iCloud CalDAV seçeneklerini değerlendir.
- Kimlik bilgilerini kaynak koduna koyma; ortam değişkenleri ve yerel gizli dosyalar kullan.

### 3. WhatsApp
- Kişisel WhatsApp için genel amaçlı, resmi bir bot API'si bulunduğunu varsayma.
- Desteklenmeyen WhatsApp Web oturum otomasyonunu kullanma.
- İlk aşamada mesaj taslağı hazırla; gönderimi kullanıcı elle onaylasın.
- Otomatik gönderim ancak resmi, desteklenen bir çözüm ve açık onay varsa değerlendirilsin.

### 4. Yayınlama
- Ücretsiz statik barındırma ile arayüz prototipi yayınlanabilir.
- Takvim erişimi ve kişisel veriler için sunucu gerekiyorsa güvenli dağıtım ve olası maliyetleri ayrıca değerlendir.
- Gizli anahtarları GitHub'a commit etme.

## İlk sürümde yok
- Gerçek takvim bağlantısı
- Gerçek WhatsApp gönderimi
- Arka planda çalışan ajan
- Hassas işlemlerin otomatik onayı