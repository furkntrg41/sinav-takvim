# Sınav Takvim

Üniversite sınav takvimi ve derslik oturma planı oluşturan masaüstü uygulaması.

## Özellikler

- Excel'den öğrenci, ders ve derslik verilerini otomatik içe aktarma
- Çakışma kontrolü ve kapasite yönetimi ile otomatik takvim üretimi
- Sınav oturma düzeni oluşturma
- PDF ve Excel çıktısı

## Teknolojiler

- **Python + PyQt6** — masaüstü arayüz
- **openpyxl** — Excel okuma/yazma
- **reportlab** — PDF çıktısı
- **argon2-cffi** — şifre hashleme

## Kurulum

```bash
pip install -r requirements.txt
python src/app.py
```

## Proje Yapısı

```
src/
├── app.py          # Giriş noktası
├── config.py       # Uygulama ayarları
├── core/           # İş mantığı (takvim, oturma planı)
├── ui/             # PyQt6 arayüz bileşenleri
└── utils/          # Yardımcı araçlar ve logger
```
