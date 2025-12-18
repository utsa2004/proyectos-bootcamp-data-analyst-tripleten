# 📚 Proyecto 14.2 – Análisis SQL para Producto Literario Digital  
**Bootcamp de Data Analytics – TripleTen**

---

## 📌 Descripción del proyecto

Durante la pandemia de COVID-19, los hábitos de consumo cambiaron significativamente y la lectura digital se convirtió en una de las principales actividades de entretenimiento en casa. Este contexto impulsó el crecimiento de startups enfocadas en productos literarios digitales, como plataformas de lectura, recomendación y reseñas de libros.

En este proyecto se analiza la base de datos de un servicio literario digital que contiene información sobre **libros, autores, editoriales, calificaciones y reseñas de usuarios**, con el objetivo de generar insights que ayuden a diseñar un nuevo producto orientado a lectores.

El análisis se realiza **exclusivamente mediante consultas SQL**, utilizando Python únicamente como intermediario para ejecutar las consultas y presentar los resultados.

---

## 🎯 Objetivo del proyecto

Analizar el ecosistema editorial digital para identificar patrones relevantes que permitan:

- Comprender la producción editorial y su evolución en el tiempo  
- Evaluar la interacción de los usuarios mediante calificaciones y reseñas  
- Identificar autores y editoriales con mejor desempeño  
- Generar información estratégica para el diseño de un nuevo producto literario digital  

---

## 📂 Descripción de los datos

La base de datos contiene cinco tablas principales:

### 📘 `books`
Información general de los libros:
- `book_id`
- `author_id`
- `title`
- `num_pages`
- `publication_date`
- `publisher_id`

### ✍️ `authors`
Información de autores:
- `author_id`
- `author`

### 🏢 `publishers`
Información de editoriales:
- `publisher_id`
- `publisher`

### ⭐ `ratings`
Calificaciones otorgadas por usuarios:
- `rating_id`
- `book_id`
- `username`
- `rating`

### 📝 `reviews`
Reseñas de texto escritas por los usuarios:
- `review_id`
- `book_id`
- `username`
- `text`

---

## 🧩 Preguntas de análisis abordadas

El proyecto responde, mediante consultas SQL, a las siguientes preguntas:

1. ¿Cuántos libros fueron publicados después del 1 de enero de 2000?
2. ¿Cuál es el número de reseñas de usuarios y la calificación promedio para cada libro?
3. ¿Qué editorial ha publicado el mayor número de libros con más de 50 páginas?
4. ¿Qué autor tiene la calificación promedio más alta considerando solo libros con al menos 50 calificaciones?
5. ¿Cuál es el número promedio de reseñas de texto entre los usuarios que calificaron más de 50 libros?

Cada pregunta fue resuelta mediante consultas SQL documentadas y ejecutadas desde el notebook.

---

## 🛠️ Herramientas y tecnologías utilizadas

- SQL (PostgreSQL)
- Python
- Pandas
- SQLAlchemy
- Jupyter Notebook

> 🔎 Todas las métricas y resultados se obtuvieron mediante **consultas SQL**.  
> Python se utilizó únicamente para la conexión a la base de datos y la visualización de resultados.

---

## 📈 Principales hallazgos

- La producción editorial muestra un ritmo sostenido de publicaciones entre los años 2000 y 2020.
- Editoras consolidadas como **Penguin Books** y **Vintage** lideran la publicación de libros extensos (más de 50 páginas).
- Autores como **Diana Gabaldon** y **J.K. Rowling** presentan las calificaciones promedio más altas, superando el valor de 4.2.
- Los usuarios más activos (más de 50 calificaciones) muestran un alto nivel de compromiso, con un promedio cercano a **720 reseñas de texto**.
- El uso de `LEFT JOIN` permitió incluir libros con calificaciones aun cuando no contaban con reseñas escritas, evitando sesgos en el análisis.

---

## 🧭 Conclusión general

El análisis reveló un ecosistema literario digital donde la **calidad de las obras, la reputación de autores consolidados y la participación activa de los usuarios** juegan un papel central.

Los resultados muestran que los usuarios más comprometidos no solo califican libros con frecuencia, sino que también aportan reseñas detalladas, generando valor para la comunidad lectora. Asimismo, la concentración de publicaciones en editoriales reconocidas sugiere un mercado que prioriza la calidad editorial y la experiencia del lector.

Este proyecto demuestra cómo el uso estratégico de **SQL** permite transformar datos relacionales en conocimiento accionable, apoyando decisiones relacionadas con la curaduría de contenidos, el diseño de productos digitales y las estrategias de recomendación.

---

## 📂 Archivos del proyecto

- 📓 `notebook Proyecto SQL Final.ipynb` – Consultas SQL y análisis
- 📘 `README.md` – Documentación del proyecto

---

## ✅ Estado del proyecto

✔ Consultas SQL completadas  
✔ Resultados documentados  
✔ Análisis alineado a objetivos de negocio  

---

## 🔗 Enlace al repositorio

El código completo del proyecto y las consultas SQL se encuentran disponibles en el repositorio de GitHub:

👉 https://github.com/utsa2004/proyectos-bootcamp-data-analyst-tripleten/tree/main/Proyecto%20FInal%20Sprint%2014/14.2%20Proyecto%20SQL

---

## 🧠 Nota final

Este proyecto evidencia la capacidad de **analizar bases de datos relacionales complejas**, formular preguntas de negocio y obtener respuestas claras mediante SQL, sentando bases sólidas para el desarrollo de productos digitales orientados a datos en el sector editorial.
