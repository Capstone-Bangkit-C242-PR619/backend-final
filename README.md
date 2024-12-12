
# Project Title

A brief description of what this project does and who it's for


## API Reference

#### Get all items

```http
  POST /register
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `email` | `string` | **Required**.  |
| `password` | `string` | **Required**.  |
| `namalengkap` | `string` | **Required**.  |
| `tanggallahir` | `string` | **Required**. yyyy-mm-dd |
| `jeniskelamin` | `string` | **Required**.  |
| `alamat` | `string` | **Required**.  |
| `nomortelp` | `string` | **Required**. |

#### Get item

```http
  POST /uploadphoto
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `userPhoto`      | `form-data` | **Required**. foto user |
| `uid` | `string` | **Required**. uid diambil dari userCredential pakai getAuth() firebase |

```http
  POST /registerbayi
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `uid` | `string` | **Required**. uid diambil dari userCredential pakai getAuth() firebase |
| `namalengkapbayi`      | `string` | **Required**. nama bayi |
| `tanggallahirbayi`      | `string` | **Required**. yyyy-mm-dd |
| `jeniskelaminbayi`      | `string` | **Required**. jenis kelamin bayi |
| `tinggibadanbayi`      | `string` | **Required**. tinggi badan bayi dalam centimeter |
| `beratbadanbayi`      | `string` | **Required**. berat badan bayi dalam kilogram |
| `lingkarlenganbayi`      | `string` | **Required**. lingkar lengan dalam centimeter |

```http
  POST /home
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `uid` | `string` | **Required**. uid diambil dari userCredential pakai getAuth() firebase |

```http
  POST /updatestatusbayi
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `uid` | `string` | **Required**. uid diambil dari userCredential pakai getAuth() firebase |
| `namalengkapbayibaru`      | `string` | **Required**. nama bayi fixed aja user jangan dikasih akses ganti |
| `tanggallahirbayibaru`      | `string` | **Required**. yyyy-mm-dd |
| `tinggibadanbayibaru`      | `string` | **Required**. tinggi badan bayi yang baru dalam centimeter |
| `beratbadanbayibaru`      | `string` | **Required**. berat badan bayi yang baru dalam kilogram |
| `lingkarlenganbayibaru`      | `string` | **Required**. lingkar lengan yang baru dalam centimeter |


```http
  GET /article
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `-` | `-` |  `-`|

```http
  POST /article/{judulSlug}
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `judulSlug` | `string` | **Required**. diambil dari return article di page article|

```http
  POST /profile/{uid}
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `uid` | `string` | **Required**. uid diambil dari userCredential pakai getAuth() firebase |

```http
  POST /chatbot
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `message` | `string` | **Required**. pesan dari pengguna yang ingin disampaikan ke chatbot |