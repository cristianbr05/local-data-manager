# 📊 Gestor Local de Registros - Panel SPA

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![Status](https://img.shields.io/badge/Status-Complete-green?style=flat-square)

> **Aplicación web de página única (SPA) diseñada para la visualización, filtrado y gestión de registros procedentes de hojas de cálculo.** 
> La herramienta procesa la información de forma estrictamente local en el navegador del usuario, evitando la transferencia de datos a servidores externos.

| ⚙️ Tipo | 📄 Formatos soportados | 🗄️ Persistencia | 🔍 Motor de búsqueda |
| :--- | :--- | :--- | :--- |
| SPA (Frontend) | `.xlsx`, `.xls`, `.csv` | IndexedDB (localForage) | Fuse.js |

---

## 🛠️ Funcionalidades principales

* **Procesamiento en cliente:** Lectura de hojas de cálculo directamente en el navegador mediante `SheetJS`.
* **Almacenamiento persistente:** Guardado de los registros en la base de datos local del navegador utilizando `localForage`.
* **Búsqueda y filtrado:** Motor de búsqueda difusa (`Fuse.js`) y filtrado multicriterio (fecha, servicio, centro).
* **Exportación de datos:** Generación y descarga de archivos `.csv` a partir de los datos filtrados en pantalla.
* **Gestión de almacenamiento:** Función de purgado manual para eliminar definitivamente los datos de la sesión actual.

---

## 🚀 Instrucciones de uso

1. Abrir el archivo `index.html` en cualquier navegador web moderno.
2. Arrastrar o seleccionar un archivo de hoja de cálculo compatible en la zona de carga principal.
3. Utilizar el panel de controles superior para buscar, filtrar y ordenar los registros cargados en memoria.
4. Emplear el botón **Exportar CSV** para descargar los resultados que se muestran en la tabla.
5. Para limpiar la base de datos local del navegador, pulsar el botón **Borrar Datos**.

> ⚠️ **Nota de privacidad:** Todos los datos se procesan exclusivamente en la memoria RAM del equipo y en el almacenamiento local del navegador (IndexedDB). El aplicativo no realiza peticiones de red para procesar la información.

---
*Desarrollado con ayuda de herramientas de IA.*