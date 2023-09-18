# Pinterest app clone
#### Proyecto Final FullStack - NUCBA

Este proyecto es el resultado de un esfuerzo conjunto como parte de un proyecto integrador de nuestra academia. Nuestro objetivo principal es aplicar y demostrar las habilidades y conocimientos que hemos adquirido a lo largo de nuestro programa de formación. Estoy emocionado de compartir esta aplicación con la comunidad y espero que encuentres inspiración y utilidad en ella.

PinterestAppClone es una aplicación inspirada en Pinterest que ofrece funcionalidades básicas similares a la plataforma original. Esta aplicación te permite explorar y guardar tus imágenes favoritas en tableros personalizados.

## 📌 Demo del proyecto
#### 🔗 Link:

👉 Cliente: https://pinterest-clone-frontend-git-main-matiasard.vercel.app/home

#### 🧑 Cuenta de prueba:

| email             | password  |
| :---------------- | :-------  | 
| `dante@gmail.com` | `1234`    |

## 📌 Screenshots
### ✨ Home:
![localhost_5173_home (1)](https://github.com/matiasard/pinterest/assets/60995996/a0433859-98fc-4a0d-a75a-5432b550f25c)

### ✨ Guardados:
![localhost_5173_home (1)](https://github.com/matiasard/pinterest/assets/60995996/77474f0d-eb77-4b55-82f8-16862e29650e)

---

## 📌 API Reference

```http base url server
https://pinterest-api.onrender.com
```

#### ➡ Registro de una nueva cuenta

```http
  POST /api/auth/register
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `user`  | `form-data` | Crea un nuevo usuario registrando una cuenta en la plataforma. |

#### ➡ Iniciar sesión

```http
  POST /api/auth/login
```

| Body      | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `User`    | `form-data` | Verifica si la cuenta del usuario existe y permite el inicio de sesión. |

#### ➡ Refrescar Token

```http
  POST /api/auth/refrestoken
```

| Body      | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `token`    | `string` | Verifica el token y proporciona un nuevo token. |

----


#### ➡ Obtener imágenes por usuario

```http
  GET /api/image/${id}
```

**Descripción:** Obtiene las imágenes pertenecientes a un usuario específico mediante su ID.

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `id`      | `number` | **Required**. ID del usuario para buscar y obtener sus imágenes. |


#### ➡ Guardar imagen

```http
  POST /api/image
```

| Body      | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `Image`   | `object` | Guarda la informacion de la imagen en la base de datos|


#### ➡ Eliminar imagen por ID

```http
  DELETE /api/image/${id}
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `id`      | `number` | **Required**. ID de la imagen que se desea eliminar. |



