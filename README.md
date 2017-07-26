# RESPONSI TCCL
Dalam responsi ini saya membuat program HTML tentang web_event_seminar. Kemudian dijadikan docker image app web dengan nama saya sendiri. Berikut hasil dari web saya
![hasil.PNG](https://github.com/erwinrobbip/responsitccl/blob/master/img/hasil.png)

Menggunakan OS alpine dan menggunakan service nginx. Berikut isi file Dockerfile
```
FROM nginx:alpine
COPY . /usr/share/nginx/html/
EXPOSE 80
CMD ["nginx", "-g", "daemon off;"]
```
FROM : mendefenisikan base image Docker yang digunakan, dalam contoh ini menggunakan nginx:alpine

COPY melakukan proses duplikasi semua file yang ditandai titik(.) pada direktori responsi ke dalam root direktori html nginx di dalam container

EXPOSE : Mendefenisikan port yang digunakan

CMD : Eksekusi perintah command pada lingkungan container

**build images**
![sudo%20docker%20build.png](https://github.com/erwinrobbip/responsitccl/blob/master/img/sudo%20docker%20build.png)
```
sudo docker build -t nginx-erwinrobbip:v2 .
```
perintah sudo digunakan untuk akses ke root kemudian dilanjutkan dengan docker build. -t menunjukan tag list dan diikuti nama image yang kita inginkan. v2 terakhir menunjukan versi dari image yg kita bangun. Kemudian ada tanda . yang diartikan all file in folder.

**jalankan image yang kita bangun**
![uocker%20run%20-d%20-p.png](https://github.com/erwinrobbip/responsitccl/blob/master/img/docker%20run%20-d%20-p.png)
perintah diatas docker menjalankan -d diartikan sebagai menjalankan container dalam background dan mencetak ID container kemudian dilanjutkan -p yakni port yang digunakan kemudinan images yang akan dijalankan

**cek images**
![uocker%20run%20-d%20-p.png](https://github.com/erwinrobbip/responsitccl/blob/master/img/docker%20run%20-d%20-p.png)
```
sudo docker images
```

**cek container**
![Screenshot%20from%202017-07-26%2022-06-01.png](https://github.com/erwinrobbip/responsitccl/blob/master/img/Screenshot%20from%202017-07-26%2022-06-01.png)
container ID tercipta setelah kita run images. disebelah juga tertulis images nginx-erwinrobbip:v2 sesuai image yang kita bangun



**Prestasi:**
 1. Github Star Project : https://github.com/erwinrobbip/captiveportal_mikrotik
 2. Collabolator: https://github.com/amanuDigm/kolaborasi-tccl
