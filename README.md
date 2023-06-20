# Day 5 - Backend

## API

Extension Visual Studio Code:

__Thunder Client__

---
## RESTful API

1. Uniform Interfaces: The API has a consistent and standardized way of interacting with resources.
2. Stateless
3. Client-Server Architecture
4. Cacheable

| test | API Link | Description |
| ---- | -------- | ----------- |
| GET | http://localhost/movies | List of all movies |
| GET | http://localhost/movies/1 | View a movie |
| POST | http://localhost/movies -> request body | Add a new movie |
| PATCH | http://localhost/movies -> request body | Update a movie |
| DELETE | http://localhost/movies/1 | Delete a movie |

---

## Build API

[Klik untuk Link API](https://github.com/Cizz22/Genics-API)

> Fork dulu repository Genics API-nya, kalau sudah, ikuti step yang ada di README.md nya. Jangan lupa buat Database dulu di MongoDB.

Step membuat database baru di [MongoDB](https://cloud.mongodb.com):
1. Buka homepagenya MongoDB.
2. Ke bagian Database, terus klik Create
3. Kalau ngga salah pilih yang __Dedicated__, terus pilih Cloud Provider & Regionnya __aws__ dan __Jakarta (ap-southeast-3)__, yang lain biarin default. Terus klik Create Cluster
4. Kalau sudah buat, klik __Connect__ di Database yang baru.
5. Isi dulu username dan password yang diinginkan. Terus next. Pilih Drivers, terus next. Settingannya biarin default aja, trus copy link yang ada di point ke 3. Terus di VSCode, buat file dengan nama __".env"__ _(engga perlu nama file kyk biasa kita buat file baru)_.
6. Isi file .env dengan code berikut
    ```
    MONGO_DB = <link tadi>
    PORT = 5000
    ```
7. Lalu buka file __package.json__, tambahin di bagian _script_
    ```
    "start": "node index.js"
    ```
8. Terus buka terminal, ketik
    ```
    npm install
    ```
    Setelah selesai proses, ketik
    ```
    npm start
    ```
    __JANGAN LUPA INSTALL NODE.JS DULU YAA!__

Kalau mau lihat hasil coding tadi pas pertemuan, bisa buka GitHubku di [sini](https://github.com/rigelra15/Genics-API.git), tinggal lihat perbedaan list syntax code-nya.