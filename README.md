Aplikasi Web Profile HTML

1. Docker Image

    Docker image merupakan template dasar untuk docker container. Image ini berisi sistem oeprasi ataupun aplikasi yang sudah selesai. Docker image ini berfungsi untuk menjalankan container.

2. Dockerfile

    Dockerfile merupakan script yang yang berisi dari serangkaian perintah yang akan dieksekusi secara otomatis dan berurutan untuk membuat sebuah image. 

Nah, penjelasan untuk script yang ada pada dockerfile :

    FROM nginx 
    MAINTAINER azisphanick azisp73@gmail.com
    ADD . /usr/share/nginx/html

![1.png](https://github.com/azisphanick/ResponsiTCCL/blob/master/1.png)


   Kemudian kita membuat direktori baru degan perintah yang digunakan mkdir responsiku, Setelah itu buat dan tambahkan file README.md kedalam direktori tersebut.
   
3. Membuat Image

![2.png](https://github.com/azisphanick/ResponsiTCCL/blob/master/2.png)

Perintah docker build -t responsiku ., digunakan untuk membuat images yang akan kita gunakan yaitu responsiku. Hasilnya dapt dilihat pada gambar diatas.

![3.png](https://github.com/azisphanick/ResponsiTCCL/blob/master/3.png)

Perintah docker run -p 8080:80 --name responsiku-1 responsiku, digunakan untuk menjalankan images responsi di localhost dengan port 80 yang namanya responsiku-1. 

4. Push Image ke Github

![5.png](https://github.com/azisphanick/ResponsiTCCL/blob/master/5.png)

Perintah diatas dgunakan untuk memindahkan projek dari lokal host ke github

5. Hasil
 
![4.png](https://github.com/azisphanick/ResponsiTCCL/blob/master/4.png)


Prestasi

    Github Contribution : https://github.com/jiharAkakom/fcm/graphs/contributors
