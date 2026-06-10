<div align="center">

# Sınav Takvim

**Üniversite sınav programı ve derslik oturma planı oluşturucu**

[![Python](https://img.shields.io/badge/Python-3.10+-3776AB?style=flat-square&logo=python&logoColor=white)](https://python.org)
[![PyQt6](https://img.shields.io/badge/PyQt6-desktop%20app-41CD52?style=flat-square&logo=qt&logoColor=white)](https://www.riverbankcomputing.com/software/pyqt)
[![Platform](https://img.shields.io/badge/Platform-Windows%20%7C%20macOS%20%7C%20Linux-lightgrey?style=flat-square)](https://python.org)
[![License](https://img.shields.io/badge/License-MIT-22c55e?style=flat-square)](LICENSE)

</div>

---

## Ne Yapar?

Excel formatında gelen öğrenci, ders ve derslik listelerinden otomatik olarak:
- Çakışmasız sınav takvimi oluşturur
- Her sınav için oturma düzeni üretir
- PDF ve Excel formatında çıktı verir

---

## Özellikler

- **Excel import:** Öğrenci, ders ve derslik verilerini Excel'den otomatik okuma
- **Akıllı planlama:** Ders çakışması ve derslik kapasitesi kontrolü
- **Oturma düzeni:** Sınav başına otomatik koltuk planı
- **Çıktı:** PDF raporu (reportlab) ve Excel tablosu (openpyxl)
- **Güvenli giriş:** argon2 ile şifreli yönetici paneli
- **Masaüstü UI:** PyQt6 ile native görünümlü arayüz

---

## Kurulum

**Gereksinim:** Python 3.10+

```bash
# Repo'yu klonla
git clone https://github.com/furkntrg41/sinav-takvim.git
cd sinav-takvim

# Bağımlılıkları yükle
pip install -r requirements.txt

# Uygulamayı başlat
python src/app.py
```

### Windows (PowerShell)

```powershell
.\run.ps1
```

---

## Kullanım

1. Uygulamayı başlatın
2. **Excel import** ile öğrenci, ders ve derslik listelerini yükleyin
3. **Takvim Oluştur** butonuna tıklayın
4. Sonuçları PDF veya Excel olarak dışa aktarın

---

## Proje Yapısı

```
.
├── src/
│   ├── app.py          # Giriş noktası
│   ├── config.py       # Uygulama ayarları
│   ├── core/           # İş mantığı
│   │   ├── scheduler.py    # Takvim algoritması
│   │   └── seating.py      # Oturma düzeni oluşturucu
│   ├── ui/             # PyQt6 arayüz bileşenleri
│   └── utils/          # Logger ve yardımcılar
├── resources/          # İkonlar ve statik kaynaklar
├── requirements.txt
└── run.ps1             # Windows başlatma scripti
```

---

## Bağımlılıklar

| Paket | Versiyon | Kullanım |
|-------|----------|---------|
| PyQt6 | ≥6.6.1 | Masaüstü arayüz |
| openpyxl | 3.1.2 | Excel okuma/yazma |
| reportlab | 4.0.7 | PDF çıktısı |
| argon2-cffi | 23.1.0 | Şifre hashleme |
| python-dateutil | 2.8.2 | Tarih işleme |

---

## Lisans

[MIT](LICENSE) © 2026 furkntrg41
