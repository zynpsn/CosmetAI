# CosmetAI 🐱💄

**Aradığın kozmetik ürün, yakınındaki hangi mağazada var?**

CosmetAI; Gratis, Watsons, Rossmann, Sephora, Eve ve markaların kendi mağazalarında (Flormar, Golden Rose, KIKO Milano) bir kozmetik ürünün (marka, ürün ve ton) nerede bulunabileceğini kullanıcının konumuna göre gösteren bir web uygulaması prototipidir. Türkiye'nin 81 ilini kapsar.

🔗 **Canlı site:** https://zynpsn.github.io/CosmetAI/

---

## Neden?

Bir ürünü sosyal medyada görüp denemek istediğimizde çoğu zaman mağaza mağaza dolaşmak zorunda kalıyoruz. Zincirlerin çoğunda "hangi mağazada stokta var?" araması yok. CosmetAI bu sorunu tek bir aramayla çözmeyi hedefler.

## Özellikler

- 🔎 **Ürün arama:** 400'ü aşkın marka; ruj, fondöten, kapatıcı gibi ürünlerde gerçek ton adları ve numaraları (ör. *Maybelline Lifter Gloss 002 Ice*, *Pastel Daylong Kissproof 15 Marina*). Ürün adını ve türünü yazınca (ör. *note mattemoist ruj*) tonlar numara sırasıyla önerilir; Türkçe ve İngilizce kelimeler birlikte çalışır (*ruj* yazınca *Lipstick* de bulunur)
- 🧾 **Sadece gerçek ürünler:** Listede yalnızca gerçek ürün adları vardır; "Marka + Ruj" gibi otomatik oluşturulmuş genel ürünler kullanılmaz
- 📍 **Konuma göre mağaza bulma:** Tarayıcı konumu ya da il seçimi ile en yakın mağazalar
- 🗺️ **Harita:** Mağazalar harita üzerinde işaretlenir, her mağaza için yol tarifi bağlantısı
- 🏷️ **Mağaza–marka eşleştirmesi:** Her marka yalnızca satıldığı zincirlerde gösterilir. Bu eşleştirme zincirlerin kendi sitelerinde (gratis.com, watsons.com.tr, rossmann.com.tr, eveshop.com.tr) tek tek kontrol edilerek yapılmıştır (ör. *Sheglam* yalnızca Gratis'te, *NYX* yalnızca Watsons'ta, *KIKO Milano* yalnızca kendi mağazalarında). Bu zincirlerin hiçbirinde satılmayan markalar için mağaza gösterilmez
- 🏬 **Marka mağazaları:** Flormar, Golden Rose (Golden Shop) ve KIKO Milano mağazaları da haritada aranır
- ➕ **Ürün ekleme:** Listede olmayan ürünler tek tek veya toplu olarak eklenebilir
- 🌙 **Açık / koyu tema** ve 🌐 **Türkçe / English** dil desteği
- 📱 Telefon ve bilgisayarda çalışan duyarlı (responsive) tasarım

## Kullanılan teknolojiler ve veri kaynakları

| Ne için | Kaynak |
|---|---|
| Arayüz | HTML, CSS, JavaScript (tek dosya, kurulum gerektirmez) |
| Harita | [Leaflet](https://leafletjs.com/), yedek olarak Google Haritalar |
| Mağaza konumları | [OpenStreetMap](https://www.openstreetmap.org/) (Overpass API, Nominatim) ve [TomTom Search API](https://developer.tomtom.com/) |
| Ürün önerileri | [Open Beauty Facts](https://world.openbeautyfacts.org/) (CC BY-SA) |
| Yayın | GitHub Pages |

## Sınırlamalar

- **Stok adetleri örnek (simüle) veridir.** Kozmetik zincirleri mağaza bazlı stok bilgisini herkese açık olarak paylaşmamaktadır. Uygulama, gerçek stok verisi bağlanabilecek şekilde tasarlanmıştır; gerçek kullanımda bu veri zincirlerle resmi iş birliği veya kullanıcı bildirimleriyle sağlanabilir.
- **Mağaza konumları** açık harita verilerinden gelir; bazı mağazalar eksik veya güncel olmayabilir.
- **Ton listeleri** Türk ve yabancı satıcı sayfalarından derlenmiştir; her tonun Türkiye'de satışta olduğu ayrıca doğrulanmamıştır.
- **Marka–zincir eşleştirmesi** marka düzeyindedir: bir markanın o zincirde satıldığı doğrulanmıştır, ancak her ürünün her mağazada bulunduğu anlamına gelmez. Eczane ve marketler kapsam dışıdır.

## Gizlilik

Konum yalnızca yakındaki mağazaları bulmak için harita servislerine sorgu olarak gönderilir; site konumu kaydetmez veya saklamaz. Kullanıcının eklediği ürünler yalnızca kendi tarayıcısında tutulur.

## Nasıl kullanılır?

1. Arama kutusuna ürünü yaz (ör. *maybelline fit me 120*).
2. **Konumumu kullan**'a bas ya da ilini seç.
3. Listeden ürünü seç; yakındaki mağazalar ve stok durumu harita ile birlikte görünür.

---

*Bu proje bir üniversite dersi kapsamında hazırlanmıştır.*
