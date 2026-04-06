# 📊 NumPy General Review: Employee Performance Analysis

Bu proje, Python'ın bilimsel hesaplama kütüphanesi **NumPy**'ın veri analizi süreçlerindeki gücünü ve esnekliğini göstermek amacıyla hazırlanmış bir "Genel İnceleme" çalışmasıdır. Proje, 8 çalışanın 6 aylık performans verilerini içeren bir matris yapısı üzerinden çeşitli senaryoları simüle eder.

---

## 🎯 Proje Amacı ve Kapsamı
Proje, ham bir veri setinden anlamlı istatistiksel çıkarımlar yapma sürecini kapsar. 8x6 boyutundaki bir matris (8 ay x 6 çalışan veya tam tersi kurgulanabilir) üzerinde veri temizleme, normalizasyon ve karşılaştırmalı analiz teknikleri uygulanmıştır.

---

## 🛠️ Teknik Özellikler ve Kazanımlar

Bu notebook içerisinde aşağıdaki NumPy yetenekleri aktif olarak kullanılmıştır:

* **Veri Üretimi:** `np.random.randint` ile belirlenen sınırlar dahilinde (50-100 arası) rastgele veri setleri oluşturma.
* **Matris Öznitelikleri:** `shape`, `ndim`, `dtype` ve `size` komutlarıyla veri yapısının teknik özelliklerini inceleme.
* **İstatistiksel Analizler:**
    * `sum()`, `max()`, `min()` ve `mean()` fonksiyonları ile genel performans raporlama.
    * **Eksen Bazlı Analiz:** `axis=1` ile aylık ortalamalar, `axis=0` ile çalışan bazlı ortalamalar elde etme.
    * `argmax()` ile en yüksek performansın hangi indekste olduğunu saptama.
* **Veri Normalizasyonu:** Veriyi standart bir ölçeğe (0-100) getirmek için matematiksel formülizasyon ve `round()` ile hassasiyet ayarı.
* **Matris Manipülasyonu:**
    * `reshape()`: Veri yapısını (6,8) şeklinde yeniden boyutlandırma.
    * `transpose()`: Satır ve sütunların yerini değiştirerek farklı perspektiflerden bakış.
    * `ravel()`: Çok boyutlu yapıyı tekil bir liste haline getirme.

---

## 📂 Proje Yapısı

* `performans`: 8x6 boyutundaki ana veri matrisi.
* `çalışanlar`: Çalışan isimlerini ve onlara ait performans sütunlarını tutan Python sözlüğü.
* `normalizasyon`: Formülize edilmiş ve standartlaştırılmış performans değerleri.

---

## 📈 Raporlama ve Sonuçlar
Program çalıştırıldığında aşağıdaki verileri otomatik olarak hesaplar:
- **En Başarılı Çalışan:** Ortalama puanı en yüksek olan personelin saptanması.
- **En Verimli Dönem:** Genel ortalamanın zirve yaptığı ayın bulunması.
- **Genel Performans Ortalama:** Tüm sistemin başarı yüzdesi.

---

## 🚀 Nasıl Çalıştırılır?

1. Gerekli kütüphaneyi yükleyin:
   ```bash
   pip install numpy
