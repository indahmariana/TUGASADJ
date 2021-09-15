# TUGASADJ
Pada tugas ini saya mengembangkan sebuah Website Static Sederhana menggunakan HTML CSS dengan Docker dan Nginx, berikut laporan langka-langkahnya :
Langkah pertama : Menginstall Docker Desktop di https://docs.docker.com/
Langkah kedua : Membuat Folder untuk file HTML, CSS serta file yang dibutuhkan.
Langkah ketiga : Membuat satu file dengan nama Dockerfile dimana file ini akan kita buat didalam satu folder dengan file HTML dan CSS.
![1](https://user-images.githubusercontent.com/73211222/133446821-ab13c189-6e79-4801-bf76-1181ba75525c.jpg)

Langkah keempat : Mengisi file Docker dengan
![2](https://user-images.githubusercontent.com/73211222/133446834-23177bda-a8ac-4158-8754-787544834c0b.jpg)
Penjelasan tentang isi file Docker :
-	Pada baris pertama terdapat comman FROM, ini akan menarik nginx:alpine image ke mesin lokal dan kemudian mengembangkan custo kita diatasnya.
-	Pada baris kedua terdapat comman COPY , disini kita menyalin file index.html ke directory /usr/share/nginx/html didalam container yang menimpa index.html default yang disediakan nginx:alpine image.
-	Pada baris keempat terdapat comman LABEL,  Digunakan untuk menambahkan metadata ke image, seperti deskripsi, versi, author dll. Anda dapat menentukan lebih dari satu LABEL dan setiap instruksi LABEL adalah key-value pair.

Langkah kelima : Build images, dengan cara membuka terminal lalu ketik seperti dibawah ini :
docker build -t html-indah-mariana:v1 .
![3](https://user-images.githubusercontent.com/73211222/133446842-86fa3494-e5db-410b-8bb7-7d38b8894b74.jpg)

Langkah keenam : Setelah membuat images, kita cek terlebih dahulu seperti dibawah ini
![4](https://user-images.githubusercontent.com/73211222/133446849-0a5caad7-5a15-4c1b-8d8f-20a0274208f6.jpg)
Akan terlihat images apa saja yang sudah kita buat

Langkah ketuju : Membuat personal access token di github
![5](https://user-images.githubusercontent.com/73211222/133446854-8f9be415-9120-4e39-a33e-034ffb5181ce.jpg)
Lalu login, seperti dibawah ini :
![6](https://user-images.githubusercontent.com/73211222/133446856-379b99f7-5b55-4755-8d45-75a96da32ab2.jpg)

Langkah kedepalan : Build images kedua
![7](https://user-images.githubusercontent.com/73211222/133446863-ac91ca1f-57e8-43ca-bf7a-557757b22581.jpg)

Langkah kesembilan : Mengecek images, lalu menyalin ID image yang kedua
![8](https://user-images.githubusercontent.com/73211222/133446868-432b8707-24fb-4f6d-bd7d-892c0b0afcf7.jpg
![9](https://user-images.githubusercontent.com/73211222/133446876-4a42bdb9-4817-4d75-a5af-3f95832670d4.jpg)

Langkah kesepuluh : Memberikan tag di image
![10](https://user-images.githubusercontent.com/73211222/133446879-1a870dd0-aa60-4ef6-be7a-3644e7b8bfb7.jpg)

Langkah kesebelas : Push image
![11](https://user-images.githubusercontent.com/73211222/133446885-d29ffad0-b60a-4430-ba87-19701f7484bf.jpg)

Langkah keduabelas : Mengecek packages di github
![12](https://user-images.githubusercontent.com/73211222/133446896-3bb27cd5-fef5-4256-86a2-2927103135bc.jpg)

Langkah ketigabelas : Run Docker untuk melihat hasil
![13](https://user-images.githubusercontent.com/73211222/133446906-a446890b-2019-4912-ba16-344a6c460cd9.jpg)

Buka localhost:80
![14](https://user-images.githubusercontent.com/73211222/133446917-d7431b00-e9ab-4c25-833f-ab76dcd77ee9.jpg)

Tampilan Docker images
![15](https://user-images.githubusercontent.com/73211222/133446921-1cf5673b-96ea-44b7-9e19-db86279697d9.jpg)

![16](https://user-images.githubusercontent.com/73211222/133446925-ad5d1201-7740-4537-93e3-6380dde2e6f9.jpg)
