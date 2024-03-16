

#include <iostream>

using namespace std;

int main(){
    int pil, jarak, harga, ongkir, total;
    string nama;

    cout<< "Selamat datang di layanan pesan-antar makanan online! \n";
    cout<< "Atas nama siapa?";cin>>nama;
    cout<< "Mau pesan apa?\n1.Paket A (Rp25000)\n2.Paket B (Rp30000)\n3.Paket C (Rp45000)\n";
    cin>>pil;

    if (pil==1){cout<<"Okey, harga paket A=Rp25000\n"; harga=25000;}
    else if (pil==2){cout<<"Okey, harga paket B=Rp30000\n"; harga=30000;}
    else if (pil==3){cout<<"Okey, harga paket C=Rp45000\n"; harga=45000;}
    else {cout<<"error\n";harga=0;}
    cout<< "\nBerapa jarak rumah kamu ke restoran??\n1.Kurang dari 500m\n2.500m-1.5km\n3.lebih dari 1.5km\n";
    cin>>jarak;

    if (jarak==1){cout<<"Asik!!! Kamu dapat gratis ongkir\n"; ongkir=0;}
    else if (jarak==2){cout<<"Ongkos kirimmya Rp10000 yaa\n"; ongkir=10000;}
    else if (jarak==3){cout<<"Ongkos kirimnya Rp20000 yaa\n"; ongkir=20000;}
    else {cout<<"error\n";ongkir=0;}

    cout<< "=====================================================================\n\n";

    total=harga+ongkir;
    cout<< "Hai "<<nama;
    cout<< "\nHarga paket (Rp"<<harga<< ") + "<< "ongkir (Rp"<<ongkir<<") = "<< "Rp"<<total<<"\n";
    cout<<"Jadi total biaya yang harus kamu bayar adalah Rp"<<total;
    cout<< "\n\nTerima Kasih Sudah Memesan Paket Kami \nTunggu Sebentar Yaa... \n\n";

}

