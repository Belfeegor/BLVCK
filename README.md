# BLVCK — Tienda online de ropa urbana

Sitio de e-commerce para una marca de ropa streetwear, con catálogo de productos, carrito de compras funcional y ficha de producto interactiva. Construido como proyecto personal para practicar y demostrar manejo de JavaScript vanilla, manipulación del DOM y diseño de interfaz.

## Demo

<img width="1353" height="696" alt="image" src="https://github.com/user-attachments/assets/28973fc8-e629-4209-a230-2e96c3385455" />


## Características

- **Catálogo de productos** con filtro por categoría (Poleras, Pantalones, Chaquetas, Accesorios)
- **Carrito de compras** persistente durante la sesión, con drawer lateral animado
- **Ficha de producto en modal**, con selección de talla y descripción
- **Gestión de cantidad** por ítem (agregar, restar, eliminar)
- **Formulario de newsletter** con confirmación visual
- **Diseño responsive**, adaptado a mobile, tablet y desktop
- **Identidad visual propia**: paleta oscura con acentos en amarillo, tipografía Anton (títulos) + Space Mono (cuerpo), detalles como el hazard stripe y el stamp animado

## Decisiones técnicas

- **JavaScript vanilla, sin frameworks ni librerías externas de UI** La decisión fue deliberada: para un catálogo de este tamaño, un framework como React agregaría complejidad de build (bundler, JSX, dependencias) sin un beneficio real. El estado del carrito se maneja con un array simple en memoria y funciones de render que redibujan solo lo necesario.
  
- **Un solo archivo HTML/CSS/JS.** Facilita compartir y probar el proyecto sin necesidad de servidor ni configuración — se abre directo en el navegador.
  
- **Datos de productos como array estático en el script** No hay backend: es intencional para este alcance. El checkout muestra un mensaje explícito de que es una demo, en vez de simular un pago falso.
  
- **CSS con variables** para la paleta de colores, lo que permite cambiar la identidad visual completa modificando solo el bloque `:root`.

## Estructura del proyecto

```
├── index.html      # Estructura, estilos y lógica (todo en un archivo)
└── README.md
```

## Autor

Dadkerry — Estudiante de programación en INACAP.
