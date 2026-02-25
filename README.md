# DOSW_ParcialT1_Miguel_Sandoval

# Punto 1
---
## Diagrama de cotexto

<img width="510" height="338" alt="diagrama de contexto" src="https://github.com/user-attachments/assets/608a5c0a-4521-4cc6-9d43-f190793dcc8b" />

---

# Punto 2 
---
## Patrones de diseño

# Primer patron

- A) Factory method
- B) Patron creacional
- C) justificacion: podria usarse ya que se debe crear distintos tipos de reservas dependiendo del recurso y eso permite que este patron centralice la creacion de objetos

# Segundo patron

- A) Strategy 
- B) Patron de Comportamiento 
- C) justificacion: podriamos usar este patron ya que hay diferentes tipos de recursos ya sean salones, oficinas o salas de estudio y cada una tiene sus reglas como de validacion para su respectiva reserva y este patron podria evitar muchos if/else por si sea agrega nas recursos.

# Punto 3
- Requerimientos Funcionales:
  
- RF1-CREAR RESERVAS
- El sistema debe permitir a los usuarios crear una reserva indicando el tipo de recurso, fecha, hora, duracion y demas datos que requieran segun el recurso ( este requerimeinto esta asociado al patron de factory method )

---
  
- RF2-VALIDAR REGLAS DE RESERVA
- El sistema debe validar que las reserva cumpla con todas las reglas definidas para el tipo de recurso, como tipo de usuario, tiempo maximo y su capacidad.

---

- RF3-CONFIRMAR O RECHAZAR RESERVA
- El sistema debe confirmar o denegar la reserva dependiendo del resultado de las validaciones, informando al usuario el resultado

---
- Requerimientos NO Funcionales:
  
- RNF1-DISEÑO VISUAL
- El sistema debe mantener los colores representativos del programa de ingenieria de sistemas y utilizar una tipografia legible

---

- RNF2-INTERFAZ RESPONSIVE
- El sistema debe ser responsive, permitiendo su uso en diferentes dispositivios (computadores, tabletas y moveiles)

# Punto 4
- Los requerimientos que escogi son RF1 y RF2

- DIAGRAMA:

  <img width="531" height="457" alt="Screenshot 2026-02-25 175114" src="https://github.com/user-attachments/assets/ce8fe424-31dc-4c6d-a949-48f5fdd92899" />

- Historias de uso:
  1. Como usuario quiero crear una reserva de un recurso para poder utulizarlo en un hoario especifico
  2. Como sistema quiero validar la reserva segun las reglas del recurso para poder asegurar que cumple con las condiciones
  3. Como usuario quiero consultar la disponibilidad para poder realizar una reserva
  4. Como sistema quiero consultar el tipo de reserva para ver si cumple con las reglas y poder validar o cancelar

# Punto 5
- esta en docs

# Punto 6
- Requerimiento RF1 Crear una reserva
- EPICA:
- Permitir a los usuarios crear reservas de diferentes tipos de recursos cumpliendo las reglas definidas por el sistema

--- 

- Historias de uso
- HU
- Como usuario quiero crear una reserva de un recurso para poder utilizarlo en una fecha y hora especifica

--- 

- Tareas:
1.
- Crer clase base (Resera)
- Definir atributos comunes(fecha, hora, duracion, capacidad)
- definir clases hijas:
- reserva salon o oficina o de estudio y equipo
  
2. 
- Implementacion del patron de diseño factory method
- implemetar un metodo para crear reservas segun su tipo de recurso
  
3.
- integrar la validacion con la cracion
- enviar la reserva creada al modulo de validacion
- preparar la estructura para manejar la respuesta
  
