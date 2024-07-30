# Virtualization

## Membuat Sebuah VM

### 1. Mengenerate VM Melalui Microsoft Azure

pada tahap ini kita membuat vm berdasarkan spesifikasi yang kita perlukan dan mengisi data-data seperti username, hostname, OS, dll

![image](https://github.com/user-attachments/assets/3c0a9f3a-d65b-44c0-af71-bbb30e7ae308)


- Hostnamenya ```irwanpanai.gmail.com```
- Usernamenya ```irwanpanai```
- menggunakan OS Ubuntu 20.04

![image](https://github.com/user-attachments/assets/cc03e9ea-7349-40a2-9524-9217cfb5b149)


### 2. Menginstal Webserver Nginx

sebelum menginstall webserver nginx kita melakukan update repositori terlebih dahulu dengan memasukkan perintah
```
sudo apt update
```
```
sudo apt upgrade
```

setelah melakukan update kita melakukan install webserver nginx dengan memasukkan perintah
```
sudo apt install nginx
```

setelah terinstall kita pastikan nginxnya sudah berjalan dengan memasukkan perintah
```
sudo systemctl status nginx
```

Jika Nginx tidak berjalan, gunakan perintah berikut untuk memulai:
```
sudo systemctl start nginx
```

![image](https://github.com/user-attachments/assets/485db00b-f65d-452f-81c3-95faa49b0700)

### 3. membuat webserver profile dan deploy ke webserver nginx

masuk ke direktori ```/var/www/html``` lalu edit ```index.nginx-debian.html```

```
sudo nano index.nginx-debian.html
```
```
<!DOCTYPE html>
<html>
<head>
<title>Profil Irwan</title>
<style>
    body {
        width: 35em;
        margin: 0 auto;
        font-family: Tahoma, Verdana, Arial, sans-serif;
    }
</style>
</head>
<body>
<h1>Irwansyah Idris Panai</h1>
<p>I am a graduate with a Bachelor's degree in Physics from Gorontalo State University.
My academic background has equipped me with a strong foundation in analytical thinking and
 problem-solving. Recently, I successfully completed a bootcamp program, specializing
 in DevOps engineering. This intensive program has enhanced my skills in deploying and
 managing infrastructure, automating workflows, and ensuring seamless collaboration between
 development and operations teams. I am enthusiastic about applying my academic knowledge
 and practical experience to contribute effectively in a dynamic and challenging work environment.
 My dedication to continuous learning and passion for technology align well with the evolving
 landscape of DevOps practices.</p>
</body>
</html>
```

![image](https://github.com/user-attachments/assets/93d34e2f-edd6-49b3-b549-15e336a25aa5)

![image](https://github.com/user-attachments/assets/610c7ccd-2aae-4746-8d28-d7054b799cba)
