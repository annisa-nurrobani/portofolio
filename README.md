## Prerequisites
- Install Visual Studio Code https://code.visualstudio.com/
- Install GitHub Desktop https://desktop.github.com/
- Read Tailwind Documentation https://tailwindcss.com/docs/installation
- Install Visual Studio Code Extension:
  - Live Server
  - Live Preview
  - Tailwind CSS IntelliSense

## Step
1. Ikuti prerequisites
2. Buka GitHub Desktop dan clone repository ini dengan menyalin link repository ini

  ![image](https://user-images.githubusercontent.com/55025382/209630235-18e86ab4-18c7-4a23-9d20-aac7c3ba1d22.png)

> Clone dapat juga dilakukan dengan klik "Open with GitHub Desktop" di repository ini
  ![image](https://user-images.githubusercontent.com/55025382/209628490-a4786f7c-4461-4362-aefd-619cb24f656b.png)

3. Pada GitHub Desktop, pilih repository yang sudah di clone dan buka VS Code dengan klik "Open in Visual Studio Code"
  ![image](https://user-images.githubusercontent.com/55025382/209627206-82dbc8ee-5b5a-479b-81e8-91bc10d23bcd.png)

4. Copy dan masukkan kode berikut ke terminal VS Code
```
npm init -y
npm install -D tailwindcss
npx tailwindcss init
```

5. Agar Tailwind dapat memantau setiap perubahan, masukkan kode berikut di terminal VS Code
```
npx tailwindcss -i ./src/input.css -o ./dist/output.css --watch
```
  ![image](https://user-images.githubusercontent.com/55025382/209627964-743af6aa-f7c7-447c-bb9e-a6c77ad93286.png)
  > Selalu jalankan kode tersebut sebelum mengedit apapun

6. Edit
> Untuk melihat sementara perubahan yang dilakukan dapat dilakukan dengan klik kanan file HTML dan pilih "Show Preview"
  ![image](https://user-images.githubusercontent.com/55025382/209632007-3553e4f6-31c3-4a8f-b3c0-aa6070075ad2.png)

7. Setelah melakukan perubahan apapun, jangan lupa untuk save dengan ```Ctrl + S``` dan Commit ke GitHub
8. Commit dapat dilakukan dengan membuka GitHub Desktop, pastikan telah berada di repository yang telah diedit dan akan muncul tampilan kode yang telah berubah, klik "Commit to main" untuk melakukan Commit

![image](https://user-images.githubusercontent.com/55025382/209629658-51519a29-fa81-4a79-9039-489b23f21e72.png)

9. Kemudian klik "Push Origin"
  ![image](https://user-images.githubusercontent.com/55025382/209629791-c5e05773-d22b-427f-88d6-65c1148eaabc.png)


## Struktur File
- dist
  - ```img``` Tempat menaruh seluruh gambar
    - ```clients``` Tempat menaruh gambar clients (saat ini tidak ditampilkan)
    - ```portofolio``` Tempat menaruh gambar portofolio
    - ```hero.png``` Foto landing page
  - ```js``` Tempat JavaScript
    - ```script.js``` Jangan diubah
  - ```video``` Tempat menaruh video
    - project-one.mp4
    - project-two.mp4
  - ```output.css``` Tailwind thing, jangan disentuh atau diubah
- ```node_modules``` Generated, jangan diubah
- ```portofolio``` Tempat menaruh halaman secondary
  - ```narrated.html``` Halaman individual untuk video Narrated (Dapat diubah)
  - ```ndandani.html``` Halaman individual untuk video Ndandani (Dapat diubah)
- src
  - ```input.css``` Bypass some Tailwind style, jangan diubah kalau gatau
- ```.gitignore``` Ignore this
- ```index.html``` Halaman utama yang dapat diubah
- package-lock.json
- package.json
- tailwind.config.js

## Ubah Mengubah
File yang dapat diubah adalah `index.html`, `narrated.html`, dan `ndandani.html`

Jika ingin menambahkan halaman video, silakan copy salah satu file html di `portofolio` dan paste di folder itu juga (jangan lupa ganti namanya sesuai judul video). Selanjutnya buka `index.html` dan copy line ke `276` hingga `285` dan paste dibawah line `295`. Tinggal edit nama, foto thumbnail, dan linknya.

Jika ingin menambahkan foto, silakan buka `index.html` dan copy line ke `221` hingga `227` dan paste dibawah line `227`. Ubah link foto, judul, dan deskripsi. Jangan lupa masukan gambar ke folder `img > portofolio`.

Ikutin aja formatnya kaya yang diatasnya, pasti bisa
