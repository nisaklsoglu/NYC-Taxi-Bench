# NYC Yellow Taxi Cost & Time Estimator

Bu proje, NYC Yellow Taxi verilerini kullanarak maliyet ve zaman tahminleme simülasyonu yapmaktadır.

## Proje Yapısı
Projeyi klonladıktan sonra kök dizinde aşağıdaki klasör yapısını manuel olarak oluşturmanız gerekmektedir:

cab_cost_and_time_estimator/ ├── data/ │ ├── raw/ # Ham .parquet dosyaları buraya konulmalı │ └── clean/ # ETL boru hattı çıktıları buraya yazılacak ├── notebooks/ # Jupyter Notebook dosyaları └── README.md


## Veri Kümesinin Temini
Projede kullanılan veriler büyük boyutlu (12 GB+) olduğu için GitHub deposuna dahil edilmemiştir. 
Verileri çalıştırmak için:
1. [NYC TLC Trip Record Data](https://www.nyc.gov/site/tlc/about/tlc-trip-record-data.page) sayfasına gidin.
2. 2023 yılına ait **Yellow Taxi Trip Records** (Ocak - Aralık) dosyalarını indirin.
3. İndirilen dosyaları `data/raw/yellow_tripdata_2023/` klasörünün altına yerleştirin.
4. Ardından preprocessing (ön işleme) notebook'unu çalıştırarak `data/clean/` veritabanını oluşturun.