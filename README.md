# Inventario Móvil

[![Licencia: MIT](https://img.shields.io/badge/Licencia-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![GitHub issues](https://img.shields.io/github/issues/nayo/inventarios)](https://github.com/nayo/inventarios/issues)
[![GitHub stars](https://img.shields.io/github/stars/nayo/inventarios)](https://github.com/nayo/inventarios/stargazers)

**Inventario Móvil** es una aplicación web de código abierto para la gestión de inventarios, diseñada para ser fácil de usar en dispositivos móviles y de escritorio. Permite gestionar múltiples inventarios, agregar, editar o eliminar productos, capturar imágenes con la cámara, exportar datos a CSV y PDF (con imágenes), aplicar filtros (búsqueda, categoría, marca, inventario bajo), y personalizar temas (Claro, Oscuro, Azul, Verde) y umbrales de inventario bajo. La aplicación está optimizada para iOS y Android y puede instalarse como un acceso directo en la pantalla de inicio.

Este proyecto está alojado en [GitHub](https://github.com/nayo/inventarios) y es de código abierto bajo la [Licencia MIT](#licencia). ¡Animamos a la comunidad a contribuir con mejoras, correcciones de errores y nuevas funcionalidades!

## Características

- **Gestión de múltiples inventarios**: Crea, edita y elimina inventarios con confirmación de eliminación.
- **Gestión de productos**: Agrega, edita o elimina productos con detalles como nombre, descripción, precio, categoría, marca, cantidad e imagen, con confirmación de eliminación.
- **Captura de imágenes**: Sube imágenes o usa la cámara del dispositivo para asociar fotos a los productos, con vista previa en la interfaz.
- **Exportación de datos**: Exporta inventarios a CSV o PDF, incluyendo imágenes de productos y detalles de reabastecimiento si el filtro de inventario bajo está activo.
- **Filtros avanzados**: Busca productos por nombre, filtra por categoría, marca o inventario bajo.
- **Umbral de inventario bajo**: Configura un umbral personalizado para identificar productos con stock bajo y calcula el costo de reabastecimiento.
- **Interfaz adaptable**: Alterna entre vista de tarjetas y lista, con temas personalizables (Claro, Oscuro, Azul, Verde) configurables en el menú de **Configuraciones**.
- **Optimización móvil**: Compatible con iOS (Safari) y Android (Chrome, Samsung Internet), con soporte para áreas seguras, eventos táctiles, cámara y modo de pantalla completa.
- **Acceso directo**: Instala la aplicación como un acceso directo en la pantalla de inicio de iOS o Android para un acceso rápido.

## Demo

Prueba la aplicación en: [https://nayo.github.io/inventarios/](https://nayo.github.io/inventarios/)

## Requisitos

- Un navegador moderno (Safari, Chrome, Firefox, Samsung Internet, etc.).
- Conexión a internet para cargar dependencias (Material Components Web, jsPDF).
- Acceso a la cámara del dispositivo para la captura de imágenes (opcional).
- HTTPS para instalación como acceso directo en iOS/Android (proporcionado por GitHub Pages).

## Instalación

1. **Clona el repositorio**:
   ```bash
   git clone https://github.com/nayo/inventarios.git
   cd inventarios
   ```

2. **Prueba localmente** (opcional):
   - Instala un servidor local como `http-server`:
     ```bash
     npm install -g http-server
     http-server .
     ```
   - Abre `http://localhost:8080` en tu navegador.

3. **Instala como acceso directo**:
   - **En iOS (Safari)**:
     - Abre [https://nayo.github.io/inventarios/](https://nayo.github.io/inventarios/) en Safari.
     - Toca el ícono de **Compartir** (cuadrado con flecha hacia arriba).
     - Selecciona **Agregar a pantalla de inicio**, edita el nombre (e.g., “Inventario Móvil”) y toca **Agregar**.
   - **En Android (Chrome)**:
     - Abre [https://nayo.github.io/inventarios/](https://nayo.github.io/inventarios/) en Chrome.
     - Toca el menú de tres puntos > **Agregar a pantalla de inicio**.
     - Edita el nombre y toca **Agregar**.

## Uso

1. **Crear un inventario**:
   - Haz clic en el ícono de “Agregar inventario” (+) en la pantalla principal.
   - Ingresa un nombre y guarda.

2. **Agregar productos**:
   - Selecciona un inventario y haz clic en el ícono de “Agregar producto” (+).
   - Completa los campos en el diálogo de **Agregar Producto** (nombre, descripción, precio, categoría, marca, cantidad).
   - Opcionalmente, sube una imagen o toma una foto con la cámara (se muestra una **Vista previa de la imagen**).

3. **Gestionar productos**:
   - Ajusta cantidades (+1/-1), edita o elimina productos desde la lista.
   - Usa los filtros (búsqueda, categoría, marca, inventario bajo) para gestionar productos.
   - Confirma la eliminación de productos con el diálogo **Confirmar Eliminación**.

4. **Eliminar inventarios**:
   - En la pantalla principal, haz clic en “Eliminar” junto a un inventario.
   - Confirma en el diálogo **Confirmar Eliminación**.

5. **Exportar datos**:
   - Exporta el inventario actual a CSV o PDF usando los botones en la pantalla de gestión.
   - Los PDF incluyen imágenes y detalles de reabastecimiento si el filtro de inventario bajo está activo.

6. **Personalizar**:
   - Abre el menú de **Configuraciones** (ícono de engranaje) para ajustar el umbral de inventario bajo y seleccionar un **Tema** (Claro, Oscuro, Azul, Verde).

## Contribución

¡Invitamos a la comunidad a contribuir! Este proyecto es de código abierto y se beneficia de las mejoras y correcciones de todos. Aquí tienes cómo participar:

### Cómo contribuir

1. **Fork el repositorio**:
   - Haz clic en **Fork** en [https://github.com/nayo/inventarios](https://github.com/nayo/inventarios).

2. **Clona tu fork**:
   ```bash
   git clone https://github.com/yourusername/inventarios.git
   cd inventarios
   ```

3. **Crea una rama**:
   ```bash
   git checkout -b feature/nueva-funcionalidad
   ```

4. **Realiza cambios**:
   - Edita el código en `index.html` u otros archivos.
   - Asegúrate de que los cambios sean compatibles con navegadores móviles (Safari, Chrome).
   - Prueba localmente antes de enviar.

5. **Envía un Pull Request**:
   ```bash
   git add .
   git commit -m "Agrega nueva funcionalidad: descripción"
   git push origin feature/nueva-funcionalidad
   ```
   - Crea un Pull Request en [https://github.com/nayo/inventarios](https://github.com/nayo/inventarios), describiendo los cambios y su propósito.

### Lineamientos de contribución

- **Código limpio**: Sigue las convenciones de estilo del proyecto (HTML, CSS, JavaScript).
- **Compatibilidad**: Asegúrate de que los cambios funcionen en iOS (Safari) y Android (Chrome, Samsung Internet).
- **Pruebas**: Incluye pruebas para nuevas funcionalidades o correcciones, especialmente en dispositivos móviles.
- **Issues**: Revisa o crea un issue en [https://github.com/nayo/inventarios/issues](https://github.com/nayo/inventarios/issues) para discutir propuestas.
- **Documentación**: Actualiza este README si agregas nuevas funcionalidades o cambias el uso de la app.

### Ideas para contribuciones

- Agregar soporte completo para Progressive Web App (PWA) con `manifest.json` y service worker para uso offline.
- Implementar sincronización con una base de datos en la nube (e.g., Firebase).
- Mejorar el diseño para pantallas grandes (tabletas, escritorio).
- Agregar soporte para múltiples idiomas.
- Implementar notificaciones para productos con inventario bajo.
- Optimizar el rendimiento para grandes inventarios (e.g., paginación).
- Mejorar la compresión de imágenes para reducir el tamaño de los PDF.

## Problemas conocidos

- **Actualización de UI en móviles**: Resuelto en la última versión. Si persisten problemas, verifica la versión del navegador o reporta un issue en [https://github.com/nayo/inventarios/issues](https://github.com/nayo/inventarios/issues).
- **Imágenes grandes en PDF**: Las imágenes grandes pueden aumentar el tamaño del PDF. Considera agregar compresión de imágenes.
- **Soporte offline**: La app requiere conexión para cargar dependencias. Un service worker puede habilitar uso offline.

Reporta cualquier error o sugerencia en [GitHub Issues](https://github.com/nayo/inventarios/issues).

## Licencia

Este proyecto está licenciado bajo la [Licencia MIT](LICENSE). Siéntete libre de usar, modificar y distribuir el código según los términos de la licencia.

## Contacto

- **Autor**: Nayo
- **GitHub**: [nayo](https://github.com/nayo)
- **Issues**: Reporta problemas o sugerencias en [https://github.com/nayo/inventarios/issues](https://github.com/nayo/inventarios/issues).

¡Gracias por contribuir a Inventario Móvil! 🚀
