# Veriden-Karara-U-tan-Uca-M-teri-Stratejileri
Python ve Pandas kullanılarak gerçekleştirilen, ham veriyi RFM (Recency, Frequency, Monetary) segmentasyonuna ve stratejik iş kararlarına dönüştüren uçtan uca müşteri analitiği projesi.

🚗 Otomotiv Sektöründe Veri Odaklı Müşteri Segmentasyonu (RFM Analizi)

📌 Proje Özeti
Bu çalışma, otomotiv satış sonrası hizmetler (servis, yedek parça, bakım) verilerini kullanarak müşteri bağlılığını ve kârlılığını artırmayı hedefleyen analitik bir modeldir. Ham servis verileri RFM (Recency, Frequency, Monetary) metodolojisi ile işlenerek, her bir müşteri segmenti için özelleştirilmiş aksiyon planları oluşturulmuştur.

🛠️ İş Problemi ve Çözüm
Otomotiv dünyasında müşteriyle kurulan bağ, araç anahtarı teslim edildiğinde bitmez; asıl o an başlar. Ancak, binlerce araçlık portföyde hangi müşterinin kaybedilme riski taşıdığını veya hangi grubun sadakat programına dahil edilmesi gerektiğini manuel olarak takip etmek imkansızdır.

Çözüm: Python ve Pandas kütüphaneleri kullanılarak geliştirilen bu algoritma;

    Kirli ve eksik verileri temizler.

    Müşterileri harcama gücü ve servis ziyaret sıklığına göre segmente eder.

    Pazarlama ve servis operasyonları için veri odaklı bir yol haritası sunar.
    

🚀 Analitik İş Akışı
1. Veri Ön İşleme (Data Preprocessing)

    Veri Temizliği: Negatif harcama tutarları ve eksik (NaN) servis kayıtları ayıklandı.

    Tarih Dönüşümü: Servis ziyaret tarihleri, analiz edilebilir zaman nesnelerine çevrildi.

    Recency Hesaplama: Müşterinin son servis ziyaretinden bugüne geçen gün sayısı (pasiflik süresi) hesaplanarak aktiflik durumu belirlendi.


2. Segmentasyon Mantığı (RFM Logic)

Algoritma, müşterileri şu 4 stratejik gruba ayırır:

    💎 VIP (Yüksek Değer & Aktif): Düzenli servis ziyareti yapan ve yüksek bütçeli bakım/yedek parça harcaması olan kitle.

    ⭐ Sadık (Geri Kazanılmalı): Geçmişte yüksek değer üretmiş ancak servis periyodu gecikmiş müşteriler.

    🌱 Potansiyel (Yeni/Aktif): Yeni araç almış veya ilk servisini yapmış, sadakat programına aday grup.

    🚨 Risk (Kaybedilme Olasılığı): Hem harcama tutarı düşük hem de servis ziyaretleri arasındaki süre çok uzamış kitle.

📊 Görsel Raporlama ve Stratejik Notlar
![Otomotiv Satış Sonrası Hizmetlerde Stratejik Müşteri Analizi  1](https://github.com/user-attachments/assets/b0de32d0-e503-4f5e-8533-f290c0050d2c)


Proje çıktısı olarak üretilen "Otomotiv Müşteri Portföyü Dağılımı" grafiği, işletmenin mevcut durumunu tek bir karede özetler.


    📍 Stratejik Not:
    Analiz sonucunda portföyün %20'sinin Risk, %40'ının Potansiyel ve %40'ının VIP/Sadık olduğu saptanmıştır. Bu veriler ışığında, kaynakların %40'lık potansiyel grubu sadık hale getirmek için kullanılması önerilmektedir.

💻 Kullanılan Teknolojiler

    Python: Ana geliştirme dili.

    Pandas: Veri temizleme, manipülasyon ve RFM hesaplamaları.

    Matplotlib: Sektörel raporlama görselleri.

    Io & Datetime: Veri akışı yönetimi.

📂 Çıktılar

    otomotiv_segmentasyon_analizi.png: Segmentasyon dağılım grafiği.

    otomotiv_stratejik_analiz_raporu.csv: Her bir müşterinin atanmış segmentini içeren detaylı liste.


