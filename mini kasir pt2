#include <iostream>
using namespace std;

// Fungsi menampilkan menu
void tampilkanMenu() {
    cout << "============================" << endl;
    cout << "        MINI KASIR" << endl;
    cout << "============================" << endl;

    cout << "\n--- MENU MAKANAN ---" << endl;
    cout << "1. Soto  : Rp15000" << endl;
    cout << "2. Rawon : Rp20000" << endl;
    cout << "3. Pecel : Rp10000" << endl;

    cout << "\n--- MENU MINUMAN ---" << endl;
    cout << "1. Teh   : Rp3000" << endl;
    cout << "2. Kopi  : Rp5000" << endl;

    cout << "============================" << endl;
}

// Fungsi menghitung total
int hitungTotal(int harga, int jumlah) {
    return harga * jumlah;
}

int main() {
    int makanan, minuman;
    int jumlahMakan, jumlahMinum;
    int hargaMakan, hargaMinum;
    int total, bayar, kembalian;
    char ulang;

    do {
        tampilkanMenu();

        cout << "\nPilih makanan (1-3): ";
        cin >> makanan;

        if (makanan == 1) {
            hargaMakan = 15000;
        }
        else if (makanan == 2) {
            hargaMakan = 20000;
        }
        else if (makanan == 3) {
            hargaMakan = 10000;
        }
        else {
            cout << "Menu makanan tidak tersedia!" << endl;
            continue;
        }

        cout << "Jumlah makanan: ";
        cin >> jumlahMakan;

        if (jumlahMakan <= 0) {
            cout << "Jumlah tidak valid!" << endl;
            continue;
        }

        cout << "\nPilih minuman (1-2): ";
        cin >> minuman;

        if (minuman == 1) {
            hargaMinum = 3000;
        }
        else if (minuman == 2) {
            hargaMinum = 5000;
        }
        else {
            cout << "Menu minuman tidak tersedia!" << endl;
            continue;
        }

        cout << "Jumlah minuman: ";
        cin >> jumlahMinum;

        if (jumlahMinum <= 0) {
            cout << "Jumlah tidak valid!" << endl;
            continue;
        }

        int totalMakan = hitungTotal(hargaMakan, jumlahMakan);
        int totalMinum = hitungTotal(hargaMinum, jumlahMinum);

        total = totalMakan + totalMinum;

        cout << "\n============================" << endl;
        cout << "         STRUK KASIR" << endl;
        cout << "============================" << endl;
        cout << "Total makanan : Rp" << totalMakan << endl;
        cout << "Total minuman : Rp" << totalMinum << endl;
        cout << "Total bayar   : Rp" << total << endl;

        cout << "\nUang pembayaran: Rp";
        cin >> bayar;

        if (bayar < total) {
            cout << "Uang pembayaran kurang!" << endl;
        }
        else {
            kembalian = bayar - total;

            cout << "Kembalian     : Rp" << kembalian << endl;
            cout << "============================" << endl;
            cout << "       TERIMA KASIH!" << endl;
        }

        cout << "\nTransaksi lagi? (y/n): ";
        cin >> ulang;

    } while (ulang == 'y' || ulang == 'Y');

    cout << "\nProgram selesai!" << endl;

    return 0;
}
