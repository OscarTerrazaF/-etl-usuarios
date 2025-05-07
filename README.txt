TAREA SIMULACRO - ETL DE USUARIOS

Objetivo:
Construir un pipeline ETL que limpie y cargue datos de usuarios registrados.

Pasos:
1. Extract:
   - Leer el archivo usuarios_registrados.csv

2. Transform:
   - Limpiar 'nombre_completo': quitar espacios y convertir a minúsculas.
   - Validar 'email': eliminar filas sin email válido (que contenga "@" y ".")
   - Estandarizar 'fecha_registro' a formato YYYY-MM-DD. Si es inválida o vacía, dejar nulo.
   - Establecer 'activo' como booleano: sí, SI, Sí = True; no, false = False

3. Load:
   - Cargar los datos limpios a una base SQLite llamada usuarios.db
   - La tabla debe llamarse 'usuarios_limpios' con el siguiente esquema:
     id_usuario (int), nombre (text), email (text), fecha_registro (text), activo (boolean)

4. Verificación:
   - Hacer un SELECT * FROM usuarios_limpios
   - Hacer un SELECT COUNT(*) WHERE activo = TRUE
