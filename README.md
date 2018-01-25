# cobaalpine-alpine
Membangun Image Manual (Pastikan sudah memiliki alpine versi terbaru)

Link Dockerhub : https://hub.docker.com/r/dioob/cobaalpine-alpine/

Membangun Image Manual (Pastikan sudah memiliki alpine versi terbaru)

Buka dengan perintah : docker run -it alpine /bin/sh
.
Saya hanya ingin membuat file:
/ # echo "Two plus two is four, minus one is three QUICK MATHS!" > cobaalpine

Cek nama container nya :
aeb20c0dcafc alpine "/bin/sh" 2 minutes ago Exited (0) 6 seconds ago nostalgic_swartz

Buat image baru dari container nostalgic_swartz :
$ docker commit -m "punyaku, punyaku, punyaku" nostalgic_swartz cobaalpine-alpine
sha256:6adb660101310b6205b9294ed4b80dd48e494ad842049fe90b6bc97450e2cbb8

Lalu saya PUSH image yang saya buat manual tadi.

Cara RUN :
$ docker run -it cobaalpine-alpine /bin/sh

Lalu ketik :
/ # cat cobaalpine
