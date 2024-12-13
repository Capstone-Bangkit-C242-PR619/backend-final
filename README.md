
# Project Title

This backend is built with the node.js Hapi framework by dividing its files into several parts with their respective tasks.
Below are how to connect to the backend API with their requirement parameters

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
| `nomortelp` | `integer` | **Required**. |

#### Get item

```http
  POST /uploadphoto
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `userPhoto`      | `form-data` | **Required**. foto user |
| `uid` | `string` | **Required**. Take UID from token |

```http
  POST /registerbayi
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `uid` | `string` | **Required**. Take UID from token |
| `namalengkapbayi`      | `string` | **Required**. |
| `tanggallahirbayi`      | `string` | **Required**. yyyy-mm-dd |
| `jeniskelaminbayi`      | `string` | **Required**. |
| `tinggibadanbayi`      | `integer` | **Required**. in centimeter |
| `beratbadanbayi`      | `integer` | **Required**. in kilogram |
| `lingkarlenganbayi`      | `integer` | **Required**. in centimeter |

```http
  POST /home
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `uid` | `string` | **Required**. Take UID from token |

```http
  POST /updatestatusbayi
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `uid` | `string` | **Required**. Take UID from token |
| `namalengkapbayibaru`      | `string` | **Required**. nama bayi fixed aja user jangan dikasih akses ganti |
| `tanggallahirbayibaru`      | `string` | **Required**. yyyy-mm-dd |
| `tinggibadanbayibaru`      | `integer` | **Required**. in centimeter |
| `beratbadanbayibaru`      | `integer` | **Required**. in kilogram |
| `lingkarlenganbayibaru`      | `integer` | **Required**. in centimeter |


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
| `judulSlug` | `string` | **Required**. |

```http
  POST /profile/{uid}
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `uid` | `string` | **Required**.  |

```http
  POST /chatbot
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `message` | `string` | **Required**.  |