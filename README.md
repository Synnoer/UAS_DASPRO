# Ujian Akhir Semester
<br>Mata Kuliah	: Dasar Pemrograman
<br>Nama	: Dimas Arya Nurhakim
<r>NIM		: 1227050038
<br>Jurusan	: [Teknik Informatika](http://if.uinsgd.ac.id/) [UIN Sunan Gunung Djati Bandung](https://uinsgd.ac.id/)

# Deskripsi Umum
Program Array 2 dimensi, Menukar baris dan kolom sebuah array
  
# Source Code
	#include<iostream>
	#include<conio.h>
	using namespace std;

	int main(){
	cout<<"Membalikkan Baris dan Kolom Array\n";
	cout<<"=================================\n";	
	//Input baris dan kolom array dimensi 2
    	int i,j,b,k;
	cout<<"Masukkan baris: ";cin>>b;
	cout<<"Masukkan kolom: ";cin>>k;
    	int a[b][k];
    	int aa[k][b];
    
	//Input Nilai
	for(i = 1; i <= b; i++){    
		for(j = 1; j <= k; j++){      
		cout<<"Masukan Nilai {"<<i<<","<<j<<"} : ";cin>>a[i][j];    
		}
	}
	for(i = 1; i <= b; i++){    
		for(j = 1; j <= k; j++){              
		aa[j][i] = a[i][j];    
		}
	}
	
	//Ubah baris menjadi kolom; kolom menjadi baris
	system("cls");
	cout<<"Array : \n";
	for(i = 1; i <= b; i++){
		for(j = 1; j <= k; j++){        
		cout<<"    "<<a[i][j];
		}  
	cout<<endl;
	}
	
	cout<<"\nArray Terbalik : \n";
	for(i = 1; i <= k; i++){
		for(j = 1; j <= b; j++){        
		cout<<"    "<<aa[i][j];
		}  
	cout<<endl;
	}
	cout<<"\n==================================\n";
	cout<<"Dimas Arya N <"<<"> 1227050038";
   	getch();
	}
  
# Output
  Array :
  <br>1    2    3    4
  <br>5    6    7    8

  Array Terbalik :
  <br>1    5
  <br>2    6
  <br>3    7
  <br>4    8
