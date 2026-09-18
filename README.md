# Generador de Asignación de Camioneta

Formulario web para generar el documento de "Asignación de camioneta por supervisor" (Geotek/GBB). Se completa el formulario de la izquierda y la vista previa de la derecha se actualiza al instante, lista para descargar como PDF o imprimir.

## Estructura del proyecto

```
.
├── index.html          # Estructura de la página (formulario + vista previa)
├── assets/
│   ├── styles.css       # Estilos de la aplicación
│   ├── script.js        # Lógica: estado del formulario, vista previa y generación de PDF
│   └── logo.png          # Logo de Geotec Boyles Bros usado en el documento
└── README.md
```

## Uso

Abre `index.html` en el navegador (no requiere servidor ni build). También puedes publicarlo gratis con GitHub Pages:

1. Sube este repositorio a GitHub.
2. En **Settings → Pages**, elige la rama `main` y la carpeta `/ (root)`.
3. GitHub te entrega una URL pública (`https://<usuario>.github.io/<repositorio>/`).

## Funcionalidad

- **Datos del documento**: fecha, modelo de camioneta, patente (PPU) y número interno.
- **Reciben conforme**: lista de personas (nombre, cargo, RUT), se pueden agregar o quitar filas.
- **Descargar PDF**: genera un PDF con el mismo diseño del documento original usando `html2canvas` + `jsPDF` (cargados desde CDN).
- **Imprimir**: abre el diálogo de impresión del navegador con estilos optimizados para carta (`@media print`).
- **Restablecer campos**: vuelve el formulario a sus valores por defecto.
- Los datos del formulario se guardan en `localStorage` del navegador para no perderlos al recargar la página.

## Dependencias externas (vía CDN)

- [html2canvas](https://cdnjs.cloudflare.com/ajax/libs/html2canvas/1.4.1/html2canvas.min.js)
- [jsPDF](https://cdnjs.cloudflare.com/ajax/libs/jspdf/2.5.1/jspdf.umd.min.js)

No requiere instalación de paquetes ni proceso de build.
