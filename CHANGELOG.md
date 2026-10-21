---
layout: default
---

# Porsuk değişiklik geçmişi / Change history

Bu notlar yerel geliştirme kayıtlarını ve paketlenmiş veriyi özetler; App Store yayın tarihlerini belirlemez. / These notes summarize local development records and the bundled data. They do not establish public App Store release dates.

## 1.1.0 (9)

Veri sürümü / dataset: 2026.10.21.1 · 179.736 / 179,736 kamp alanı / campsites · Türkiye / Türkiye 1.804

### Türkçe

Yeni:

- **Planla sekmesi** (Keşfet, Planla, Favoriler, Ayarlar): *Yol Üstü Kamp* (durakları yaz; rota Apple Haritalar ile hesaplanır; yol üstündeki kamp alanları şerit genişliğine ve türe göre listelenir ve haritada gösterilir; internet yoksa rota düz hat tahminidir; GPX içe aktarma, kayıtlı rotalar), *Bu Gece Nerede?* (En yakın / En konforlu / Ücretsiz-doğada önerileri, yolculuk süresi, gün batımı, "en geç şu saatte çık" önerisi, sezon dışı uyarısı; müsaitlik bilinmediği her kartta yazar) ve *Saha Modu* (internetsiz radar ile koordinat, DMS, Plus Code, yükseklik, konum yaşı, acil durum araması ve konum paylaşımı içeren güvenlik kartı).
- **Kamp Profilim** (araç, yol arkadaşları, ihtiyaçlar), Keşfet'te "Profilime göre", kayıtlı filtreler ve "Konumuma" mesafe seçenekleri. Profil yalnızca türe ve açık olumsuzlara (ör. köpek kabul edilmiyor) göre eler; olanaklar sıralamayı etkiler ya da rozet olarak görünür.
- **Kamp hava durumu asistanı:** 14 günlük tahmin (ilk 7 gün öne çıkar, sonrası düşük güvenilirlik), rüzgâr / don / sıcak / yağış / UV uyarıları (bilgilendirme amaçlı), ay evresine göre yıldız gecesi ipucu, yükselti. Hava durumu verisi Open-Meteo'dan gelir.
- **Favoriler 2.0:** harita görünümü, listeler ("Gitmek istediklerim", "Gittiklerim", en fazla 20 özel liste), "Gittim" işareti, 3 kampa kadar karşılaştırma, listeyi bağlantı / metin / GPX olarak paylaşma, bağlantıdan önizlemeli içe aktarma (dokunmadan hiçbir şey içe aktarılmaz).
- **Çevrede:** kamp alanı sayfasında, Apple Haritalar ile çevredeki market, yakıt, eczane, hastane, çamaşırhane, ATM, şarj istasyonu ve restoran (yalnızca kamp alanının koordinatı gönderilir).
- **Dışa aktarma ve harita uygulamaları:** kamp alanını GPX / KML olarak paylaşma; "Yol tarifi" menüsünde Apple Haritalar ve kuruluysa Waze, Organic Maps / OsmAnd (çevrimdışı).
- **Eksik kamp alanı ekle:** Ayarlar'da ve kamp alanı menüsünde üç adımlık rehber (OpenStreetMap'e ekleme).
- **Katalog:** 179.736 kamp alanı (veri sürümü 2026.10.21.1), Türkiye'de yaklaşık 1.800 (1.804). Veritabanı ODbL 1.0 altında açık veri olarak [son sürümde](https://github.com/emircanby/porsuk-support/releases/latest) yayımlanır.

Değişen:

- Gizlilik metni yeni özellikleri doğru anlatır: Apple Haritalar'a gidenler, Open-Meteo'ya gidenler, OpenStreetMap düzenleyici bağlantısındaki yaklaşık konum, cihazda kalanlar ve "Hesabı sil" ile silinenler. Geliştirici hiçbir veri toplamaz.
- Ayarlar > Veri kaynakları ve lisanslar: Apple Haritalar hizmetleri ve Open-Meteo, kamp alanı kaynaklarından ayrı bir "Çevrimiçi hizmetler" bölümünde.
- Mesafeler bölgene göre km ya da mil gösterilir; mil kullanan bölgelerde "Konumuma" seçenekleri 15/30/60/150 mil olur ve daire gerçekten o kadar geniştir.
- Çevrimdışı uyarısı Planla'da neyin çalıştığını söyler (rota düz hat tahmini, Bu Gece ve Saha Modu çalışır).
- "Hesabı sil" artık profili, kayıtlı rotaları, listeleri ve kayıtlı filtreleri de siler.
- Bölge aramaları: Akdeniz, Ege, Marmara, Karadeniz (Batı ve Doğu Karadeniz dahil), İç / Doğu / Güneydoğu Anadolu ve Trakya (ve İngilizce adları) artık bir daireyle değil, bölgenin illeriyle aranır; komşu bölgelerin kamp alanları listeye girmez. Yedi bölge 81 ili paylaşır, her Türkiye kampı tam bir bölgededir.
- Katalog verisi, üç temizlik: kamp alanı olmayan noktalar artık listelenmez: yerinden edilmiş kişilerin çadırları ve mülteci kampları, BM görev noktaları, adı üs / kışla / karakol / ordu kampı olan noktalar, işçi ve şirket kampları, hac çadır parselleri (231 kayıt); konaklama yeri olmayan işletmeler: karavan satıcıları, kiralama firmaları, depolama sahaları, tamir atölyeleri, kamp malzemesi mağazaları ve yalnızca boşaltma istasyonu olan noktalar (190 kayıt kaldırıldı); işleten kuruluşu bir yardım kuruluşu olan 3 nokta. Kurallar adlara bakar, bu yüzden adı belli etmeyen bir nokta yine de listelenmiş olabilir. Çalışmayan web siteleri artık gösterilmez (145 kayıt web sitesini kaybetti, 134'ü Türkiye'de; yanıt veren siteler kalır) ve Dikili'de aynı kampın iki kaydı birleştirildi (Türkiye 1.805'ten 1.804'e).

Düzeltilen (1.1.0 geliştirilirken bulundu; hiçbiri yayımlanmış bir sürümde yoktu): "Rotaya ekle" açık bir rota ekranında görünmüyordu; Bu Gece Nerede?'de aynı kampın iki kartı kalabiliyordu; favoriden çıkarılan kamp listelerde kalabiliyordu; Saha Modu radarı çökebiliyordu; okunamayan liste, profil ya da kayıtlı filtre dosyası sessizce boş başlıyordu (artık uyarı çıkar).

Doğrulanmadı / bilinen sınırlar: müsaitlik, fiyat ya da "doğrulanmış" iddiası yoktur; bilinmeyen bilgi "yok" olarak gösterilmez. Hafta sonu kaçamağı, akıllı arama, widget ve bildirimler bu sürümde yoktur.

### English

New:

- **Plan tab** (Discover, Plan, Favorites, Settings): *Camps Along Your Route* (enter stops; Apple Maps calculates the route; campsites along it are listed by corridor width and kind and shown on the map; offline the route is a straight-line estimate; GPX import, saved routes), *Where Tonight?* (Nearest / Most comfortable / Free-nature picks, travel time, sunset, a "leave by" hint and an off-season notice; every card says availability is unknown) and *Field Mode* (an offline radar and a safety card with coordinates, DMS, Plus Code, altitude, fix age, emergency call and position sharing).
- **My camping profile** (vehicle, companions, needs), "Match my profile" in Discover, saved filters and "Near me" distance options. A profile only filters by kind and explicit negatives (for example dogs not allowed); amenities influence ranking or appear as badges.
- **Camp weather assistant:** a 14-day forecast (the first 7 days are prominent, later days are marked low confidence), wind / frost / heat / rain / UV advisories (information only), a stargazing hint from the moon phase, elevation. Weather data comes from Open-Meteo.
- **Favorites 2.0:** a map view, lists ("Want to go", "Been there" and up to 20 custom lists), a "been there" mark, comparing up to 3 campsites, sharing a list as a link / text / GPX, and importing from a link with a preview (nothing is imported without a tap).
- **Around here:** on a campsite page, shops, fuel, pharmacies, hospitals, laundries, ATMs, charging stations and restaurants around it from Apple Maps (only the campsite's coordinates are sent).
- **Export and maps apps:** share a campsite as GPX / KML; the "Directions" menu lists Apple Maps and, when installed, Waze and Organic Maps / OsmAnd (offline).
- **Add a missing campsite:** a three-step guide in Settings and in the campsite menu (adding to OpenStreetMap).
- **Catalog:** 179,736 campsites (dataset 2026.10.21.1), about 1,800 (1,804) in Türkiye. The database is published as open data under ODbL 1.0 on the [latest release](https://github.com/emircanby/porsuk-support/releases/latest).

Changed:

- The privacy text describes the new features accurately: what goes to Apple Maps, what goes to Open-Meteo, the approximate position in the OpenStreetMap editor link, what stays on the device and what "Delete account" erases. The developer collects no data.
- Settings > Data sources & licenses: Apple Maps services and Open-Meteo are in an "Online services" section, apart from the campsite data sources.
- Distances follow your region, km or miles; in regions that use miles the "Near me" options are 15/30/60/150 mi and the circle really is that wide.
- The offline notice in Plan says what still works (routes as a straight-line estimate, Tonight and Field Mode).
- "Delete account" now also erases the profile, saved routes, lists and saved filters.
- Region searches: Akdeniz, Ege, Marmara, Karadeniz (including Western and Eastern Black Sea), İç / Doğu / Güneydoğu Anadolu and Trakya (and their English names) are now searched by the provinces of the region, not by a circle; campsites of neighbouring regions no longer appear. The seven regions share the 81 provinces, so every campsite in Türkiye is in exactly one region.
- Catalog data, three cleanups: points that are not campsites are no longer listed: tents of displaced people and refugee camps, United Nations mission sites, points whose name is a base / barracks / checkpoint / army camp, workers' and company camps, Hajj tent plots (231 records); businesses that are not a place to stay: caravan dealers, rental firms, storage yards, workshops, camping-goods shops and dump-station-only points (190 records removed); and 3 points run by a humanitarian agency. The rules go by names, so a point whose name does not give it away can still be listed. Websites that no longer work are no longer shown (145 records lost a website, 134 of them in Türkiye; sites that respond stay), and two records of one campground in Dikili were merged (Türkiye 1,805 to 1,804).

Fixed (found while developing 1.1.0; none was in a published release): "Add to route" did not show up in an open route screen; Where Tonight? could keep two cards for the same campsite; a campsite un-favorited elsewhere could stay in lists; the Field Mode radar could crash; an unreadable lists, profile or saved-filters file silently started empty (a notice appears now).

Not verified / known limits: there is no availability, price or "verified" claim; unknown information is never shown as "no". Weekend escape, smart search, widgets and notifications are not in this release.

## 1.0.2 (7)

- Bundled catalog: 25,037 campsites. / Paketlenmiş katalog: 25.037 kamp alanı.
- Preview-first startup and location-specific data loading. / Önizleme katalogla hızlı açılış ve konuma özel veri yükleme.
- Prepared search documents and grid-based map indexing. / Hazırlanmış arama dizinleri ve ızgara tabanlı harita dizini.
- City/region search separated from broad country fallbacks. / Şehir/bölge araması geniş ülke sonuçlarından ayrıldı.
- Campsite classification and fee display corrections. / Kamp alanı sınıflandırması ve ücret gösterimi düzeltmeleri.
- Turkish address corrections: Can Mocamp appears in Kaş, Antalya. / Türkçe adres düzeltmeleri: Can Mocamp Kaş, Antalya'da görünür.
- Shortcuts for search and Favorites. / Arama ve Favoriler için kestirmeler.
