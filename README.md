# <img width="1831" height="134" alt="Captura de pantalla 2025-08-25 105746" src="https://github.com/user-attachments/assets/19d89aee-03ee-4104-a3b8-3f4ea35a815a" />

<a name="indice"></a>
## <img width="159" height="92" alt="Captura de pantalla 2025-08-25 110450" src="https://github.com/user-attachments/assets/a1adf839-9802-48ea-b56f-7cd19f47d3cf" />

1. [Descripción del trabajo](#descripcion-del-trabajo)  
2. [Objetivos de Aprendizaje](#objetivos-de-aprendizaje)
3. [Tecnologías usadas](#tecnologias-usadas)  
4. [Requisitos Técnicos](#requisitos-tecnicos)
5. [Resultado Final](#resultado-final)
6. [Recomendaciones](#recomendaciones)  
7. [Conclusiones](#conclusiones)  
8. [Desarrolladora](#desarrolladora)  

---

<a name="descripcion-del-trabajo"></a>
## <img width="486" height="91" alt="Captura de pantalla 2025-08-25 110458" src="https://github.com/user-attachments/assets/877a6f78-4cde-43b1-9a19-0bf3301700a1" />

Este proyecto consiste en la construcción de una **versión digital de la Tabla Periódica** utilizando únicamente etiquetas de **tablas HTML**. El reto busca aplicar una estructura semántica correcta, estilos personalizados y un poco de interactividad con CSS.  

La Tabla Periódica es el ejemplo perfecto de datos tabulares, y este reto demuestra cómo **HTML + CSS** pueden organizar información compleja de manera clara, elegante y dinámica.  

[⬆️ Volver al índice](#indice)

---

<a name="objetivos-de-aprendizaje"></a>
## <img width="192" height="98" alt="Captura de pantalla 2025-08-25 110506" src="https://github.com/user-attachments/assets/6bbbdf85-1e97-4114-8f6c-4ec9306d31e7" />

- Estructurar datos complejos usando las etiquetas `<table>`, `<tr>`, `<th>` y `<td>`.  
- Manejar **celdas vacías** y expansiones de columnas (`colspan`) para crear layouts complejos.  
- Aplicar **estilos dinámicos** basados en categorías de elementos químicos.  
- Añadir **interactividad visual** utilizando pseudo-clases de CSS (`:hover`).  

[⬆️ Volver al índice](#indice)

---

<a name="tecnologias-usadas"></a>
## <img width="401" height="107" alt="Captura de pantalla 2025-08-25 110513" src="https://github.com/user-attachments/assets/b8800793-2a03-4237-aeb1-7ebfe61aa95d" />

- **HTML5** → estructura de la tabla y contenido de cada elemento.  
- **CSS3** → estilos, categorías por colores, y efectos dinámicos.  
- **Git & GitHub** → control de versiones y despliegue del proyecto.  

[⬆️ Volver al índice](#indice)

---

<a name="requisitos-tecnicos"></a>
## <img width="352" height="95" alt="Captura de pantalla 2025-08-25 110653" src="https://github.com/user-attachments/assets/83d70c86-f07e-4c08-98bb-a38a541d7c9d" />

### 1️⃣ Estructura del HTML (`index.html`)  
- Toda la tabla está contenida en un `<table>`.  
- Se crean filas con `<tr>` y celdas con `<td>`.  
- Cada elemento tiene su celda propia, mientras que los espacios vacíos se representan con `<td></td>`.  
- Ejemplo de la primera fila:  
  - 1 celda para el **Hidrógeno**  
  - 16 celdas vacías  
  - 1 celda para el **Helio**  

Dentro de cada celda de elemento se muestra:  
- Número atómico  
- Símbolo químico  
- Nombre del elemento  

---

### 2️⃣ Estilizado con CSS (`style.css`)  
- Bordes, tamaños y alineación configurados para una presentación clara.  

```css
.table {
  border-collapse: collapse;
  width: 100%;
}

.element {
  border: 1px solid #ccc;
  padding: 10px;
  text-align: center;
  width: 5.5%; /* 100% / 18 columnas aprox */
}
```

- Colores por categorías químicas (ej: `.gas-noble`, `.alcalino`, `.metal-transicion`).
- Celdas vacías sin color.

---

### 3️⃣ Interactividad con `:hover`

Se aplica un efecto visual elegante cuando el usuario pasa el cursor sobre los elementos:

```css
.element:hover {
  transform: scale(1.1);
  box-shadow: 0 0 10px rgba(0,0,0,0.5);
  background-color: #333;
  color: white;
}
```

[⬆️ Volver al índice](#indice)

---
<a name="resultado-final"></a>
## <img width="271" height="94" alt="Captura de pantalla 2025-08-25 115251" src="https://github.com/user-attachments/assets/774bb374-bfe4-454b-8ced-f99b26b3683f" />

<img width="1919" height="1021" alt="Captura de pantalla 2025-08-25 115130" src="https://github.com/user-attachments/assets/d28882dc-66ed-41f2-8d63-ae4ba8819839" />

<a name="recomendaciones-contenido"></a>
## <img width="302" height="92" alt="Captura de pantalla 2025-08-25 110520" src="https://github.com/user-attachments/assets/e94df966-44ab-4e6a-89bc-b6732c8665b2" />

- Usar un navegador actualizado para visualizar correctamente el diseño.  
- Mantener el código ordenado y comentado para futuras mejoras.  
- Se sugiere explorar la posibilidad de agregar **JavaScript** para hacerlo interactivo (por ejemplo: mostrar información de cada elemento al pasar el cursor).  

[⬆️ Volver al índice](#indice)

---

<a name="conclusiones"></a>
## <img width="263" height="86" alt="Captura de pantalla 2025-08-25 110527" src="https://github.com/user-attachments/assets/01be363c-3b7e-406e-9245-ecc7cdd630ff" />

Este reto permitió aplicar de manera práctica los conocimientos de HTML y CSS en la construcción de una tabla compleja como la tabla periódica, gracias a la estructura semántica con `<table>`, `<tr>`, `<th>` y `<td>`, fue posible organizar los elementos químicos y espacios vacíos de forma ordenada, representando fielmente la distribución real de la tabla periódica. El trabajo con estilos CSS para diferenciar categorías de elementos y aplicar efectos de interactividad reforzó la importancia de combinar estructura semántica y diseño visual en un mismo proyecto.

Durante el desarrollo del proyecto, el uso de Git y GitHub fue fundamental para mantener un control de versiones claro y un flujo de trabajo organizado, estas herramientas facilitaron el guardado de avances incrementales, la posibilidad de revertir cambios en caso de errores, y mantener un historial completo del desarrollo. En un entorno académico y de colaboración, este tipo de control de versiones resulta clave para simular las mejores prácticas de la industria del software y acostumbrarse a trabajar de manera profesional desde la formación universitaria.

El proyecto no solo cumplió con los objetivos planteados, sino que también establece una base sólida para futuras mejoras y funcionalidades. La tabla periódica digital desarrollada puede evolucionar incorporando más estilos, funcionalidades interactivas o incluso información adicional de cada elemento, convirtiéndose en una herramienta educativa digital, de esta manera, lo que comenzó como un ejercicio académico puede llegar a ser un recurso útil para estudiantes y docentes de ciencias, demostrando el potencial de integrar programación y educación


[⬆️ Volver al índice](#indice)

---

<a name="desarrolladora"></a>
## <img width="283" height="86" alt="Captura de pantalla 2025-08-25 110539" src="https://github.com/user-attachments/assets/b47c5155-393e-4014-8eec-5a58960f7121" />

Este proyecto fue desarrollado por Johana Jazmín Saavedra, estudiante de cuarto semestre en Técnica profesional en programación de aplicaciones de software de la Fundación Universitaria Compensar. Con una participación activa en la creación y desarrollo del proyecto.

<div align="center">
  <img width="124" height="336" alt="Joh sin fondo" src="https://github.com/user-attachments/assets/6c7a7f5a-749b-4912-8fbc-9fec2bba3463" />
  <br>
  <strong>Johana Jazmín Saavedra</strong>
</div>

[⬆️ Volver al índice](#indice)
