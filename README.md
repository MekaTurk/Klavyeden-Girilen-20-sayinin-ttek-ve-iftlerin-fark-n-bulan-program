//		Kullanıcının klavyeden girdiği 20 sayından tek ve çift sayıların toplamlarının farkını ekrana yazan program...
#include<iostream>
using namespace std;

main()
{
  int i,sayi,tektoplam=0,cifttoplam=0,yerdegisme; 
  
  for(i=1;i<=20;i++)
  {
  	cout<<i<<".Sayiyi Giriniz= "; cin>>sayi;
  	
  	if(sayi%2==0) {cifttoplam+=sayi;     }
  	if(sayi%2!=0) {tektoplam+=sayi;     }
	  }
	  if(cifttoplam<tektoplam) { yerdegisme=cifttoplam;  cifttoplam=tektoplam; tektoplam=yerdegisme;
	  }
  cout<<"Cift Sayiların Toplamları - Tek Sayilarin Toplamlari=  "<<cifttoplam-tektoplam;
  cout<<endl;
  system("pause");
}
