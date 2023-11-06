# Tugas2-BigData

## Scheduling Crawling Data Airflow :
Apache Airflow:
Instal dan konfigurasi Apache Airflow.
Buat DAG (Directed Acyclic Graph) untuk menjadwalkan dan mengotomatisasi proses crawling data.

## Instalasi dan Konfigurasi Hadoop:
- pada tugas ini kami menggunakan hadoop di cloudera (linux) menggunakan vmbox
## Crawling Data dan Disimpan di HDFS (Sqoop):

Sqoop adalah alat yang memungkinkan Anda untuk mentransfer data antara Hadoop dan penyimpanan struktural seperti basis data relasional.

1. Persiapkan Data dan Tabel:
   Pastikan data hasil crawling sudah disimpan di sistem lokal atau di basis data yang dapat diakses oleh Sqoop.

3. Gunakan perintah Sqoop untuk mengimpor data dari sumber eksternal ke dalam HDFS. contoh :
   sqoop import --connect jdbc:mysql://hostname:port/database_name --username username --password password --table table_name --target-dir /path/in/hdfs


### Melakukan Analisis Descriptive / Predictive (Hive):
Persiapkan :
- Pastikan data hasil crawling sudah disimpan di HDFS atau tersedia di dalam kontainer Hadoop.

Masuk ke konsol Hive dengan perintah: hive

Buat Tabel Hive :
- Di dalam Hive, buat tabel untuk data hasil crawling menggunakan  perintah "CREATE TABLE" sesuai dengan data crawling

Process data :
- Setelah tabel dibuat, gunakan perintah LOAD DATA di Hive untuk mengimpor data dari HDFS ke dalam tabel Hive.
- Lakukan Analisis di hive
