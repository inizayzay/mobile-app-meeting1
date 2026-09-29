# Tugas Pertemuan 1 - Dasar Dart

NIM: 1124160218
NAMA: ZACKY ZALFA FAHRUR ROZY

---

```dart
import 'package:flutter/material.dart';

void main() {
  print("hello world");
  print('hello worldd');

  String name = 'Kurt Cobain';

  print(name);

  int jumlah = 10;

  print(jumlah);

  bool cukupUsia;

  int usia = 15;

  cukupUsia = usia > 17 ? true : false;

  //   usia = "Sepuluh";
  //   usia = null

  String? namaIstri;

  namaIstri = null;

  print(cukupUsia ? "Anda boleh membuat KTP" : "Anda belum bisa membuat KTP");

  print(namaIstri);

  int hitung() {
    int hasil = 10 + 10;
    return hasil;
  }

  print(hitung());


  late String receiptNumber;

  void generateReceipt() {
    receiptNumber = 'REC-${DateTime.now().millisecondsSinceEpoch}';
    print(receiptNumber); // Aman dibaca setelah diinisialisasi
  }

  generateReceipt();

  print('Nama $name');


  double tinggiBadan = 1.7;;

  print('Tinggi Badan : $tinggiBadan');

//   List<String> makanan = [
//     'Sop Ayam',
//     'Lele',
//     'Tempe',
//     'Tempe'
//   ];

  Set<String> makanan = {
    'Sop Ayam',
    'Lele',
    'Tempe',
    'Tempe'
  };

  makanan.add('Pecel');

  print('Makanan Kesukaan : $makanan');
  String makananFavorit = makanan.elementAt(1);
  print('Makanan Favorit : $makananFavorit');

  Map<String, dynamic> produk = {
    'id': 1,
    'nama': 'Kemeja',
    'harga': 500000,
  };

  print('Ini produk $produk');

  Object namaDosen = 'Zacky';
  namaDosen = 30;
  namaDosen = true;
  namaDosen = 'Dodi';

  print(namaDosen);

  if (namaDosen is String) {
    print(namaDosen.toUpperCase());
  }
}
```
