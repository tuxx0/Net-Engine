# VMware

VMware adalah software virtualisasi yang digunakan untuk membuat dan menjalankan **Virtual Machine (VM)**. Dengan VMware, beberapa sistem operasi dapat berjalan dalam satu komputer secara bersamaan.

VMware termasuk **Hypervisor**, yaitu perangkat lunak yang mengelola Virtual Machine dan membagi sumber daya komputer seperti CPU, RAM, Storage, dan Network kepada setiap VM.

---

## Tipe Hypervisor


<p align="center">
    <img src="https://github.com/tuxx0/Net-Engine/blob/main/tools/Assets/Types%20of%20Hypervisor.png?raw=true" width="700">
</p>

Secara umum terdapat dua jenis Hypervisor:
* **Type-1 (Bare Metal):** *Hypervisor* diinstal langsung di atas perangkat keras (seperti sistem operasi utama). Contoh: VMware ESXi, Proxmox. Biasanya digunakan di level *data center* atau *server* produksi karena performanya yang sangat efisien.
* **Type-2 (Hosted):** *Hypervisor* diinstal sebagai aplikasi di atas sistem operasi utama (seperti Windows, macOS, atau Linux). Contoh: VMware Workstation Pro, VMware Fusion, Oracle VirtualBox. Inilah yang kita gunakan untuk kebutuhan *lab* pribadi di laptop.

---

## Langkah-Langkah Instalasi & Setup

### A. Persiapan Awal
1. **Spesifikasi Laptop:** Minimal RAM 8GB (disarankan 16GB), penyimpanan SSD, dan prosesor yang mendukung virtualisasi.
2. **BIOS/UEFI:** Pastikan fitur **Virtualization Technology (VT-x / AMD-V)** sudah **Enabled** di BIOS laptop Anda.

### B. Instalasi VMware
1. Kunjungi portal resmi Broadcom untuk mengunduh installer: [Broadcom Support Portal](https://support.broadcom.com/). Daftar dulu kalo belum punya akun
2. Pada kolom pencarian ketikan saja VMware/VMware workstation

<p align="center" > 
<img width="776" height="308" alt="Image" src="https://github.com/user-attachments/assets/068fa3fe-ef87-4563-8211-6084690ce513" />    
</p>

3. Pilih menu "My Downloads" dan klik kata "here" ini

<p align="center">
   <img width="776" height="308" alt="Image" src="https://github.com/user-attachments/assets/d0d04dce-c3ce-42e7-b18b-ff34d8cc44f7" />
</p>

4. Cari "VMware Workstation Pro" untuk Windows/Linux, atau "VMware Fusion Pro" untuk macOS. Pilih Versi terbarunya dan Download dengan klik gambar awan


<p align="center">
<img width="776" height="308" alt="Image" src="https://github.com/user-attachments/assets/34773bc1-f5e8-4fcd-a498-f6436b4fb2a6" />
</p>

<p align="center">
<img width="776" height="308" alt="Image" src="https://github.com/user-attachments/assets/a94ba7bd-4ead-48c7-a176-c1526c73edf8" />
</p>

*NB:*
*Kalo gabisa di download kita harus baca terms and conditionnya dl lalu centang dan download deh*

5. Terakhir, buka file hasil downloadnya dan selesaikan setup wizard instalationnya-*klik next next aja*

