# Pre-Test Bootcamp DevOps

## knowledge base

1. Apa yang anda ketahui tentang DevOps?
2. Apa yang anda ketahui tentang Infrastructure?
3. Apa yang anda ketahui tentang server, sebutkan implementasi berserta contohnya?
4. Mengapa server dibutuhkan dalam pengembangan/development suatu software?
5. Apa yang anda ketahui mengenai Virtualisasi dan Container?
6. Mengapa teknology container saat ini sangat populer?
7. Apa yang anda ketahui tentang Orchestration Container System?

Cara pengerjaan, silahkan update file ini tulis jawabanya di bawah ini

## Jawaban

### 1. Apa yang anda ketahui tentang DevOps?

DevOps adalah pendekatan yang menggabungkan tim pengembangan (Dev) dan operasi (Ops) untuk menciptakan alur kerja perangkat lunak yang lebih efisien. Tujuannya adalah meningkatkan kecepatan, kualitas, dan keandalan produk.

Konsep kunci: kolaborasi, otomatisasi, kontinuitas, dan kualitas.

Manfaat: pengiriman lebih cepat, kualitas lebih baik, sistem lebih andal, dan proses lebih efisien.

Alat yang digunakan: Git, Jenkins, Docker, Kubernetes, dan lain-lain.

Intinya, DevOps membantu tim bekerja sama lebih baik dan menghasilkan produk yang lebih baik.

### 2. Apa yang anda ketahui tentang Infrastructure?

Infrastruktur Teknologi Informasi (IT) terdiri dari komponen dasar yang diperlukan untuk mengoperasikan dan mengelola layanan IT dalam sebuah organisasi. Komponen utamanya meliputi:

- Perangkat Keras (Hardware): Server, komputer, perangkat penyimpanan, dan perangkat jaringan.
- Perangkat Lunak (Software): Sistem operasi, aplikasi, dan middleware.
- Jaringan (Network): Internet, intranet, LAN, dan WAN.
- Fasilitas (Facilities): Data center, pasokan listrik, dan sistem pendingin.
- Keamanan (Security): Firewall, antivirus, dan protokol keamanan.
- Layanan dan Dukungan (Services and Support): Manajemen IT, layanan cloud, dan support desk.
- Virtualisasi dan Cloud Computing: Teknik virtualisasi dan penyediaan sumber daya melalui cloud.

Infrastruktur IT memastikan layanan IT berjalan lancar, efisien, dan aman, mendukung produktivitas dan pertumbuhan bisnis.

### 3. Apa yang anda ketahui tentang server, sebutkan implementasi berserta contohnya?

Server adalah komputer yang menyediakan layanan dan sumber daya kepada komputer lain dalam jaringan. Berikut beberapa jenis server dan contohnya:

- Web Server: Fungsinya Menghosting situs web. contoh: Apache, Nginx.
- Database Server: Fungsinya Menyimpan dan mengelola basis data. Contoh: MySQL, Oracle Database.
- Mail Server: Fungsinya Mengelola email. Contoh: Microsoft Exchange, Postfix.
- Application Server: Fungsinya Menjalankan aplikasi bisnis. Contoh: Apache Tomcat, IBM WebSphere.
- DNS Server: Fungsinya Menerjemahkan nama domain menjadi alamat IP. Contoh: BIND, Microsoft DNS.
- Virtualization Server: Fungsinya Menjalankan beberapa mesin virtual. Contoh: VMware ESXi, Microsoft Hyper-V.

### 4. Mengapa server dibutuhkan dalam pengembangan/development suatu software?

Server dibutuhkan dalam pengembangan software karena:

- Kolaborasi Tim: Memungkinkan banyak pengembang bekerja bersama.
- Versi Kontrol: Mengelola versi kode dan mencegah konflik.
- Lingkungan Pengujian: Menguji aplikasi sebelum dirilis.
- Deployment: Menjalankan aplikasi di server produksi.
- CI/CD: Mengotomatiskan build, testing, dan deployment.
- Manajemen Basis Data: Menyimpan dan mengelola data aplikasi.
- Keamanan: Melindungi kode dan data.
- Skalabilitas: Memastikan aplikasi tetap optimal dengan peningkatan pengguna.

Server mendukung efisiensi, keamanan, dan kualitas aplikasi dalam pengembangan software.

### 5. Apa yang anda ketahui mengenai Virtualisasi dan Container?

- Virtual Machine (VM)
  
Bayangkan sebuah komputer di dalam komputer. Itulah konsep dasar dari VM. Sebuah VM pada dasarnya adalah tiruan dari sistem komputer lengkap, termasuk sistem operasinya sendiri (misalnya, Windows, macOS, atau Linux), aplikasi, dan sumber daya virtual (CPU, RAM, penyimpanan). VM berjalan di atas perangkat keras fisik dan dikelola oleh sebuah perangkat lunak yang disebut hypervisor.

- Container

Berbeda dengan VM, container tidak meniru seluruh sistem komputer. Container hanya mengemas aplikasi dan semua dependensinya (pustaka, file konfigurasi, dll.) menjadi satu unit yang portabel dan ringan. Container berbagi kernel sistem operasi dari mesin host, sehingga lebih efisien dalam hal penggunaan sumber daya.


### 6.  Mengapa teknology container saat ini sangat populer?

Teknologi container populer karena:

- Portabilitas: Aplikasi dapat berjalan konsisten di berbagai lingkungan.
- Efisiensi: Container lebih ringan dan cepat daripada mesin virtual.
- Isolasi: Mencegah konflik antar aplikasi dan meningkatkan keamanan.
- Skalabilitas: Mudah di-scale up atau down sesuai kebutuhan.
- CI/CD: Mendukung otomatisasi build, testing, dan deployment.
- DevOps: Meningkatkan kolaborasi antara pengembang dan operasi.
- Ekosistem Kuat: Alat seperti Docker dan Kubernetes mendukung manajemen container.
- Penghematan Biaya: Mengurangi biaya infrastruktur dengan efisiensi tinggi.

Container memungkinkan pengembangan, deployment, dan pengelolaan aplikasi yang lebih cepat dan efisien.


### 7. Apa yang anda ketahui tentang Orchestration Container System?

Orchestration Container System adalah teknologi yang mengelola penyebaran, skala, dan operasi container secara otomatis di lingkungan produksi. Sistem ini memastikan bahwa aplikasi yang berjalan di container selalu tersedia, terukur, dan dikelola dengan baik. Fungsinya meliputi:

1. Deployment Otomatis: Memudahkan penyebaran aplikasi.
2. Scaling: Menambah atau mengurangi container sesuai kebutuhan.
3. Load Balancing: Mendistrisbusikan trafik ke container.
4. Self-Healing: Mengganti container yang gagal secara otomatis.
5. Resource Management: Mengoptimalkan penggunaan sumber daya.
6. Networking: Mengatur komunikasi antar container.
7. Security: Menerapkan kebijakan keamanan.

Contoh Sistem Orchestration:

- Kubernetes: Populer dan kuat, mengelola aplikasi container skala besar.
- Docker Swarm: Integrasi dengan Docker, mudah digunakan.
- Apache Mesos: Manajemen sumber daya skala besar.


## Task 1 (Virtualization)

- Buatlah sebuah VM dengan kententuan
  - username: `<github_user>` contoh `dimasm93`
  - hostname: `<email_without_at>` contoh `dimas.tabeldata.com`
  - OS: `ubuntu-20.04` atau `centos-7`
- Install webserver `nginx`
- Buatlah web profile temen-temen kemudian deploy ke webserver nginx tersebut yang telah di deploy
  
(kirimkan hasil screenshotnya simpan dalam folder `screenshot` dengan nama `task1.png`)

## Task 2 (Container)

Jika saya memiliki architecture seperti berikut:

![container-apps](docs/images/01-container.png)

Dimana berikut adalah configurasi docker image:

1. Backend container
  - image: `dimmaryanto93/udemy-springboot-app:latest`
  - port: `8080`
  - env: 
    - `DATABASE_HOST`: `<ip-domain-db>`
    - `DATABASE_PORT`: `5432` 
    - `DATABASE_NAME`: `<db-name>`
    - `DATABASE_PASSWORD`: `<db-password>`
    - `APPLICATION_PORT`: `8080`
  need:
    - Database PostgreSQL v14.2
2. Frontend container
  - image: `dimmaryanto93/udemy-angular-app:latest`
  - port: `80`
  - env:
    - `APPLICATION_PORT`: `80`
    - `NGINX_ROOT_DOCUMENT`: `/var/www/html`
    - `BACKEND_HOST`: `<ip-backend-apps>`
    - `BACKEND_PORT`: `<port-backend-apps>`
    - `BACKEND_CONTEXT_PATH`: `/`
  - need:
    - Backend container

Silahkan buat docker-compose filenya, kemudian simpan dalam folder `tasks` dengan nama `docker-compose.yaml`

