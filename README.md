# Dokumentasi Ruang Kerja: Pengolahan Citra Digital
### Praktikum Machine Learning - Computer Vision

Repositori ini menyimpan catatan teknis mengenai prosedur penyiapan lingkungan kerja (environment setup) untuk keperluan analisis citra digital. Seluruh proses instalasi dan konfigurasi di bawah ini merujuk pada materi pengenalan tools dan library yang disampaikan pada video tutorial pertama.

## Informasi Praktikan
* **Nama:** Nur Wanda Aulia
* **NIM:** 231001066
* **Mata Kuliah:** Praktikum Machine Learning
* **Dosen Pengampu:** Bapak Herfandi, A.Md., S.Kom., M.Kom

---

## Prosedur Persiapan Sistem (Berdasarkan Tutorial)

Berikut adalah urutan langkah teknis yang saya lakukan untuk memastikan sistem siap menjalankan algoritma Computer Vision:

### 1. Manajemen Paket menggunakan Anaconda
Sesuai arahan, saya menggunakan **Anaconda** sebagai *package manager* utama. Hal ini mempermudah pengelolaan berbagai library Python yang diperlukan dalam riset data science dan Computer Vision.

### 2. Konfigurasi Isolate Environment
Untuk menghindari konflik antar library, saya membuat lingkungan kerja terisolasi melalui **Anaconda Prompt**.
* **Perintah:** `conda create --name ENV_BELAJAR python=3.11` (menggunakan versi Python yang stabil untuk OpenCV).
* **Aktivasi:** Menjalankan perintah `conda activate ENV_BELAJAR` untuk masuk ke ruang kerja tersebut.

### 3. Instalasi Library Inti (OpenCV)
Tahap selanjutnya adalah memasang library utama, yaitu **OpenCV** (Open Source Computer Vision Library). Library ini merupakan komponen paling vital untuk melakukan manipulasi matriks gambar dan video.
* **Perintah:** `conda install opencv` atau melalui channel `conda-forge`.

### 4. Pengembangan menggunakan Jupyter Lab
Dalam praktik ini, saya menggunakan **Jupyter Lab** sebagai IDE (Integrated Development Environment) karena tampilannya yang interaktif dan memudahkan dalam melakukan visualisasi data gambar secara langsung.

### 5. Verifikasi dan Validasi
Langkah terakhir adalah memastikan library telah terhubung dengan benar. Saya menjalankan *script* pengujian berikut pada Jupyter Notebook:
```python
import cv2
print("Versi OpenCV terdeteksi:", cv2.__version__)
