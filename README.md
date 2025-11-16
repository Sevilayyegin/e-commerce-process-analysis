# **E-Ticaret Süreci Analizi – Portföy Projesi**

Bu proje, bir e-ticaret şirketinin satış verilerini analiz ederek müşteri davranışlarını, satın alma eğilimlerini ve iş performansını daha iyi anlamayı amaçlayan kapsamlı bir veri analizi çalışmasıdır. Proje, iş analitiği bakış açısıyla hazırlanmış olup; veri temizleme, keşifsel analiz, müşteri segmentasyonu, KPI değerlendirmesi ve iş tarafına yönelik içgörü üretme adımlarını içermektedir.

---

## **📌 Projenin Amacı**

* E-ticaret satış süreçlerini uçtan uca analiz etmek
* Veri odaklı iş kararlarına ışık tutacak metrikler ve içgörüler üretmek
* Müşteri davranışlarını anlamak (RFM segmentasyonu)
* İade, gelir, sipariş ve müşteri aktivitelerini görünür kılmak
* İş analisti rolünü destekleyecek şekilde rapor, yorum ve süreç iyileştirme önerileri sunmak

Bu proje, teknik analiz kadar **iş analisti perspektifi** de içermektedir: müşteri yolculuğu, operasyonel aksaklıklar, segment bazlı aksiyon önerileri ve KPI yorumları gibi.

---

## **📂 Proje Yapısı**

e-ticaret-sureci-analizi/
│
├─ notebooks/ # Analiz ve görselleştirme notebook’ları
│ ├─ 01_EDA.ipynb # Keşifsel Veri Analizi (EDA)
│ └─ 03_KPIs.ipynb # KPI hesaplamaları ve grafikler
│
├─ reports/ # Yorumlanmış raporlar
│ └─ kpi_summary.md
│
├─ outputs/ # Analiz çıktıları
│ └─ rfm_segments.csv # RFM segment sonuçları
│
├─ data/ # Kaynak veri
│ └─ online_retail.csv
│
└─ README.md # Proje açıklaması


---

## **📊 Kullanılan Veri Seti**

Bu projede kullanılan veri seti, bir e-ticaret şirketinin **2010–2011** dönemine ait gerçek satış hareketlerini içeren bir transaction datasıdır.

**Veri seti özellikleri:**

* Müşteri bazlı işlem kayıtları
* Fatura, stok kodu, ürün açıklaması
* Miktar ve birim fiyat
* Ülke bilgisi
* İade işlemleri (InvoiceNo “C” ile başlayan kayıtlar)

**Veri boyutu:**

* **Toplam işlem:** Yaklaşık ~500.000 kayıt
* **Zaman aralığı:** Aralık 2010 → Aralık 2011
* **Toplam gelir:** 9.7M+
* **İade sayısı:** ~9K

---

## **🧽 1. Veri Temizleme Adımları**

Proje boyunca aşağıdaki temizlik adımları uygulanmıştır:

* Eksik müşteri ID’lerinin kontrolü
* Negatif miktar / fiyat kontrolleri
* İade kayıtlarının “IsReturn” olarak işaretlenmesi
* Tarih formatlarının dönüştürülmesi
* Yanlış karakter içeren ürün açıklamalarının temizlenmesi
* Outlier tespiti (iş mantığına göre değerlendirilerek)

Bu adımların her biri hem doğruluk hem de KPI hesaplamalarının sağlıklı yapılması için gerçekleştirilmiştir.

---

## **🔍 2. Keşifsel Veri Analizi (EDA)**

Analiz edilen başlıca sorular:

### ✔ Satış hacmi zaman içinde nasıl değişiyor?

* Günlük / aylık sipariş trendleri
* Sezon etkileri

### ✔ En çok satan ve en çok gelir getiren ürünler hangileri?

* Pareto analizi (80/20)
* Kategori/ürün bazlı yoğunluk

### ✔ İade davranışı nasıl?

* En çok iade edilen ürünler
* Ülke bazlı iade farkları
* İadelerin toplam gelire etkisi

Bu adımda ayrıca veri setinin iş açısından anlamlandırılması için grafikler ve ilgili açıklamalar hazırlanmıştır.

---

## **📐 3. KPI Hesaplamaları**

Projede hesaplanan ana metrikler:

| KPI                               | Açıklama                                          |
| --------------------------------- | ------------------------------------------------- |
| **Toplam Gelir**                  | Tüm satışların toplam tutarı                      |
| **Net Gelir**                     | İadeler çıktıktan sonra kalan gelir               |
| **Ortalama Sipariş Değeri (AOV)** | Gelir / Sipariş sayısı                            |
| **Tekil Müşteri Sayısı**          | Aktif müşteri adedi                               |
| **Sipariş Frekansı**              | Müşteri başına yapılan ortalama sipariş adedi     |
| **İade Oranı**                    | İade edilen siparişlerin toplam siparişlere oranı |

Tüm KPI sonuçları, iş analisti bakışıyla yorumlanmış ve rapor dosyalarında detaylandırılmıştır.

---

## **🧩 4. Müşteri Segmentasyonu – RFM Analizi**

Müşteriler şu üç boyuta göre analiz edilmiştir:

* **Recency:** Son alışverişten geçtiği gün
* **Frequency:** Toplam sipariş sayısı
* **Monetary:** Toplam harcama miktarı

RFM skorlaması sonrası elde edilen segmentler:

* Champions
* Loyal Customers
* Potential Loyalist
* At Risk
* Lost
* Needs Attention

Bu segmentler iş birimlerine yönelik aksiyon önerileriyle birlikte raporlanmıştır.

---

## **💬 5. İş Çıkarımları & Öneriler**

Analiz boyunca ortaya çıkan başlıca iş içgörüleri:

* **Sadık müşteriler toplam gelirin önemli kısmını oluşturuyor.**
  → Bu segment için özel kampanyalar maliyeti doğrudan artırmadan geliri yükseltebilir.

* **İade yoğunluğu belirli ürünlerde toplanıyor.**
  → Ürün bilgisi, paketleme veya tedarikçi kaynaklı süreçler incelenmeli.

* **Tek seferlik alışveriş yapan müşteri oranı yüksek.**
  → E-mail otomasyonları veya onboarding kampanyalarıyla tekrar satın alma teşvik edilmeli.

* **Aylık satışlar belirgin dönemlerde zirve yapıyor.**
  → Stok planlaması, pazarlama bütçesi ve kampanya takvimi buna göre optimize edilebilir.

---

## **🧰 Kullanılan Araçlar**

Bu projede hem teknik hem iş analisti araçları birlikte kullanılmıştır:

### **Teknik**

* Python
* Pandas, NumPy
* Matplotlib, Seaborn
* Jupyter Notebook (Kaggle ortamı)

### **İş Analisti Yaklaşımı**

* KPI tanımlama & süreç analizi
* RFM ile müşteri segmentasyonu
* Problem–sebep analizleri
* Veri sonuçlarının iş birimlerine dönük yorumlanması

---

## **📎 Sonuç**

Bu proje, bir e-ticaret şirketinin satış verisini uçtan uca inceleyerek hem analitik hem iş analisti bakışıyla değerlendirilen profesyonel bir çalışmadır. İçerdiği adımlar; veri temizleme, analiz, segmentasyon ve iş kararlarına yönelik çıkarımlar, portföy amaçlı güçlü bir örnek oluşturmaktadır.

---

İstersen bu README’ye **görseller**, **grafikler** veya bir **Proje Sonuçları → Bullet listesi** ekleyebilirim.

Bir sonraki adım ne olsun?
