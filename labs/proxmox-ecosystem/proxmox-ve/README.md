# Lab Proxmox VE: Membangun Home-Lab Virtual

Ini adalah catatan pribadi saya saat belajar ngebangun *Hypervisor Type-1* (Proxmox VE) di atas laptop pribadi. Tujuannya sederhana: biar saya bisa simulasi lab jaringan yang kompleks tanpa harus gonta-ganti OS di laptop utama.

## Spesifikasi "Tempur"
Biar kebayang kapasitas laptop saya buat nahan beban virtualisasi ini:
- **Host Laptop:** AMD Ryzen 5 5652U with Radeon Graphics
- **RAM:** 16 GB DDR4
- **Hypervisor:** Proxmox VE 8.x (Jalan di atas VMware Workstation)
- **Mode Jaringan:** Bridged (biar dapet IP lokal langsung dari router rumah)

## Kenapa Proxmox?
Saya milih Proxmox karena ini *open-source* dan fiturnya lengkap banget buat latihan simulasi jaringan (bisa buat VM sama Container/LXC sekaligus). Ditambah lagi, performanya jauh lebih enteng dibanding simulasi di dalam OS Windows langsung.

## Tantangan yang Saya Hadapi
*Tuliskan di sini apa yang bikin Anda pusing pas install*
Contoh:
- Awalnya bingung pas aktivasi *Nested Virtualization* di VMware. Ternyata fiturnya harus dicentang manual di *Settings*.
- Sering *crash* pas awal booting karena RAM kebagi dua, jadi harus pinter-pinter ngatur *resource* VM-nya.

## Apa yang Saya Pelajari
- Cara setup *Nested Virtualization* di level VMware.
- Konfigurasi `vmbr0` supaya VM di dalam Proxmox bisa dapet koneksi internet.
- Belajar bahwa manajemen *resource* itu penting banget kalau mainan *Hypervisor*.

---
*Catatan: Dokumentasi ini bakal saya update terus seiring bertambahnya topologi lab yang saya buat di sini.*