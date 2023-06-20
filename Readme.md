# Docker Files Key Words

- **ARG** digunakan untuk menentukan variabel yang dapat dilewati saat build-time. Anda juga dapat menentukan nilai default.


- **FROM** ialah image dasar untuk membangun image baru. Instruksi ini harus menjadi instruksi non-comment pertama di Dockerfile. Satu-satunya pengecualian dari aturan ini adalah ketika Anda ingin menggunakan variabel dalam argumen FROM. Dalam hal ini FROM dapat didahului dengan satu atau lebih instruksi ARG.


- **LABEL** digunakan untuk menambahkan metadata ke image, seperti deskripsi, versi, author dll. Anda dapat menentukan lebih dari satu LABEL dan setiap instruksi LABEL adalah key-value pair.


- **RUN** ialah perintah yang ditentukan dalam instruksi ini akan dieksekusi selama proses build. Setiap instruksi RUN membuat layer baru di atas image saat ini.


- **ADD** digunakan untuk menyalin file dan direktori dari sumber yang ditentukan ke tujuan yang ditentukan pada image docker. Sumbernya dapat berupa file atau direktori lokal atau URL


- **COPY** sama saja dengan ADD tetapi sumbernya hanya berupa file atau direktori lokal.


- **ENV** ialah instruksi ini memungkinkan Anda untuk mendefinisikan environment variable.


- **CMD** digunakan untuk menentukan perintah yang akan dieksekusi ketika Anda menjalankan sebuah container. Anda hanya dapat menggunakan satu instruksi CMD di Dockerfile Anda.


- **ENTRYPOINT** sama saja dengan CMD, instruksi ini mendefinisikan perintah apa yang akan dieksekusi ketika menjalankan sebuah container.


- **WORKDIR** directive ini menetapkan direktori kerja saat ini untuk instruksi RUN, CMD, ENTRYPOINT, COPY, dan ADD berikut.


- **USER** , Tetapkan nama user atau UID untuk digunakan ketika menjalankan instruksi RUN, CMD, ENTRYPOINT, COPY dan ADD.


- **VOLUME**, Memungkinkan Anda untuk memasang direktori mesin host ke container.


- **EXPOSE**, Digunakan untuk menentukan port tempat Container mendengarkan saat runtime.
