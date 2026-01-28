# 📦 Guía: Cómo Gestionar tus Productos

## ✨ ¡Ahora puedes agregar, editar o eliminar productos sin tocar el código de tu sitio web!

---

## 📝 Instrucciones Rápidas

### 1️⃣ Editar Productos desde GitHub (Método más fácil)

1. Ve a tu repositorio en GitHub
2. Haz clic en el archivo `productos.json`
3. Haz clic en el **icono del lápiz** (✏️) que dice "Edit this file"
4. Edita el contenido siguiendo el formato que verás abajo
5. Baja hasta el final y haz clic en **"Commit changes"**
6. ¡Listo! Tu sitio web se actualizará automáticamente

---

## 📋 Formato del Archivo JSON

```json
[
  {
    "id": 1,
    "nombre": "Nombre del Producto",
    "precio": 95.00,
    "img": "URL_de_la_imagen",
    "descripcion": "Descripción opcional del producto"
  },
  {
    "id": 2,
    "nombre": "Otro Producto",
    "precio": 45.00,
    "img": "URL_de_la_imagen",
    "descripcion": "Otra descripción"
  }
]
```

---

## ➕ Cómo AGREGAR un Producto Nuevo

1. Copia este bloque:
```json
,
{
  "id": 7,
  "nombre": "Mi Nuevo Producto",
  "precio": 99.99,
  "img": "https://images.unsplash.com/photo-XXXXXXXXX?w=600",
  "descripcion": "Descripción de mi producto"
}
```

2. Pégalo ANTES del corchete final `]`
3. Asegúrate de que el ID sea único (usa el siguiente número disponible)
4. Cambia el nombre, precio e imagen
5. Guarda los cambios

**⚠️ IMPORTANTE:** No olvides la **coma (,)** antes del nuevo producto

---

## ✏️ Cómo EDITAR un Producto Existente

1. Busca el producto que quieres editar en el archivo
2. Cambia el `"nombre"`, `"precio"` o `"img"` según necesites
3. Guarda los cambios

**Ejemplo:**
```json
{
  "id": 1,
  "nombre": "NUEVO NOMBRE AQUÍ",
  "precio": 120.00,
  "img": "https://nueva-imagen.jpg",
  "descripcion": "Nueva descripción"
}
```

---

## ❌ Cómo ELIMINAR un Producto

1. Busca el producto que quieres eliminar
2. Borra **TODO el bloque** del producto (desde `{` hasta `}`)
3. **¡CUIDADO!** Si eliminas un producto que NO es el último, también debes eliminar la coma que está después

**Antes:**
```json
[
  {
    "id": 1,
    "nombre": "Producto 1",
    "precio": 50.00
  },
  {
    "id": 2,
    "nombre": "Producto a Eliminar",
    "precio": 75.00
  },
  {
    "id": 3,
    "nombre": "Producto 3",
    "precio": 100.00
  }
]
```

**Después (eliminando Producto 2):**
```json
[
  {
    "id": 1,
    "nombre": "Producto 1",
    "precio": 50.00
  },
  {
    "id": 3,
    "nombre": "Producto 3",
    "precio": 100.00
  }
]
```

---

## 🖼️ Dónde Conseguir Imágenes

### Opción 1: Unsplash (Gratis)
1. Ve a https://unsplash.com
2. Busca la imagen que quieras
3. Haz clic derecho en la imagen → "Copiar dirección de imagen"
4. Pega esa URL en el campo `"img"`

### Opción 2: Subir tus propias imágenes a GitHub
1. En tu repositorio, haz clic en "Add file" → "Upload files"
2. Sube tu imagen (ej: `mi-producto.jpg`)
3. Usa esta URL: `mi-producto.jpg`

---

## ⚠️ Consejos Importantes

✅ **Siempre verifica que el JSON sea válido**
   - Usa comillas dobles `"` (no simples `'`)
   - No olvides las comas entre productos
   - El último producto NO debe tener coma al final

✅ **IDs únicos**
   - Cada producto debe tener un ID diferente
   - Los IDs deben ser números (sin comillas)

✅ **Precios**
   - Usa punto para decimales: `95.00` (no `95,00`)
   - Sin símbolo de dólar en el precio

✅ **Prueba tu JSON**
   - Puedes usar https://jsonlint.com para verificar que tu JSON sea válido
   - Copia y pega tu código ahí antes de guardar

---

## 🚀 Ejemplo Completo

```json
[
  {
    "id": 1,
    "nombre": "Combo Familiar Súper",
    "precio": 95.00,
    "img": "https://images.unsplash.com/photo-1542838132-92c53300491e?w=600",
    "descripcion": "Paquete completo para toda la familia"
  },
  {
    "id": 2,
    "nombre": "Kit de Salud Prioritario",
    "precio": 45.00,
    "img": "https://images.unsplash.com/photo-1584308666744-24d5c474f2ae?w=600",
    "descripcion": "Medicamentos y productos esenciales"
  },
  {
    "id": 3,
    "nombre": "Pack Cárnico Especial",
    "precio": 110.00,
    "img": "https://images.unsplash.com/photo-1621939514649-280e2ee25f60?w=600",
    "descripcion": "Carnes y embutidos premium"
  }
]
```

---

## 🆘 Solución de Problemas

**❓ Los productos no aparecen en mi sitio**
- Verifica que el archivo se llame exactamente `productos.json`
- Revisa que esté en la misma carpeta que `index.html`
- Espera 1-2 minutos para que GitHub Pages actualice

**❓ Sale un error en la página**
- Revisa tu JSON en https://jsonlint.com
- Asegúrate de tener todas las comas correctas
- Verifica que los corchetes `[` y `]` estén completos

**❓ Las imágenes no se muestran**
- Verifica que la URL de la imagen sea correcta
- Asegúrate de que la imagen sea pública (accesible sin login)

---

## 💡 Tips Extra

- Mantén los nombres de productos cortos (máximo 30 caracteres)
- Las imágenes funcionan mejor en formato cuadrado o horizontal
- Actualiza el sitio en GitHub y espera 1-2 minutos para ver los cambios
- Haz una copia de seguridad de tu `productos.json` antes de hacer cambios grandes

---

¡Listo! Ahora puedes gestionar tus productos fácilmente sin ser programador 🎉
