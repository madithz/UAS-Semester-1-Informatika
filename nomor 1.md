# UAS-Semester-1-Informatika
# Ujian Akhir Semester 
<br>Mata Kuliah 	: Dasar Pemrograman
<br> Nama		: Muhammad Aditya Hafizh Zahran
<br>NIM		:	1227050081
<br>Jurusan		:[Teknik Informatika](http://if.uinsgd.ac.id/) [UIN Sunan Gunung Djati Bandung](https://uinsgd.ac.id/) 

## Deskripsi Umum
Progam ini adalah progam untk mentranspose matriks dengan cara meningput jumlah baris dan kolom sebuah matriks. Lalu, matriks tersebut akan diisi data/nilai sesuai dengan baris dan kolom pada matriks serta diakhir progam akan mentranspose matriks dengan mengubah kolom menjadi baris dan baris menjadi kolom.
## Source Code

```
#include <iostream>
using namespace std;

int main(){
  int x, y; 
  int baris, kolom; 
  int matriks[100][100], matrikst[100][100];
  
  cout << "Selamat datang diprogam men-Transpose-kan Matriks \n";
  cout << "====================================================\n";
  
  cout << "Masukkan baris matriks: ";
  cin >> baris;
  cout << "Masukkan kolom matriks: ";
  cin >> kolom;

  cout << "\nMasukkan elemen matriks\n";
  for (x = 1; x <= baris; x++){
    for (y = 1; y <= kolom; y++){
      cout << "Baris ke-" << x << ", kolom ke-" << y << " : ";
      cin  >> matriks[x][y];
    }
  }
  
  cout << "\nBerikut adalah matriks yang anda input : \n";
  for (x = 1; x <= baris; x++){
    for (y = 1; y <= kolom; y++){
      cout << matriks[x][y] << " ";
    }
    cout << endl;
  }
  
  for (x = 1; x <= baris; x++){
    for (y = 1; y <= kolom; y++){
      matrikst[y][x] = matriks[x][y];
    }
  }
  
  cout << "\nBerikut adalah transpose dari matriks yang telah di input : \n";
  for (x = 1; x <= kolom; x++){
    for (y = 1; y <= baris; y++){
      cout << matrikst[x][y] << "\t";
    }
    cout << endl;
  }
}
```

## Output

![Screenshot 2022-12-19 153238](https://user-images.githubusercontent.com/121005363/208382456-30e9bf9f-43d5-4e3e-9ccf-38d6d8192d6d.png)
