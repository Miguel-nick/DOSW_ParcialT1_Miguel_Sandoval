# 📄 Requerimientos del Sistema

## 1. Lista general de requerimientos

El sistema de SILABINFO tiene los siguientes requerimientos (descripción a alto nivel):

### 1.1 Requerimientos funcionales

El sistema de SILABINFO debe tener la capacidad de:

- 1.CREAR RESERVAS
- El sistema debe permitir a los usuarios crear una reserva indicando el tipo de recurso, fecha, hora, duracion y demas datos que requieran segun el recurso ( este requerimeinto esta asociado al patron de factory method )
- 2.VALIDAR REGLAS DE RESERVA
- El sistema debe validar que las reserva cumpla con todas las reglas definidas para el tipo de recurso, como tipo de usuario, tiempo maximo y su capacidad.
- 3.CONFIRMAR O RECHAZAR RESERVA
- El sistema debe confirmar o denegar la reserva dependiendo del resultado de las validaciones, informando al usuario el resultado


### 1.2 Requerimientos NO funcionales

El sistema de SILABINFO debe tener:

1.DISEÑO VISUAL
2.INTERFAZ RESPONSIVE

## 2. Diagramas de caso de uso

<img width="531" height="457" alt="Screenshot 2026-02-25 175114" src="https://github.com/user-attachments/assets/9663c2a5-58cf-47b0-a11e-e0fab5af28ca" />


### 2.1 Requerimiento Funcional 1

| Campo | Descripción |
|------|-------------|
| **ID** | RF-01 |
| **Nombre del requerimiento** |*CREAR RESERVAS* |
| **Descripción** | *El sistema debe permitir a los usuarios crear una reserva indicando el tipo de recurso, fecha, hora, duracion y demas datos que requieran segun el recurso ( este requerimeinto esta asociado al patron de factory method )* |
| **Precondiciones** | *Para que el sistema cumpla con este requerimiento, SILABINFO debe tener previamente el usuario debe estar autentificado en el sistema y el sitema debe tener disponibles os recursos a reservar * |
| **Actor** | *usuario(monitor)* |
| **Flujo principal** | 1. El actor debe poder crea una reserva<br>2. El sistema le debe permirmitir crear una reservera si cumple con los requerimientos dados<br>3. El sistema crea la reserva|
| **Diagrama de caso de uso** | *<img width="498" height="135" alt="Screenshot 2026-02-25 181009" src="https://github.com/user-attachments/assets/22202d1a-09d7-4b65-b086-2876700447ba" />*|
| **Poscondiciones** | *Se espera como resultado que el usuario pueda crear sin problemas la reserva* |


### 2.2 Requerimiento Funcional 2

| Campo | Descripción |
|------|-------------|
| **ID** | RF-02 |
| **Nombre del requerimiento** |*VALIDAR REGLAS DE RESERVA* |
| **Descripción** | *El sistema debe validar que las reserva cumpla con todas las reglas definidas para el tipo de recurso, como tipo de usuario, tiempo maximo y su capacidad.* |
| **Precondiciones** | *Para que el sistema cumpla con este requerimiento, SILABINFO debe tener previamente debe existir una solicitud de reserva previamente creada con todos los datos requeridos* |
| **Actor** | *SILABINFO(administrados de silabinfo)* |
| **Flujo principal** | 1. El actor debe mirar si hay reservas pendientes <br>2. El sistema mirar si cumple con los requerimientos dados por l usuario<br>3. El sistema valida o no la reserva|
| **Diagrama de caso de uso** | *<img width="540" height="117" alt="Screenshot 2026-02-25 181443" src="https://github.com/user-attachments/assets/8518a25f-bad4-4db9-992a-1df309d3220b" />*|
| **Poscondiciones** | *Se espera como resultado que el sistema pueda tanto validar la reserva o dar una retroalimentacion del porque no se pudo realizar* |




