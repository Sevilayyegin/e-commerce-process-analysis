# 🎯 E-TİCARET BÜYÜME STRATEJİSİ: RFM TABANLI MÜŞTERİ SEGMENTASYONU VE SÜREÇ İYİLEŞTİRME VAKASI

Bu proje, Birleşik Krallık merkezli bir e-ticaret şirketinin 2010-2011 satış verilerini baz alarak kritik **iş sorunlarını** tespit etmek, **müşteri kayıp riskini (Churn)** analiz etmek ve operasyonel verimsizlikleri gidermeye yönelik **somut, eylem odaklı çözümler** önermek amacıyla yürütülmüştür.

Bu çalışma, klasik veri analizinin ötesine geçerek bir **İş Analisti (BA) Yaşam Döngüsünü** uygulamalı olarak göstermektedir: Sorun Tanımlama, Süreç Modelleme (As-Is/To-Be), Çözüm Tasarımı ve İş Değeri Hesaplama.

---

## 📌 İŞ DURUMU (BUSINESS CASE) VE KAPSAM


Bu proje, mevcut **As-Is** durumundaki kritik iş risklerini tanımlayarak, hedeflenen **To-Be** durumuna ulaşmak için bir yol haritası sunmaktadır.

### 2.1. İş Problemi ve Stratejik Gerekçe (The Business Need)

Şirket, operasyonel ve stratejik düzeyde iki ana zorlukla karşı karşıyadır:

1.  **Tek Pazar Bağımlılığı Riski:** Toplam gelirin %80'den fazlasının Birleşik Krallık'tan gelmesi, şirketi ekonomik ve politik dalgalanmalara karşı savunmasız bırakmaktadır. Uluslararası pazarlardaki **büyüme potansiyeli** yeterince değerlendirilememektedir.
2.  **Yüksek Operasyonel Kayıp:** %9 seviyesindeki iade oranı (yaklaşık £896K parasal karşılığı), lojistik ve paketleme süreçlerinde verimsizlik olduğunu ve müşteri memnuniyetinin düştüğünü göstermektedir. Bu, doğrudan **kar marjını** eriten bir maliyet kalemidir.

### 2.2. Proje Hedefleri ve Kapsam (To-Be Durumu)

Projenin temel hedefi, **RFM segmentasyonunu** kullanarak uluslararası pazarlarda sürdürülebilir bir büyüme sağlamak ve operasyonel maliyetleri düşürmektir.

#### A. Stratejik Hedef (Büyüme ve Elde Tutma)

* **Odak:** Fransa, Almanya, Hollanda, EIRE ve Avustralya pazarları.
* **Amaç:** RFM segmentlerine özel kişiselleştirilmiş kampanyalar ile **kayıp riski** altındaki müşterileri geri kazanmak ve **en değerli (Champions)** müşterilerin sadakatini artırmak.

#### B. Operasyonel Hedef (Süreç İyileştirme)

* **Amaç:** Mevcut **manuel ve yavaş iade sürecini** iyileştirmek için **Self-Servis İade Portalı** çözümü tasarlamak. Bu sayede hem operasyonel maliyetler düşürülecek hem de müşteri deneyimi iyileştirilecektir.

### 2.3. Başarı Kriterleri (Key Performance Indicators - KPIs)

Bu projenin başarısı, aşağıdaki somut ve ölçülebilir iş hedefleri ile değerlendirilecektir:

| Hedeflenen İyileşme Alanı | Mevcut Durum | Hedeflenen KPI |
| :--- | :--- | :--- |
| **Müşteri Geri Kazanım** | At Risk / Lost segmenti varlığı | Yeniden satın alma oranı (Recapture Rate) **%15 artış** |
| **Sadakat Programı Eşiği** | Champions AOV: £257.72 | **Champions** segmentinde Ortalama Sipariş Değerinde (AOV) **%5 artış** sağlanması. |
| **Operasyonel Verimlilik** | İade Oranı: %9 | İade oranını **%7'ye düşürmek** |

## ⚙️ PROJE YÖNETİMİ VE METODOLOJİ


Bu vaka çalışması, hızlı değer teslimine odaklanan **Çevik (Agile)** metodoloji çerçevesinde yürütülmüştür. Proje, tekrarlı ve aşamalı bir yaklaşım izleyerek, sürekli geri bildirim ve adapte olabilirlik prensipleriyle yönetilmiştir.

### 3.1. Yönetim Metodolojisi ve Süreç Akışı

| Metodoloji | Amaç | Takip Aracı Önerisi |
| :--- | :--- | :--- |
| **Agile (Çevik)** | Projeyi küçük, yönetilebilir parçalara (Sprint) ayırmak ve hızlıca iş değeri üretmek. | JIRA veya Trello (Sanal Kanban Panosu) |
| **Kanban (Sürekli Akış)** | İş Akışını (To Do, In Progress, Done) görselleştirmek ve darboğazları (Örn: Veri Temizliği) anında tespit etmek. | Veri analizi adımlarını görsel olarak yönetmek. |
| **Aşamalı Analiz** | Stratejik analizi (RFM) operasyonel analizden (İade Süreci) önce tamamlayarak, daha sonraki adımlara girdi sağlamak. | Analiz çıktılarına göre (RFM Segmentleri), çözüm tasarımı fazına geçiş kararı. |

### 3.2. İş Analizi Yaşam Döngüsü ve Kullanılan Teknikler

Bu projede kullanılan İş Analizi (BA) teknikleri, sorun tanımlamadan çözüm tasarımına kadar olan tüm süreci kapsamaktadır.

| Faz | Ana Odak | Kullanılan BA Aracı/Tekniği |
| :--- | :--- | :--- |
| **1. İş İhtiyacını Tanımlama** | Gelir riski ve operasyonel verimsizlikleri tespit etme. | **Kök Neden Analizi** (Yüksek iadenin nedenleri), **Sayısal KPI Analizi** (UK bağımlılığı). |
| **2. Modelleme ve Analiz** | Müşteri değerini ve süreç akışını anlama. | **RFM Segmentasyonu** (Python/Pandas), **AS-IS Süreç Modellemesi** (Mevcut İade Süreci). |
| **3. Çözüm Tasarımı** | İyileştirme gereksinimlerini belirleme ve çözümü görselleştirme. | **Gereksinim Belirleme** (BR & NFR), **TO-BE Süreç Modellemesi**, **Wireframe/Tel Kafes Tasarımı** (Self-Servis Portal). |

---


## 📊 ANA ANALİZ ÇIKTILARI VE İŞ ÇIKARIMLARI

### 1. Müşteri Segmentasyonunun Değerlendirilmesi (RFM)

RFM analizi, stratejik odaklanılması gereken segmentleri netleştirdi:

| Segment | Risk Seviyesi | Önerilen Strateji | Eylem Gereksinimi |
| :--- | :--- | :--- | :--- |
| **Needs Attention** | Orta - Yüksek | Tekrar alışverişi tetiklemek. | Kişiselleştirilmiş e-posta otomasyonu **(Tekrar Etkileşim)** |
| **At Risk / Lost** | Çok Yüksek | Geri kazanım kampanyaları. | İade sürecini hızlandıran **yeni bir self-servis arayüzü**. |
| **Champions** | Düşük | Elde tutma ve sadakati ödüllendirme. | **VIP/Premium** özelliklerin eklenmesi. |

### 2. İade Süreci Kök Neden Analizi

%9'luk iade oranı kritik bir operasyonel sorundur. Analiz, iadelerin yüksek oranda **düşük fiyatlı, yüksek hacimli** ürünlerde toplandığını gösterdi (muhtemel sebepler: paketleme hatası, yanlış ürün bilgisi).

**Sonuç:** Mevcut iade sürecinin **zahmetli** ve **yavaş** olması, kayıp müşterilerin geri kazanılmasını zorlaştırmaktadır.

---

## 🛠️ SÜREÇ İYİLEŞTİRME VE ÇÖZÜM ÖNERİLERİ

### A. Mevcut Durum (AS-IS) Süreç Modellemesi

Müşterinin manuel ve yavaş olan mevcut iade süreci (e-posta/çağrı bekleme, kargoya götürme, uzun geri ödeme süresi) **Draw.io** ile modellenmiştir.



![İade Süreci As-IS Akış Şeması](https://github.com/Sevilayyegin/e-commerce-process-analysis/blob/0f9a214ae3c4a29d58e16f1455594899defb7c7a/reports/%C4%B0ade%20S%C3%BCreci%20(AS-IS)%20Ak%C4%B1%C5%9F%20%C5%9Eemas%C4%B1%20drawio.drawio.png)


* **Tespit Edilen Engeller (Pain Points):** Manuel onay adımı, müşteri için kargo zahmeti, geri ödeme süresinin uzunluğu.

### B. Hedef Durum (TO-BE) ve Çözüm Tasarımı

Müşteri kaybını azaltmak ve iade sürecini hızlandırmak için yeni bir **"Self-Servis İade ve Geri Kazanım Portalı"** önerilmiştir.


#### 1. Yeni İş Gereksinimleri (Requirements)

| ID | Gereksinim Tipi | Açıklama | Çözüm Desteği |
| :--- | :--- | :--- | :--- |
| **BR-001** | Fonksiyonel | Müşteri, faturası üzerinden 5 dakikadan kısa sürede iade oluşturabilmelidir. | **TO-BE Süreci** |
| **BR-002** | Fonksiyonel | Kayıp riskli müşterilere iade yerine **anında kredi/kupon** teklif edilmelidir. | **RFM Stratejisi** |
| **NFR-001** | Performans | Geri ödeme süresi 7 iş gününden **48 saate** düşürülmelidir. | **Operasyonel İyileşme** |

#### 2. Self-Servis Arayüz Tasarımı (Balsamiq Wireframe)

Önerilen yeni sürecin ön yüzünü göstermek amacıyla **Balsamiq** (veya eşdeğeri) ile basit bir tel kafes (wireframe) taslağı oluşturulmuştur. Bu taslak, müşterinin hızlıca iade seçeneğini seçmesini ve alternatif olarak bir sonraki alışverişi için anında **hediye çeki** almasını sağlamaktadır.

![İade ve Değişim Merkezi](https://github.com/Sevilayyegin/e-commerce-process-analysis/blob/d979b97636aeddd5b9e684041ae987c9bacf31a2/reports/%C4%B0ade%20ve%20De%C4%9Fi%C5%9Fim%20Merkezi.png)

### C. Hedef Durum (TO-BE) Süreç Modellemesi

Önerilen çözümü içeren, daha hızlı ve verimli olan Hedef Durum süreci **Draw.io** ile modellenmiştir.

![İade Süreci TO-BE Akış Şeması](https://github.com/Sevilayyegin/e-commerce-process-analysis/blob/0f9a214ae3c4a29d58e16f1455594899defb7c7a/reports/TO-BE%20%C4%B0ade%20S%C3%BCreci.drawio.png)

* **İyileşme:** Manuel adımlar ortadan kalkar, müşteriye anında **kredi/kupon** teklif edilerek (kayıp riski altındaki müşteriler için) paranın şirket içinde kalması sağlanır.

---

## 📎 SONUÇ VE İŞ DEĞERİ

Bu proje, veri analizini doğrudan **uygulanabilir iş kararlarına** dönüştürmüş ve somut bir iş değeri yaratmıştır.

| Öneri | Beklenen İş Etkisi |
| :--- | :--- |
| **Geri Kazanım Kampanyaları** | **At Risk / Lost** segmentlerinin %15'inin geri kazanılmasıyla yıllık bazda tahmini **£30.000 - £35.000** **gelir artışı**. |
| **Self-Servis İade** | Operasyonel maliyetlerin azalması ve müşteri memnuniyetinin artması sonucu **İade Oranında %2 düşüş** (yaklaşık £190K tasarruf potansiyeli). |
| **Stratejik Risk Azaltma** | Uluslararası pazarlara (Hollanda, Almanya) odaklanarak **UK pazar bağımlılığı** riskinin uzun vadede azaltılması. |

Bu çalışma, İş Analisti olarak **problem çözme, paydaşlarla iletişim kurma (model/tasarım) ve veri sonuçlarını iş sonuçlarına çevirme** yeteneğimi göstermektedir.
