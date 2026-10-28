---
title: Yakıt Defteri — Gizlilik Politikası
---

# Yakıt Defteri — Gizlilik Politikası

Son güncelleme: 28 Ekim 2026

Yakıt Defteri, araç yakıt ve gider kayıtlarını tutan bir Android uygulamasıdır. Hesap açmanız
gerekmez. Reklam içermez. Kendi analiz aracımız yoktur; fiş okuma için kullanılan Google ML Kit'in
gönderebildiği tanılama verisi aşağıda "İnternet bağlantısı" bölümünde anlatılır.

## Hangi veriler, nerede

- **Kayıtlarınız** (araç, yakıt alımı, gider, hatırlatma, ayarlar) yalnızca telefonunuzda,
  uygulamanın kendi veritabanında saklanır. Bize veya başka bir sunucuya gönderilmez.
- **Otomatik yedek:** Uygulama, kayıtlarınızın bir kopyasını JSON dosyası olarak yazar ve son 5
  kopyayı tutar. Android 10 ve üstünde varsayılan yer `İndirilenler/YakitDefteri` klasörüdür;
  Ayarlar'dan başka bir klasör seçebilir veya otomatik yedeği kapatabilirsiniz. Android 9 ve altında
  dosyalar uygulamanın kendi klasörüne (`Android/data/com.yakitdefteri.app/files/backups`) yazılır.
  Dosyalar telefonunuzda kalır; dosya yöneticisi gibi depolama izni olan uygulamalar görebilir.
- **Elle yedek ve dışa aktarma:** "Yedek al", "CSV dışa aktar" ve "PDF rapor" dosyaları sizin
  seçtiğiniz yere kaydedilir.
- **Android yedeği:** Telefonunuzda Google yedeklemesi açıksa Android, uygulamanın veritabanını ve
  ayarlarını kendi Google hesabınıza yedekler. Bu yedek Google'ın hizmetidir; biz erişemeyiz.

## Kamera ve fotoğraflar

Fiş fotoğrafı çektiğinizde veya galeriden seçtiğinizde metin, Google ML Kit ile **telefonun
üzerinde** okunur. Fotoğraf ve fiş metni sunucuya gönderilmez. Çekilen fotoğraf uygulamanın geçici
klasöründe durur ve Android tarafından temizlenebilir.

## İnternet bağlantısı

Uygulama internete şu durumlarda çıkar:

1. **Marka logoları:** Araç markanızın logosu `cdn.simpleicons.org` adresinden indirilir. Bu istekte
   marka adı ve cihazınızın IP adresi o hizmete iletilir.
2. **Google ML Kit:** Fiş okuma kütüphanesi, çalışmasını izlemek için Google'a anonim tanılama ve
   kullanım verisi (ör. cihaz modeli, performans ölçümleri) gönderebilir. Fiş içeriğini göndermez.
   Ayrıntı: https://developers.google.com/ml-kit/terms
3. **"Verilerine sor" modeli (deneysel, isteğe bağlı):** Bu özelliği açıp modeli indirirseniz model
   dosyası (yaklaşık 300 MB) Google Play üzerinden indirilir; bu indirme Google Play'in kendi
   koşullarına tabidir. Sorularınız ve cevaplar **telefonun üzerinde** işlenir, hiçbir yere
   gönderilmez. Model Google'ın Gemma modeline dayanır ve Gemma Kullanım Şartları'na tabidir.
4. **Değerlendirme penceresi:** Uygulamada 5. yakıt kaydını girdikten sonra Google Play'in puan verme
   penceresi bir kez açılabilir. Puan ve yorum doğrudan Google Play'e gider; uygulama bunları görmez.

## Bildirimler

Hatırlatmalarınız (bakım, muayene, sigorta vb.) için telefonunuzda bildirim gösterilir. Bildirimler
telefonda oluşturulur; dışarıya veri gönderilmez.

## Veri silme

Bir aracı sildiğinizde ona ait tüm kayıtlar silinir. Uygulamayı kaldırdığınızda uygulama verileri
silinir. Android 10 ve üstünde `İndirilenler/YakitDefteri` (veya seçtiğiniz klasördeki) yedek dosyaları
siz silene kadar kalır; Android 9 ve altında uygulamanın kendi klasöründeki yedekler uygulamayla
birlikte silinir. Otomatik yedeği kapatmak eski dosyaları silmez.

## Çocuklar

Uygulama 13 yaşın altındaki çocuklara yönelik değildir ve bilerek onlardan veri toplamaz.

## İletişim

Sorularınız için: yilmazhicabi@gmail.com

---

# Yakıt Defteri — Privacy Policy

Last updated: 28 October 2026

Yakıt Defteri is an Android app for logging a car's fuel and running costs. It needs no account and
contains no ads. It has no analytics of its own; the diagnostic data that Google ML Kit (used for
reading receipts) may send is described under "Internet access".

## What data, where

- **Your records** (vehicles, fill-ups, expenses, reminders, settings) are stored only on your phone,
  in the app's own database. They are not sent to us or to any other server.
- **Automatic backup:** the app writes a copy of your records as a JSON file and keeps the last 5
  copies. On Android 10 and later the default place is the `Downloads/YakitDefteri` folder; in
  Settings you can choose another folder or turn the automatic backup off. On Android 9 and earlier the
  files go to the app's own folder (`Android/data/com.yakitdefteri.app/files/backups`). The files stay
  on your phone; apps with storage access, such as file managers, can see them.
- **Manual backup and export:** "Yedek al", "CSV dışa aktar" and "PDF rapor" files are saved where
  you choose.
- **Android backup:** if Google backup is on, Android backs up the app's database and settings to
  your own Google account. That backup is a Google service; we cannot access it.

## Camera and photos

When you take or pick a receipt photo, its text is read **on the phone** with Google ML Kit. Neither
the photo nor the receipt text is sent to a server. A photo you take stays in the app's temporary
folder, which Android may clear.

## Internet access

The app goes online in these cases:

1. **Brand logos:** your car brand's logo is downloaded from `cdn.simpleicons.org`. That request
   passes the brand name and your device's IP address to that service.
2. **Google ML Kit:** the receipt-reading library may send anonymous diagnostic and usage data to
   Google (for example device model and performance metrics). It does not send receipt contents.
   Details: https://developers.google.com/ml-kit/terms
3. **"Ask your data" model (experimental, optional):** if you turn this feature on and download the
   model, the model file (about 300 MB) comes from Google Play; that download is covered by Google
   Play's own terms. Your questions and the answers are processed **on the phone** and are not sent
   anywhere. The model is based on Google's Gemma and is subject to the Gemma Terms of Use.
4. **Rating prompt:** after you enter your 5th fill-up, Google Play's rating sheet may open once. A
   rating or review goes straight to Google Play; the app does not see it.

## Notifications

Reminders (service, inspection, insurance, etc.) are shown as notifications created on the phone.
No data leaves the phone for them.

## Deleting data

Deleting a vehicle deletes all of its records. Uninstalling the app deletes its data. On Android 10 and
later, backup files in `Downloads/YakitDefteri` (or the folder you chose) remain until you delete them;
on Android 9 and earlier, backups in the app's own folder are deleted with the app. Turning the automatic
backup off does not delete old files.

## Children

The app is not directed at children under 13 and does not knowingly collect data from them.

## Contact

Questions: yilmazhicabi@gmail.com
