---
title: Yakıt Defteri — Gizlilik Politikası
---

# Yakıt Defteri — Gizlilik Politikası

Son güncelleme: 28 Eylül 2026

Yakıt Defteri, araç yakıt ve gider kayıtlarını tutan bir Android uygulamasıdır. Hesap açmanız
gerekmez. Reklam ve analiz aracı içermez.

## Hangi veriler, nerede

- **Kayıtlarınız** (araç, yakıt alımı, gider, hatırlatma, ayarlar) yalnızca telefonunuzda,
  uygulamanın kendi veritabanında saklanır. Bize veya başka bir sunucuya gönderilmez.
- **Otomatik yedek:** Uygulama, kayıtlarınızın bir kopyasını telefonunuzdaki
  `İndirilenler/YakitDefteri` klasörüne JSON dosyası olarak yazar ve son 5 kopyayı tutar.
  Bu klasör telefonunuzda kalır; dosya yöneticisi gibi depolama izni olan uygulamalar görebilir.
- **Elle yedek ve dışa aktarma:** "Yedek al", "CSV dışa aktar" ve "PDF rapor" dosyaları sizin
  seçtiğiniz yere kaydedilir.
- **Android yedeği:** Telefonunuzda Google yedeklemesi açıksa Android, uygulamanın veritabanını ve
  ayarlarını kendi Google hesabınıza yedekler. Bu yedek Google'ın hizmetidir; biz erişemeyiz.

## Kamera ve fotoğraflar

Fiş fotoğrafı çektiğinizde veya galeriden seçtiğinizde metin, Google ML Kit ile **telefonun
üzerinde** okunur. Fotoğraf ve fiş metni sunucuya gönderilmez. Çekilen fotoğraf uygulamanın geçici
klasöründe durur ve Android tarafından temizlenebilir.

## İnternet bağlantısı

Uygulama internete iki durumda çıkar:

1. **Marka logoları:** Araç markanızın logosu `cdn.simpleicons.org` adresinden indirilir. Bu istekte
   marka adı ve cihazınızın IP adresi o hizmete iletilir.
2. **Google ML Kit:** Fiş okuma kütüphanesi, çalışmasını izlemek için Google'a anonim tanılama ve
   kullanım verisi (ör. cihaz modeli, performans ölçümleri) gönderebilir. Fiş içeriğini göndermez.
   Ayrıntı: https://developers.google.com/ml-kit/terms

## Bildirimler

Hatırlatmalarınız (bakım, muayene, sigorta vb.) için telefonunuzda bildirim gösterilir. Bildirimler
telefonda oluşturulur; dışarıya veri gönderilmez.

## Veri silme

Bir aracı sildiğinizde ona ait tüm kayıtlar silinir. Uygulamayı kaldırdığınızda uygulama verileri
silinir; `İndirilenler/YakitDefteri` klasöründeki yedek dosyaları siz silene kadar kalır.

## Çocuklar

Uygulama 13 yaşın altındaki çocuklara yönelik değildir ve bilerek onlardan veri toplamaz.

## İletişim

Sorularınız için: yilmazhicabi@gmail.com

---

# Yakıt Defteri — Privacy Policy

Last updated: 28 September 2026

Yakıt Defteri is an Android app for logging a car's fuel and running costs. It needs no account and
contains no ads or analytics tools.

## What data, where

- **Your records** (vehicles, fill-ups, expenses, reminders, settings) are stored only on your phone,
  in the app's own database. They are not sent to us or to any other server.
- **Automatic backup:** the app writes a copy of your records as a JSON file to the
  `Downloads/YakitDefteri` folder on your phone and keeps the last 5 copies. The folder stays on your
  phone; apps with storage access, such as file managers, can see it.
- **Manual backup and export:** "Yedek al", "CSV dışa aktar" and "PDF rapor" files are saved where
  you choose.
- **Android backup:** if Google backup is on, Android backs up the app's database and settings to
  your own Google account. That backup is a Google service; we cannot access it.

## Camera and photos

When you take or pick a receipt photo, its text is read **on the phone** with Google ML Kit. Neither
the photo nor the receipt text is sent to a server. A photo you take stays in the app's temporary
folder, which Android may clear.

## Internet access

The app goes online in two cases:

1. **Brand logos:** your car brand's logo is downloaded from `cdn.simpleicons.org`. That request
   passes the brand name and your device's IP address to that service.
2. **Google ML Kit:** the receipt-reading library may send anonymous diagnostic and usage data to
   Google (for example device model and performance metrics). It does not send receipt contents.
   Details: https://developers.google.com/ml-kit/terms

## Notifications

Reminders (service, inspection, insurance, etc.) are shown as notifications created on the phone.
No data leaves the phone for them.

## Deleting data

Deleting a vehicle deletes all of its records. Uninstalling the app deletes its data; backup files in
`Downloads/YakitDefteri` remain until you delete them.

## Children

The app is not directed at children under 13 and does not knowingly collect data from them.

## Contact

Questions: yilmazhicabi@gmail.com
