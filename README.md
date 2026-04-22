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


## 🧪 Praktikum 3: Pengelolaan Plan & Navigasi

Pada praktikum ini, aplikasi Master Plan dikembangkan lebih lanjut dengan menambahkan fitur pengelolaan banyak plan serta navigasi antar halaman.

---

## 🎬 Demo Praktikum 3
![Demo App](lib/images/apk (12).png)
![Demo App](lib/images/apk (11).png)
![Demo App](lib/images/apk (10).png)
![Demo App](lib/images/apk (9).png)
![Demo App](lib/images/apk (8).png)
![Demo App](lib/images/apk (7).png)
![Demo App](lib/images/apk (6).png)

---

## 🚀 Deskripsi Implementasi

Pada praktikum ini dilakukan pengembangan aplikasi dengan mengubah struktur data dari satu plan menjadi banyak plan (`List<Plan>`). Hal ini memungkinkan pengguna untuk membuat beberapa rencana sekaligus dan mengelola task di dalam setiap plan secara terpisah.

Aplikasi juga ditambahkan halaman baru yaitu `PlanCreatorScreen` yang berfungsi untuk menambahkan plan baru. Pada halaman ini, pengguna dapat memasukkan nama plan melalui `TextField`, kemudian data akan disimpan ke dalam `PlanProvider` menggunakan `ValueNotifier`.

Selain itu, ditambahkan fitur navigasi menggunakan `Navigator.push` untuk berpindah dari halaman daftar plan ke halaman detail plan (`PlanScreen`). Pada halaman detail, pengguna dapat menambahkan task, mengedit task, serta menandai task sebagai selesai.

---

## ⚙️ Fitur yang Dihasilkan
- Menambahkan plan baru
- Menampilkan daftar plan secara dinamis
- Navigasi ke halaman detail plan
- Menambahkan dan mengedit task dalam plan
- Menandai task sebagai selesai
- Menampilkan progress task pada setiap plan
- Update UI secara otomatis tanpa `setState`

---

## 🧪 Hasil Akhir
Setelah seluruh langkah praktikum diselesaikan, aplikasi berhasil berjalan dengan baik di mana pengguna dapat:
- Menambahkan beberapa plan
- Melihat daftar plan secara real-time
- Masuk ke detail plan
- Mengelola task di dalam plan

Semua perubahan data langsung diperbarui pada tampilan, yang menunjukkan bahwa state management menggunakan `InheritedNotifier` dan `ValueNotifier` telah berjalan dengan baik.

---

## 🐞 Perbaikan Error
Selama proses pengerjaan, beberapa error yang ditemukan dan diperbaiki:
- Perubahan tipe data dari `Plan` menjadi `List<Plan>`
- Penyesuaian penggunaan `PlanProvider.of(context)`
- Perbaikan konflik data saat update plan dalam list
- Penyesuaian navigasi antar screen

---