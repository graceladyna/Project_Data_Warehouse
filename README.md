# Flight Delay and Cancellation Data Warehouse

## Deskripsi
Proyek ini merupakan implementasi Data Warehouse untuk menganalisis keterlambatan dan pembatalan penerbangan di Amerika Serikat periode 2019–2023. Sistem dibangun menggunakan pendekatan Ralph Kimball dengan memanfaatkan proses ETL, Star Schema, PostgreSQL, serta OLAP menggunakan Atoti untuk menghasilkan dashboard interaktif dan insight bisnis.

## Tujuan
- Menganalisis pola keterlambatan penerbangan.
- Mengidentifikasi faktor penyebab pembatalan penerbangan.
- Mengevaluasi performa maskapai dan bandara.
- Mendukung analisis multidimensi melalui OLAP.

## Teknologi yang Digunakan
- Python
- Pandas
- PostgreSQL / Supabase
- Atoti
- Jupyter Notebook

## Dataset

Dataset yang digunakan pada proyek ini mencakup data penerbangan Amerika Serikat periode 2019–2023.

**Sumber Data:**
- Kaggle: [Flight Delay and Cancellation Dataset](https://www.kaggle.com/datasets/patrickzel/flight-delay-and-cancellation-dataset-2019-2023?select=flights_sample_3m.csv)

Dataset meliputi:
- Informasi maskapai penerbangan
- Bandara asal dan tujuan
- Departure delay dan arrival delay
- Durasi dan jarak penerbangan
- Informasi pembatalan penerbangan dan alasannya
  
## Struktur Data Warehouse
### Fact Table
- fact_flight

### Dimension Table
- dim_date
- dim_airline
- dim_origin
- dim_destination
- dim_delay
- dim_cancellation

## Measures
- Total Flights
- Total Cancellation
- Average Departure Delay
- Average Arrival Delay
- Average Air Time
- Average Distance

## Hierarchy
### Date
Year → Quarter → Month → Day

### Airline
Airline → Airline Code

### Origin
Origin City → Origin Airport

### Destination
Destination City → Destination Airport

## Dashboard dan Analisis
Dashboard yang dibuat menggunakan Atoti meliputi:

- Ringkasan KPI Penerbangan
- Average Departure Delay per Airline
- Average Arrival Delay per Airline
- Total Cancellation per Airline
- Average Arrival Delay per Year
- Average Arrival Delay per Month
- Total Flights per Year
- Average Delay per Origin dan Destination Airport
- Cancellation Reason Analysis
- Hierarchy Drill Down (Year → Quarter → Month → Day)

## Insight Utama
- Rata-rata keterlambatan keberangkatan lebih tinggi dibandingkan keterlambatan kedatangan.
- JetBlue Airways dan Allegiant Air memiliki tingkat keterlambatan tertinggi.
- American Airlines dan Southwest Airlines memiliki jumlah pembatalan tertinggi.
- Faktor cuaca merupakan penyebab utama pembatalan penerbangan.
- Keterlambatan penerbangan kembali meningkat setelah pandemi.

## Anggota Kelompok
- Ayda’ Nur Salzabillah (24031554017)
- Jeika Antama Syalom Tarigan (24031554011) 
- Alifiyanti Putri Nur Azizah (24031554032) 
- Grace Pinkkan Ladyna (24031554137)

## Mata Kuliah
Data Warehouse – Program Studi S1 Sains Data  
Universitas Negeri Surabaya  
Tahun Akademik 2025/2026
