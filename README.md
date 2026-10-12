# Negatif İyonizer Devresi Tasarımı ve Üretimi

Bu proje, yüksek gerilim tekniği prensipleri kullanılarak tasarlanmış ve fiziksel olarak üretilmiş bir **Negatif İyonizer** devresini içermektedir.

## Projenin Amacı ve Çalışma Prensibi
Negatif iyonizer, havaya negatif iyonlar salarak havadaki toz, duman ve polen gibi pozitif yüklü partikülleri nötralize edip yere çökmesini sağlayan bir cihazdır.
Devre, girişindeki alternatif akımı (AC) doğrultarak **Cockcroft-Walton voltaj çoklayıcı (merdiven)** yapısı ile yaklaşık **10 kV (10.000 Volt) DC** seviyesine
yükseltmektedir. Yüksek voltaj, çıkış terminalinde serbest elektronların havaya yayılmasını sağlayarak havayı temizler.

## Teknik Detaylar ve Hesaplamalar
* **Çoklayıcı Kademe:** Toplamda 31 adet diyot ve 31 adet kondansatör kullanılarak 15-16 kademeli bir gerilim çoklayıcı elde edilmiştir.
* **Formül:** Çıkış gerilimi hesaplamaları `Vout = n × Vpeak × 2` formülüne göre yapılmıştır (n = kademe sayısı).
* **Güvenlik:** Yüksek voltaj üretildiği için devredeki akımı sınırlandırmak ve güvenliği sağlamak amacıyla çıkışa seri olarak üç adet 1MΩ direnç eklenmiştir.

## Kullanılan Programlar ve Donanımlar
* **Yazılım:** Proteus (Devre şeması tasarımı, simülasyon ve PCB Layout çizimi).
* **Elektronik Komponentler:** 
  * 31 adet 1N4007 Diyot
  * 31 adet 150 nF (630V) Kapasitör
  * 3 adet 1MΩ Direnç, 100 mA Sigorta, Klemens

## Üretim (PCB Gerçekleme) Aşamaları
Proje yalnızca simülasyon ortamında kalmamış, tamamen donanımsal olarak üretilmiştir:
1. **Baskı İşlemi:** Proteus üzerinden alınan PCB Layout çıktısı, kuşe kağıt ve sıcak ütü yöntemi kullanılarak bakır plakete aktarıldı.
2. **Asit İndirme:** Perhidrol ve tuz ruhu (hidroklorik asit) karışımı ile bakır plaket çözeltiye atılarak devre yolları çıkarıldı.
3. **Delme ve Dizgi:** Matkap yardımıyla komponent yuvaları delindi ve devre elemanları karta dizilerek havya ile lehimleme  işlemleri tamamlandı.

**Proje Çalışma Videosu:**https://youtu.be/x75DJTbRKek 
