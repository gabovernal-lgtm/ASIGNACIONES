# Asignación de Camioneta

Aplicación web para registrar la entrega y asignación de vehículos de Geotec Boyles Bros.

## Estructura

```text
/
├── index.html
├── README.md
└── assets/
    ├── styles.css
    ├── script.js
    └── logo.png
```

## Publicar en GitHub Pages

1. Sube `index.html`, `README.md` y la carpeta `assets` a la raíz del repositorio.
2. Coloca el logo institucional en `assets/logo.png`.
3. En GitHub abre **Settings → Pages**.
4. Selecciona **Deploy from a branch**, rama `main` y carpeta `/ (root)`.
5. Guarda y espera la publicación del enlace.

## Funciones

- Diseño adaptable a computador y celular.
- Vista previa en tamaño carta.
- Generación de PDF con `html2canvas` y `jsPDF`.
- Impresión desde el navegador.
- Guardado automático local.
- Formato de patente y RUT chileno.
- Validación del dígito verificador del RUT.
- Registro de una o más personas.

> La generación de PDF requiere conexión a internet para cargar las librerías externas.
