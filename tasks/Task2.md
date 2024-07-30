# Container 

## Instalasi Docker

buat bash script berikut untuk melakukan instalasi docker 

```
#!/bin/bash

# Cek apakah skrip dijalankan sebagai root
if [[ $EUID -ne 0 ]]; then
   echo "Skrip harus dijalankan sebagai root atau dengan sudo."
   exit 1
fi

# Update paket dan instal dependensi
apt-get update
apt-get install -y apt-transport-https ca-certificates curl software-properties-common

# Tambahkan kunci GPG resmi Docker
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /usr/share/keyrings/docker-archive-keyring.gpg

# Tambahkan repositori Docker
echo "deb [signed-by=/usr/share/keyrings/docker-archive-keyring.gpg] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null

# Instal Docker
apt-get update
apt-get install -y docker-ce docker-ce-cli containerd.io

# Tambahkan pengguna saat ini ke grup docker (agar tidak perlu sudo untuk menjalankan Docker)
sudo usermod -aG docker $USER

echo "Instalasi Docker selesai. Silakan logout dan login kembali untuk menerapkan perubahan."
```

tambahkan perizinan agar script dapat di eksekusi
```
sudo chmod +x install_docker.sh
```

dan eksekusi script dengan memasukkan perintah
```
./install_docker.sh
```
![image](https://github.com/user-attachments/assets/4a3186a3-15b9-4f1e-85b6-1bbfe4cfda1e)

## Docker Compose

```
sudo nano docker-compose.yaml
```

```
services:
  db:
    image: postgres:14.2
    ports:
      - "5432:5432"
    environment:
      POSTGRES_DB: postgres
      POSTGRES_USER: postgres
      POSTGRES_PASSWORD: irwan123

  backend:
    image: dimmaryanto93/udemy-springboot-app:latest
    ports:
      - "8080:8080"
    environment:
      DATABASE_HOST: db
      DATABASE_PORT: 5432
      DATABASE_NAME: postgres
      DATABASE_USERNAME: postgres
      DATABASE_PASSWORD: irwan123
      APPLICATION_PORT: 8080
    depends_on:
      - db

  frontend:
    image: dimmaryanto93/udemy-angular-app:latest
    ports:
      - "88:80"
    environment:
      APPLICATION_PORT: 80
      NGINX_ROOT_DOCUMENT: /var/www/html
      BACKEND_HOST: backend
      BACKEND_PORT: 8080
      BACKEND_CONTEXT_PATH: /
    depends_on:
      - backend
```

jalankan docker-composenya dengan memasukkan perintah
```
docker compose up -d
```

![image](https://github.com/user-attachments/assets/9e75b1c7-cf9f-4c7b-aa19-5825c468d9dc)
