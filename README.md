# Ujian Akhir Semester 
<br>Mata Kuliah 	: Dasar Pemrogaman
<br> Nama		: Muhammad Shah Zaid
<br>NIM		:	1227050095
<br>Jurusan		:[Teknik Informatika](http://if.uinsgd.ac.id/) [UIN Sunan Gunung Djati Bandung](https://uinsgd.ac.id/) 

## Deskripsi Umum
Dalam Tugas Ulangan Akhir Semester ini kita diberikan soal yang sudah dipelajari sebelumnya, sebelum mengerjakan soal ini, kita harus memahami konsep array 2 dimensi dan matriks terlebih dahulu,kemudian kita ditugaskan untuk membuat kolom serta baris dan harus membagi habis nilai yang diinputkan yang dibagi oleh bilangan prima yaitu 3,5,7.
## Source Code 
  Tugas 1

     #include <iostream>
     #include <iomanip>
     using namespace std;
     int main(){

      int arr[100][100], jumlahBaris, jumlahKolom, i, j, baris, kolom;

      cout<< "Tugas Program Bilangan Yang Habis Dibagi 3,5,7\n";
      cout<< "==============================================\n";
      cout<< "Nama  : Muhammad Shah Zaid\n";
      cout<< "Nim   : 1227050095\n";
      cout<< "                                               \n";

        cout<<"Input jumlah baris: "; cin>>jumlahBaris;
        cout<<"Input jumlah kolom: "; cin>>jumlahKolom;
        cout << endl;

        for(i = 0; i < jumlahBaris; i++){
      for(j = 0; j < jumlahKolom; j++){
          cout << "Baris " <<i+1<<", kolom "<<j+1<< " = ";
          cin >> arr[i][j];
      }
      cout << endl;
        }

        cout << "Hasil input nilai : " << endl;

        for(i = 0; i < jumlahBaris ; i++){
        for(j = 0; j < jumlahKolom; j++){
      cout << setw(3) << arr[i][j] << " ";
        }
        cout << endl;
        }

        cout << "\nHasil bilangan yang habis dibagi 3,5,7 : " << endl;

        for(i = 0; i < jumlahBaris ; i++){
        for(j = 0; j < jumlahKolom; j++){
      if(arr[i][j] % 3 == 0 || arr[i][j] % 5 == 0 || arr[i][j] % 7 == 0){
      cout << setw(3) << arr[i][j] << " ";
      }
        }
        cout << endl;
        }


        cout << endl;
        return 0;
    }

 Tugas 2

    #include<iostream>
    #include<iomanip>
    using namespace std;

    int main(){

      int arr[100][100], jumlahBaris, jumlahKolom, i, j, baris, kolom;

      cout<< "Tugas Program Mencetak Matrix Transpos\n";
      cout<< "=======================================\n";
      cout<< "Nama  : Muhammad Shah Zaid\n";
      cout<< "Nim   : 1227050095\n";
        cout<< "                          \n";

        cout<<"Input jumlah baris: "; cin>>jumlahBaris;
        cout<<"Input jumlah kolom: "; cin>>jumlahKolom;
        cout << endl;

        for(i = 0; i < jumlahBaris; i++){
      for(j = 0; j < jumlahKolom; j++){
          cout << "Baris " <<i+1<<", kolom "<<j+1<< " = ";
          cin >> arr[i][j];
      }
      cout << endl;
        }
        cout << "Hasil matriks: " << endl;

        for(i = 0; i < jumlahBaris ; i++){
        for(j = 0; j < jumlahKolom; j++){
      cout << setw(3) << arr[i][j] << " ";
        }
        cout << endl;
        }

        baris = jumlahBaris;
        kolom = jumlahKolom;

        jumlahKolom = baris;
        jumlahBaris = kolom;

        cout << "\nUbah kolom jadi baris dan baris jadi kolom: " << endl;

        for(i = 0; i < jumlahBaris ; i++){
      for(j = 0; j < jumlahKolom; j++){
      cout << setw(3) << arr[j][i] << " ";
        }
        cout << endl;
        }
      return 0;
    }
## Output
Tugas 1
![Screenshot 2022-12-23 140548](https://user-images.githubusercontent.com/120699933/209293952-fa8940a7-6106-4c86-b6ba-d9bd575098f3.png)
Tugas 2
![Screenshot 2022-12-23 140411](https://user-images.githubusercontent.com/120699933/209294020-790f094b-ee17-49b0-b411-f769c471e0af.png)
