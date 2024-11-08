# Página Personal Adaptable a Diferentes Pantallas

Este proyecto adapta una página personal para que se visualice de manera óptima en dispositivos de diferentes tamaños de pantalla. Se ha utilizado el atributo `viewport` en HTML y las **media queries** en CSS para cambiar el diseño de la página de manera radical según el ancho de pantalla, garantizando una buena experiencia de usuario tanto en dispositivos grandes como pequeños.

## Características

1. **Adaptación a Pantallas Pequeñas (< 800px):**

   - Cuando el ancho de pantalla es menor a 800 píxeles:
     - El `header`, que incluye la imagen personal, el nombre y un SVG, cambia de un diseño horizontal a un diseño vertical, centrando cada elemento uno encima del otro.
     - Estilos específicos para cada elemento:
       - **Imagen personal**: Se ajusta a un ancho del **50%**.
       - **Nombre (h1)**: Ocupa el **100%** del ancho disponible.
       - **SVG**: Ocupa el **100%** del ancho disponible y se le aplica un borde o un color de fondo ligeramente diferente para identificarlo fácilmente.

2. **Adaptación a Pantallas Grandes (>= 800px):**

   - Cuando el ancho de pantalla es igual o mayor a 800 píxeles, el diseño del `header` se muestra en formato horizontal, distribuyendo los elementos con un diseño **20-60-20**:
     - **Imagen personal**: Ocupa el **20%** del ancho.
     - **Nombre (h1)**: Ocupa el **60%** del ancho.
     - **SVG**: Ocupa el **20%** del ancho.

3. **Optimización para Dispositivos Móviles:**
   - Se utiliza la etiqueta `<meta name="viewport" content="width=device-width, initial-scale=1.0">` para hacer que el diseño se adapte automáticamente al ancho del dispositivo y que el zoom inicial sea 1:1, permitiendo una visualización óptima en dispositivos móviles.
