# 📘 Flutter Master Plan App

Aplikasi sederhana berbasis Flutter untuk mengelola rencana (plan) dan daftar tugas (task).  
Project ini dibuat sebagai bagian dari praktikum Flutter.

---

## 🎬 Demo Aplikasi
![Demo App](lib/images/apk%20(1).png)
![Demo App](lib/images/apk%20(2).png)

---

## 🚀 Fitur
- Menambahkan Plan baru
- Menambahkan Task dalam Plan
- Mengedit Task secara langsung
- Menandai Task selesai (checkbox)
- Menampilkan progress task
- Scroll otomatis + dismiss keyboard

---

## 🧠 Konsep yang Digunakan
- StatefulWidget
- InheritedNotifier
- ValueNotifier
- ListView.builder
- Flutter Lifecycle (initState & dispose)

---

# 📘 Flutter Master Plan App (Praktikum 2)

Aplikasi ini merupakan implementasi dari Praktikum 2 yang berfokus pada pengelolaan state menggunakan **InheritedWidget** dan **InheritedNotifier** dalam Flutter.

---

## 🎬 Demo Aplikasi
![Demo App](lib/images/apk%20(5).png)
![Demo App](lib/images/apk%20(4).png)
![Demo App](lib/images/apk%20(3).png)


---

## 🚀 Deskripsi Aplikasi
Aplikasi Master Plan digunakan untuk mengelola daftar rencana (plan) dan tugas (task).  
Pada praktikum ini, aplikasi dikembangkan dengan memisahkan data layer dan view menggunakan InheritedWidget sehingga pengelolaan state menjadi lebih terstruktur dan efisien.

---

## ⚙️ Fitur Aplikasi
- Menambahkan task baru ke dalam plan
- Mengedit task secara langsung melalui input field
- Menandai task sebagai selesai menggunakan checkbox
- Menampilkan progress jumlah task yang telah selesai
- UI otomatis ter-update saat data berubah (tanpa setState)

---

## 🛠️ Implementasi
Pada praktikum ini dilakukan beberapa perubahan utama:
- Menggunakan `PlanProvider` sebagai penghubung data (state) ke seluruh widget
- Menggunakan `ValueNotifier` untuk menyimpan dan memperbarui data
- Menggunakan `ValueListenableBuilder` untuk membangun UI secara reaktif
- Menambahkan `SafeArea` untuk menampilkan progress task di bagian bawah layar

---

## 🧪 Hasil Akhir
Setelah seluruh langkah praktikum diselesaikan:
- Aplikasi dapat menampilkan daftar task secara dinamis
- Perubahan data langsung terlihat pada UI
- Tidak diperlukan penggunaan `setState` untuk update tampilan
- Struktur kode menjadi lebih rapi karena memisahkan data dan tampilan

---

## 🐞 Perbaikan Error
Selama pengerjaan praktikum, beberapa error yang ditemukan dan diperbaiki:
- Kesalahan penggunaan tipe data setelah perubahan ke `ValueNotifier`
- Penyesuaian parameter `BuildContext` pada beberapa method
- Perbaikan struktur widget agar sesuai dengan konsep state management

---

