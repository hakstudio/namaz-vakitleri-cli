# Namaz Vakitleri CLI

Diyanet İşleri Başkanlığı verilerini kullanarak terminal üzerinden namaz vakitlerini görüntüleyen bir araçtır.

## Kurulum

Program zaten sisteminizde kurulu durumdadır. Terminalde `namaz-vakitleri` yazarak çalıştırabilirsiniz.

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

Programı ve tüm yapılandırma dosyalarını sisteminizden tamamen kaldırmak için şu komutu çalıştırın:

```bash
rm -rf ~/.config/namaz-vakitleri ~/bin/namaz-vakitleri /Users/hak/Projects/Others/namaz-vakitleri
```

