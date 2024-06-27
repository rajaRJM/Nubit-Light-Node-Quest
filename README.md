# Nubit-Light-Node-Quest
Light Node Quest




1. **Menginstal Paket Screen (jika belum ada):**
    ```bash
    sudo apt-get install screen
    ```

2. **Memeriksa Versi Screen:**
    ```bash
    screen --version
    ```

3. **Membuat Session Screen untuk Nubit:**
    ```bash
    screen -S nubit
    ```

4. **Menjalankan Nodenya:**
    ```bash
    curl -sL1 https://nubit.sh | bash
    ```

5. **Simpan Pubkey dan Jalankan Selama 15 Menit:**
    Setelah menjalankan nodenya, pastikan untuk memverifikasi bahwa semuanya berfungsi dengan baik.

6. **Keluar dari Session Screen:**
    Tekan `Ctrl + A` diikuti oleh `D` untuk keluar dari sesi screen.

7. **Masuk Kembali ke Session Screen:**
    Untuk masuk kembali ke sesi screen, jalankan:
    ```bash
    screen -r nubit
    ```

8. **Melihat Daftar Sesi Screen yang Ada:**
    ```bash
    screen -ls
    ```

9. **Menghapus Sesi Screen (Jika Diperlukan):**
    ```bash
    screen -X -S <session_id> quit
    ```

*Tambahan*


1. **Menghentikan dan Menonaktifkan Servis Nubit:**
    ```bash
    sudo systemctl stop nubit
    sudo systemctl disable nubit
    ```

2. **Menghapus Service Nubit:**
    ```bash
    sudo rm /etc/systemd/system/nubit.service
    ```

3. **Memuat Ulang Servis:**
    ```bash
    sudo systemctl daemon-reload
    ```

4. **Memeriksa Status Servis:**
    ```bash
    sudo systemctl status nubit
    ```

5. **Menghapus Semua Folder Terkait Nubit:**
    ```bash
    sudo rm -rf /root/nubit-node
    sudo rm -rf /root/.nubit-light-nubit-alphatestnet-1
    sudo rm -rf /root/.nubit-validator
    ```
