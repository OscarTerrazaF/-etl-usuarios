# 🚀 Proyecto ETL de Usuarios – Simulación práctica para Data Engineering

Este proyecto implementa un pipeline ETL real usando Python y SQLite, aplicado a un dataset desordenado de usuarios. Fue realizado como parte de mi camino de formación práctica para convertirme en Data Engineer.

---

## 🔧 Tecnologías utilizadas

- **Python 3**
- **Pandas**
- **SQLAlchemy**
- **SQLite** (y DB Browser para visualización)

---

## 🧠 Qué hace este pipeline

✔️ Lee datos desordenados desde un archivo `.csv`  
✔️ Limpia nombres, valida emails, normaliza fechas  
✔️ Convierte campos booleanos escritos de forma inconsistente  
✔️ Descarta registros inválidos  
✔️ Carga los datos limpios en una base relacional  
✔️ Ejecuta una consulta de verificación final

---

## 🧪 Dataset original

`usuarios_registrados.csv` contiene errores comunes en bases reales:
- Formatos mixtos de fechas
- Emails inválidos o faltantes
- Mayúsculas y espacios desordenados
- Campos booleanos tipo: `sí`, `SI`, `no`, `false`

---

## 📁 Estructura del proyecto
📦 etl-usuarios
┣ 📄 etl_usuarios.py
┣ 📄 usuarios_registrados.csv
┣ 📄 usuarios.db
┗ 📄 README.md
