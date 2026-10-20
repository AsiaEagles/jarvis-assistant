# Jarvis Assistant

Tamamen ücretsiz araçlarla geliştirilmek üzere tasarlanan, iPhone öncelikli Türkçe kişisel asistan prototipi.

**Canlı demo:** https://asiaeagles.github.io/jarvis-assistant/

## Şu anda çalışanlar
- Görev ekleme, tamamlama, silme ve filtreleme.
- Görevlere isteğe bağlı son tarih ve düşük/normal/yüksek öncelik verme.
- Görevleri aynı tarayıcıda yerel olarak saklama.
- Apple Takvim'e eklenmek üzere .ics etkinlik dosyası oluşturma.
- Basit komutlar ve mesaj taslağını panoya kopyalama.

## Önemli sınırlar
- Görevler şu anda yalnızca aynı cihaz/tarayıcıdaki localStorage alanında tutulur; otomatik eşitlenmez ve tarayıcı verisi silinirse kaybolabilir.
- .ics dosyası etkinliği doğrudan takvime yazmaz; dosyayı açıp Apple Takvim'e eklemeyi kullanıcı onaylar.
- WhatsApp mesajları arka planda okunmaz ve otomatik gönderilmez. Mesajlar paylaşım/kopyalama yoluyla kullanıcı tarafından aktarılır.
- GitHub Pages statik barındırmadır; sunucu tarafında kod çalıştırmaz. Site ve depo herkese açık olabilir, bu yüzden özel mesajlar, takvim verileri, parolalar veya API anahtarları depoya eklenmemelidir.
- Gelişmiş yapay zekâ özelliği henüz eklenmedi. Ücretsiz hizmetler kota ve kullanım sınırlarına tabi olabilir.

## İlkeler
- Her yeni özellik mevcut çalışan işlevleri korumalı.
- Dış işlemler kullanıcı onayıyla yapılmalı.
- Gizli anahtarlar kaynak koda eklenmemeli.
- Gerçek olmayan entegrasyonlar varmış gibi gösterilmemeli.

## Geliştirme planı
Aşamalar, kabul ölçütleri ve iPhone kısıtları için [PLAN.md](PLAN.md) dosyasına bakın.
