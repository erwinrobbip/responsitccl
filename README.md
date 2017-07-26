# RESPONSI TCCL
Dalam responsi ini saya membuat program HTML tentang web_event_seminar. Kemudian dijadikan docker image app web dengan nama saya sendiri. Berikut hasil dari web saya
![hasil.PNG](https://github.com/erwinrobbip/responsitccl/blob/master/img/hasil.png)

Menggunakan OS alpine dan menggunakan service nginx. Berikut isi file Dockerfile
```FROM nginx:alpine
COPY . /usr/share/nginx/html/
EXPOSE 80
CMD ["nginx", "-g", "daemon off;"]
```
FROM : mendefenisikan base image Docker yang digunakan, dalam contoh ini menggunakan nginx:alpine
COPY melakukan proses duplikasi file index.html pada direktori imageku ke dalam root direktori nginx di dalam container
EXPOSE : Mendefenisikan port yang digunakan
CMD : Eksekusi perintah command pada lingkungan container



untuk responsi tccl nanti malam:
1. buat aplikasi web yang menampilkan tampilan HTML bebas. devel tools bebas, boleh php, nodejs, java, dll.
2. buat Dockerfile untuk membuat image app web tsb
3. push no 1 dan 2 ke repo github anda, beri nama repo anda: "responsitccl".
4. jelaskan apa yg sudah anda kerjakan tsb dlm file README.md. File ini jg hrs masuk ke repo.
5. tuliskan karya serta prestasi anda di readme tsb (trmsk github project dgn star > 25, kontrib proyek open source, dll).
6. setelah selesai, kirim nama, nim, username github ke grup ini. 



oke

blablalba
]asdf
ds
f
adsf 
d
fd
![unifi1.PNG](https://github.com/erwinrobbip/responsitccl/blob/master/unifi1.PNG)
