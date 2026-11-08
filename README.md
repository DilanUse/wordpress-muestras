# Muestras en WordPress

Dos sitios ficticios, hechos con un tema propio en PHP y CSS. Las portadas, los textos y las fichas se guardan en WordPress. Ambos enlaces arrancan una sesión independiente de WordPress Playground.

- [Taller Umbral · Reformas](https://playground.wordpress.net/?blueprint-url=https%3A%2F%2Fraw.githubusercontent.com%2FDilanUse%2Fwordpress-muestras%2Fmain%2Freformas.zip). Servicios, proyecto y formulario de presupuesto de prueba.
- [Clave Norte · Inmobiliaria](https://playground.wordpress.net/?blueprint-url=https%3A%2F%2Fraw.githubusercontent.com%2FDilanUse%2Fwordpress-muestras%2Fmain%2Finmobiliaria.zip). Catálogo de tres inmuebles con filtros por operación y barrio, y ficha individual.

Para probar el editor de bloques, pulsa **Editar en WordPress** al pie de una portada. Los inmuebles se administran en **Inmuebles** y sus detalles se guardan en campos personalizados. El formulario de reforma genera una confirmación de ejemplo en pantalla. Las ediciones de la sesión se pueden guardar localmente o exportar desde Playground.

## Vista previa local

```sh
npx --yes @wp-playground/cli@3.1.62 server --blueprint=reformas.zip --port=9423
```

Para abrir la otra portada, usa `inmobiliaria.zip`. Cada paquete contiene `umbral.zip`, el código fuente del tema con sus recursos. Para instalarlo en otro WordPress, extrae ese ZIP y súbelo desde **Apariencia → Temas**. `seed.php` configura el contenido de muestra cuando se ejecuta en el contexto de WordPress. Si estás en la carpeta de desarrollo, `python build.py` regenera ambos paquetes en `dist/`.

Fotografías de [Unsplash](https://unsplash.com/license): [cocina](https://images.unsplash.com/photo-1600607687920-4e2a09cf159d), [salón](https://unsplash.com/photos/RbbZn_M5fgU), [fachada](https://unsplash.com/photos/Ai6etBfYHfI) y [sala luminosa](https://images.unsplash.com/photo-1600210492486-724fe5c67fb0).
