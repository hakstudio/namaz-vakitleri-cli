# Namaz Vakitleri CLI

Diyanet İşleri Başkanlığı verilerini kullanarak terminal üzerinden namaz vakitlerini görüntüleyen bir araçtır.

## Kurulum

Sisteminizde `python3` ve `pip` kurulu olduğundan emin olun.

1. Projeyi bilgisayarınıza indirin:
   ```bash
   git clone https://github.com/hak/namaz-vakitleri.git
   cd namaz-vakitleri
   ```

2. Gerekli kütüphaneleri yükleyin:
   ```bash
   pip install requests
   ```

3. Dosyaya çalıştırma izni verin:
   ```bash
   chmod +x namaz-vakitleri
   ```

4. (Opsiyonel) Programı sistem genelinde kullanmak için bir sembolik bağlantı oluşturun:
   ```bash
   # ~/bin dizini mevcutsa ve PATH'inizdeyse:
   ln -s "$(pwd)/namaz-vakitleri" ~/bin/namaz-vakitleri

   # Veya /usr/local/bin (sudo yetkisi gerektirebilir):
   sudo ln -s "$(pwd)/namaz-vakitleri" /usr/local/bin/namaz-vakitleri
   ```

## Kullanım

### 1. Yeni Konum Ayarlama
Ülke, eyalet (veya il) ve şehir (veya ilçe) bilgilerini girerek o yerin vakitlerini görebilir ve kaydedebilirsiniz:

```bash
namaz-vakitleri türkiye osmaniye bahçe
# veya
namaz-vakitleri almanya rheinland-pfalz nassau
```

### 2. Kayıtlı Konumu Görüntüleme
Bir kez konum girdikten sonra, sadece şu komutu yazmanız yeterlidir:

```bash
namaz-vakitleri
```
Program en son kaydettiğiniz konumu hatırlar.

## Kaldırma (Uninstall)

Programı ve tüm yapılandırma dosyalarını sisteminizden tamamen kaldırmak için şu adımları izleyin:

1. **Sembolik Bağlantıyı Kaldırın:**
   ```bash
   # ~/bin dizinine kurduysanız:
   rm ~/bin/namaz-vakitleri

   # Veya /usr/local/bin dizinine kurduysanız:
   sudo rm /usr/local/bin/namaz-vakitleri
   ```

2. **Yapılandırma Dosyalarını Silin:**
   ```bash
   rm -rf ~/.config/namaz-vakitleri
   ```

3. **Proje Klasörünü Silin:**
   ```bash
   # Projeyi indirdiğiniz dizine giderek klasörü silebilirsiniz.
   rm -rf "$(pwd)"
   ```

## Teşekkür ve Lisans

- Bu proje GPL-2.0 lisansı ile korunmaktadır.
- Yerel veritabanı (`yerler.json`), [erdemarslan/namazvakti](https://github.com/erdemarslan/namazvakti) projesinden temin edilmiştir. Katkıları için teşekkür ederiz.

