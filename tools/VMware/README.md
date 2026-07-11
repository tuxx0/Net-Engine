# VMware

VMware adalah software virtualisasi yang digunakan untuk membuat dan menjalankan **Virtual Machine (VM)**. Dengan VMware, beberapa sistem operasi dapat berjalan dalam satu komputer secara bersamaan.

VMware termasuk **Hypervisor**, yaitu perangkat lunak yang mengelola Virtual Machine dan membagi sumber daya komputer seperti CPU, RAM, Storage, dan Network kepada setiap VM.

---

## Tipe Hypervisor

Secara umum terdapat dua jenis Hypervisor.

<p align="center">
    <img src="https://github.com/tuxx0/Net-Engine/blob/main/tools/Assets/Types%20of%20Hypervisor.png?raw=true" width="700">
</p>

### Type 1 (Bare Metal)

Berjalan langsung di atas hardware tanpa sistem operasi host.

**Contoh**
- VMware ESXi
- Microsoft Hyper-V
- Xen

### Type 2 (Hosted)

Berjalan di atas sistem operasi seperti aplikasi biasa.

**Contoh**
- VMware Workstation
- VMware Fusion
- Oracle VirtualBox

> VMware Workstation yang digunakan pada dokumentasi ini merupakan **Hypervisor Type 2**.

---

## Persyaratan

Sebelum menginstal VMware, pastikan komputer memenuhi persyaratan berikut.

- CPU mendukung Intel VT-x atau AMD-V
- Virtualization telah diaktifkan pada BIOS/UEFI
- RAM minimal 8 GB (disarankan 16 GB)
- Ruang penyimpanan minimal 30 GB

---

## Instalasi VMware

### 1. Download Installer

Download VMware sesuai sistem operasi.

- Windows → VMware Workstation Pro
- Linux → VMware Workstation Pro
- macOS → VMware Fusion

---

### 2. Jalankan Installer

Buka file installer, kemudian ikuti proses instalasi.

```
Next
↓
Accept License
↓
Typical Installation
↓
Install
↓
Finish
```

Restart komputer jika diminta.

---

### 3. Membuat Virtual Machine

Setelah instalasi selesai.

1. Klik **Create a New Virtual Machine**
2. Pilih file ISO sistem operasi
3. Tentukan nama Virtual Machine
4. Atur CPU, RAM, dan Storage
5. Klik **Finish**
6. Jalankan Virtual Machine

---

## Mode Network VMware

| Mode | Fungsi |
|------|--------|
| NAT | VM dapat mengakses internet melalui Host. |
| Bridged | VM berada pada jaringan yang sama dengan Host. |
| Host-Only | VM hanya dapat berkomunikasi dengan Host dan VM lainnya. |

---

## Troubleshooting

### Virtualization belum aktif

**Gejala**

```
VMware requires Intel VT-x / AMD-V.
```

**Solusi**

Aktifkan Intel VT-x atau AMD-V melalui BIOS/UEFI.

---

### Virtual Machine tidak mendapat internet

Periksa:

- Network Adapter
- Mode NAT / Bridged
- DHCP

---

### Resolusi layar kecil

Install **VMware Tools**, kemudian restart Virtual Machine.