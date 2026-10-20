# Jarvis — Geliştirme Yol Haritası

## Nihai hedef
Tamamen ücretsiz araçlarla, iPhone'da rahat kullanılan; görevleri, günlük planı, takvim etkinliklerini, WhatsApp'tan kullanıcı tarafından paylaşılan mesajları ve ses/Kestirmeler akışını tek yerde birleştiren kişisel asistan.

## Temel ilkeler
- Önce çalışan, küçük adımlar; her aşamada mevcut işlevleri koru.
- Kullanıcı onayı olmadan mesaj gönderme, etkinlik kaydetme veya başka dış işlem yapma.
- Gizli anahtar, parola, özel mesaj ve kişisel takvim verilerini herkese açık GitHub deposuna koyma.
- Ücretsiz planlarda kota, hız sınırı veya erişim değişikliği olabilir; “ücretsiz” bir hizmeti sınırsız varsayma.
- Gerçek bir entegrasyon hazır değilse arayüzde demo olduğunu açıkça belirt.

## Mevcut prototipte doğrulananlar
- [x] Türkçe, mobil uyumlu statik web paneli.
- [x] Görev ekleme, tamamlama ve silme.
- [x] Görevleri aynı tarayıcıda localStorage ile saklama.
- [x] Takvim etkinliği için .ics dosyası oluşturma; Apple Takvim'e eklemeyi kullanıcı onaylar.
- [x] Basit metin komutları ve mesaj taslağını kopyalama.
- [x] WhatsApp'a otomatik erişim/gönderim olmadığını açıklayan gizlilik notu.

## Aşamalar

### Aşama 1 — Güvenilir temel ve görev yönetimi
- [ ] Görevlere son tarih ve öncelik ekle.
- [ ] Açık/tamamlanan görevleri filtrele ve gecikmiş görevleri belirginleştir.
- [ ] Eski localStorage kayıtlarıyla geriye dönük uyumluluğu koru.
- [ ] iPhone Safari'de ekleme, yenileme, tamamlama ve silme testlerini yap.
- Kabul ölçütü: Yenilemeden sonra görevler kalır; son tarih/öncelik doğru görünür; mevcut görevler kaybolmaz.

### Aşama 2 — Takvim akışını iyileştir
- [ ] .ics dosyasının tarih/saat ve notlarını doğrula; Avrupa/Berlin saat dilimini kullan.
- [ ] Etkinlik dosyasını oluşturduktan sonra iPhone'da açma ve Takvim'e ekleme adımlarını kısa şekilde göster.
- [ ] Kestirmeler uygulamasındaki “Yeni Etkinlik Ekle” eylemini alternatif manuel akış olarak belgele.
- Sınır: Statik GitHub Pages, tek başına iCloud takvimine doğrudan ve güvenli erişim sağlayan sunucu değildir. İlk sürüm .ics veya Kestirmeler ile kullanıcı onaylı çalışır.

### Aşama 3 — WhatsApp paylaşım akışı
- [ ] iOS Kestirmeleri “Paylaşım Sayfasında Göster” üzerinden gelen metni kabul edecek şekilde kullanıcı kılavuzunu tamamla.
- [ ] Paylaşılan metinden görev/cevap taslağı üretme akışını netleştir; önce metni kullanıcı kontrol eder.
- [ ] Gönderim için WhatsApp uygulamasına geçiş ve son onayı kullanıcıya bırak.
- Sınır: Jarvis, WhatsApp konuşmalarını arka planda okuyamaz; statik web sitesi kişisel WhatsApp oturumuna bağlanmaz. Kullanıcı tarafından paylaşılan/kopyalanan içerik kullanılabilir.

### Aşama 4 — iPhone ana ekranı, Kestirmeler ve ses
- [ ] Safari'den ana ekrana ekleme yönergesi hazırla.
- [ ] Kestirmeler ile paneli açma, panodaki metni alma ve kullanıcıya sonucu gösterme akışını belgele.
- [ ] iOS'un izin verdiği sesli dikte/Siri adımlarını test et.
- Sınır: Her otomasyon tetikleyicisi onaysız çalışmaz; bazı eylemler izin/etkileşim ister. Web sayfası sürekli arka planda çalışan yerel bir iPhone uygulaması değildir.

### Aşama 5 — Akıllı asistan
- [ ] Önce ücretsiz ve anahtarsız, cihaz üzerinde yapılabilecek basit komut ayrıştırma/planlama.
- [ ] Daha gelişmiş doğal dil için ücretsiz kullanım katmanı olan bir model/servis bulunursa gizlilik, kota ve şartlarını değerlendir.
- [ ] API anahtarını hiçbir zaman tarayıcıdaki JavaScript'e veya herkese açık depoya koyma. Sunucu gerekiyorsa yalnızca gerçekten ücretsiz ve güvenli seçenek doğrulanırsa ekle.
- Kabul ölçütü: Yapay zekâ mevcut değilken de temel görev ve takvim özellikleri çalışır; başarısız bağlantı anlaşılır şekilde bildirilir.

### Aşama 6 — Birleştirme ve sağlamlık
- [ ] Günlük görünüm: bugünkü görevler, geciken işler ve yaklaşan etkinlikler.
- [ ] Yedekleme/dışa aktarma ve geri yükleme seçeneği.
- [ ] Erişilebilirlik, hata mesajları, boş durumlar ve iPhone ekran testi.
- [ ] README'de gerçek özellikleri, sınırlamaları ve kurulum adımlarını güncel tut.

## Ücretsiz barındırma ve gizlilik
GitHub Pages statik HTML/CSS/JavaScript yayınlar; sunucu tarafında Python/PHP çalıştırmaz. GitHub Pages'te yayınlanan sayfa herkese açık kabul edilmelidir. Bu nedenle kişisel mesajlar, takvim kayıtları, parolalar veya gizli API anahtarları depoya eklenmez. Mevcut görev kayıtları yalnızca o tarayıcının yerel depolamasındadır; tarayıcı verileri silinirse kaybolabilir ve başka cihazlarla otomatik eşitlenmez.

## Bir sonraki somut iş
Aşama 1'in ilk parçası: görevlere son tarih ve öncelik alanlarını eklemek; eski görevleri korumak ve iPhone'da test etmek.
