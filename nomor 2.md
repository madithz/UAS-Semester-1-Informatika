# UAS-Semester-1-Informatika
# Ujian Akhir Semester 
<br>Mata Kuliah 	: Dasar Pemrograman
<br> Nama		: Muhammad Aditya Hafizh Zahran
<br>NIM		:	1227050081
<br>Jurusan		:[Teknik Informatika](http://if.uinsgd.ac.id/) [UIN Sunan Gunung Djati Bandung](https://uinsgd.ac.id/) 

## Deskripsi Umum
Progam ini adalah progam yang membuat matriks namun, hanya menampilkan bilangan yang habis di bagi 3, 5 dan 7 pada matriks tersebut. Mula-mula kita harus menginput baris dan kolom pada matriks tersebut lalu menginput data/nilai dalam matriks tersebut sesuai dengan baris dan kolom. Lalu, progam ini akan otomatis memilih bilangan mana yang habis dibagi 3, 5 dan 7 dengan bilangan yang tidak habis dibagi 3, 5 dan 7. Bilangan yang tidak habis dibagi 3, 5 dan 7 di ganti dengan 0 sedangkan bilangan yang habis dibagi 3, 5 dan 7 akan tetap ditampilkan 
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

![Screenshot 2022-12-19 153936](https://user-images.githubusercontent.com/121005363/208383265-2c82130c-dfd3-4dc9-a6bf-dd8f78bcfe11.png)

