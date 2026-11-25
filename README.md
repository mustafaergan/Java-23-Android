# Android Ders Örnekleri (2017 sonbahar)

Android derslerinde yazılan küçük uygulamalar: yaşam döngüsü, ekranlar arası geçiş, `WebView`, konum,
Google Haritalar ve SQLite. Her klasör Android Studio ile ayrı açılan bağımsız bir Gradle projesidir.

> **Not:** Bu depo 2017 yılında eğitim amaçlı yazıldı ve artık güncellenmiyor. Android Gradle eklentisi,
> Support Library, Play Services ve SDK sürümleri çok eskidir, bilinen güvenlik açıkları içerebilir;
> üretimde kullanmayın.

## İçerik

| Klasör | Ne yapar |
|---|---|
| `Hello` | Boş ekran; activity yaşam döngüsü metotlarını (`onResume`, `onDestroy` vb.) gösterir |
| `Hello2` | Girilen isme rastgele bir öneri ekleyip `Toast` ile gösterir |
| `Layout` | Giriş ekranı tasarımı; doğru bilgiyle ikinci ekrana geçer |
| `Kiprasim` | Açılınca telefonu birkaç saniye titreştirir (`Vibrator`) |
| `WebView` | Bir web sitesini uygulama içinde `WebView` ile açar |
| `Instagram` | `WebView` içinde Instagram'ı açar, yazılan kullanıcı adının sayfasına gider |
| `LokantaBul` | Konum izni ister, konumu alınca Google Haritalar'da yakındaki otelleri arar |
| `MyApplication` | Android Studio'nun Google Maps şablonu; haritaya işaret koyar |
| `Otopark` | SQLite ile araç ekleme, listeleme ve silme; menü ve birden çok ekran |

## Teknolojiler

- Java, Android SDK 26 (`minSdkVersion` 15–17)
- Android Gradle eklentisi 2.3.3, Gradle 3.3 (wrapper)
- `com.android.support:appcompat-v7:26.+`, ConstraintLayout 1.0.2
- Google Play Services Maps 11.0.4 (`MyApplication`)

## Çalıştırma

1. İstediğiniz klasörü (örneğin `Otopark`) Android Studio'da **Open** ile açın.
2. Bu sürümler güncel Android Studio ile doğrudan açılmaz; Android Studio'nun önerdiği Gradle ve eklenti
   yükseltmesini yapmanız ya da Support Library yerine AndroidX'e geçmeniz gerekir.
3. Emülatörde ya da cihazda çalıştırın.

Notlar:

- `MyApplication` için kendi Google Maps API anahtarınızı almanız ve
  `app/src/debug/res/values/google_maps_api.xml` (yayın sürümü için `src/release/...`) içindeki
  `YOUR_KEY_HERE` yerine yazmanız gerekir. Anahtarı depoya göndermeyin.
- `Layout` örneğindeki kullanıcı adı ve şifre, ders için kodun içine sabit yazılmıştır.
