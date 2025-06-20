# Publicar un informe en Power BI con datos CSV desde GitHub

## Objetivo

Crear un informe en Power BI que lea los datos del Titanic desde un CSV público alojado en GitHub, genere visualizaciones y publique un panel interactivo en el servicio de Power BI.

---

## Paso a paso

### 1. Obtener URL del CSV

1. Ve al repositorio de GitHub con el dataset.
2. Haz clic en el archivo `titanic.csv`.
3. Haz clic en **"Raw"**.
4. Copia la URL desde el navegador. Ejemplo:

   ```
   https://raw.githubusercontent.com/datasciencedojo/datasets/master/titanic.csv
   ```

---

### 2. Conectar Power BI al CSV en GitHub

1. Abre **Power BI Desktop**.
2. Haz clic en **Obtener datos** > **Web**.
3. Pega la URL copiada del CSV.
4. Asegúrate de que Power BI reconozca el delimitador correctamente.
5. Haz clic en **Cargar**.

---

### 3. Limpiar y preparar datos

1. Haz clic en **Transformar datos**.
2. Revisa que las columnas tengan tipos adecuados:

   * `Survived` → número / categórica
   * `Sex` → texto
   * `Age` → número
   * `Pclass` → número
3. Opcional: renombra columnas para legibilidad (`Survived` → `Superviviente`, etc.).
4. Cierra y aplica los cambios.

---

### 4. Crear visualizaciones

En la vista de informe, crea las siguientes visualizaciones:

#### 1. Gráfico de barras: Supervivencia por género

* Eje: `Sex`
* Valores: `Survived` (cuenta o promedio)
* Título: "Supervivencia por género"

#### 2. Histograma de edad

* Campo: `Age`
* Usa visualización de histograma personalizada o gráfico de columnas agrupadas
* Título: "Distribución de edad de pasajeros"

#### 3. Tabla resumen por clase

* Columnas: `Pclass`, `Survived` (promedio o cuenta), `Fare` (promedio)
* Título: "Resumen por clase de pasajero"

#### 4. Segmentadores

* Para filtrar visualizaciones:

  * `Sex` (Sexo)
  * `Pclass` (Clase)

---

### 5. Publicar el informe en Power BI Service

1. Haz clic en **Archivo** > **Publicar** > **Mi espacio de trabajo**.
2. Inicia sesión con tu cuenta de Power BI.
3. Espera a que se complete la publicación.

---

### 6. Crear un panel (dashboard)

1. Ve a [https://app.powerbi.com](https://app.powerbi.com) y entra a **Mi espacio de trabajo**.
2. Abre el informe publicado.
3. Haz clic en el icono de chincheta 📌 en una visualización.
4. Crea un nuevo panel llamado **"Panel Titanic"**.
5. Agrega más visualizaciones al panel.

---

### 7. Compartir el panel

* Puedes compartir el panel con otros usuarios con cuentas Power BI.
* También puedes publicar en la web si los datos son públicos:

  1. Ve al panel.
  2. Haz clic en **Archivo** > **Publicar en la web**.
  3. Copia el enlace o iframe.

---

## Resultado esperado

* Informe interactivo con visualizaciones del dataset Titanic.
* Publicación en Power BI Service.
* Panel compartible con usuarios o de forma pública.

---

¿Quieres que te genere directamente un ejemplo en Power BI (archivo `.pbix`) o alguna visualización específica en imagen?
