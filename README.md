# DOSW_ParcialT1_Miguel_Sandoval

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
