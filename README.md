# 🎨 Guía Básica: CSS y Tailwind (Bordes, Display y Posicionamiento)

## 📌 Descripción

Este proyecto muestra conceptos fundamentales de diseño web usando **CSS tradicional** y **Tailwind CSS**, enfocados en:

* Tipos de bordes
* Diferencias entre `inline`, `block` e `inline-block`
* Uso de `position` (relative / absolute)
* Creación de patrones visuales

---

## 🧱 Conceptos Clave

### 🔹 1. Tipos de Bordes en CSS

CSS permite aplicar diferentes estilos de bordes a cada lado de un elemento:

```css
border-top: 5px solid red;
border-right: 5px dashed green;
border-bottom: 5px dotted blue;
border-left: 5px double purple;
```

📚 Tipos disponibles:

* `solid`
* `dashed`
* `dotted`
* `double`
* `groove`
* `ridge`
* `inset`
* `outset`

---

### 🔹 2. Display: inline vs block vs inline-block

| Tipo           | Característica                 |
| -------------- | ------------------------------ |
| `inline`       | No respeta width/height        |
| `block`        | Ocupa todo el ancho disponible |
| `inline-block` | Mezcla ambos comportamientos   |

Ejemplo:

```css
display: inline-block;
```

💡 `inline-block` es el más usado en menús.

---

### 🔹 3. Box Model (Modelo de Caja)

Cada elemento HTML está compuesto por:

* `content`
* `padding`
* `border`
* `margin`

```css
box-sizing: border-box;
```

✔️ Recomendado para evitar problemas de tamaño.

---

### 🔹 4. Posicionamiento

Tipos principales:

* `relative` → referencia base
* `absolute` → se posiciona respecto al padre

Ejemplo:

```css
position: absolute;
top: 0;
left: 0;
```

---

## ⚡ Tailwind CSS

Tailwind es un framework de utilidades que permite escribir estilos directamente en clases HTML.

### Ejemplo básico:

```html
<div class="bg-blue-500 text-white p-4">
  Hola mundo
</div>
```

---

## 🧩 Ejemplo del Reto (Patrón Visual)

```html
<div class="relative w-[600px] h-[350px]">

  <!-- izquierda -->
  <div class="absolute left-0 top-0 h-full border-l-[12px] border-blue-900"></div>

  <!-- abajo -->
  <div class="absolute bottom-0 left-0 w-full border-b-[4px] border-cyan-400"></div>

  <!-- arriba doble -->
  <div class="absolute top-0 left-0 w-full border-t-[6px] border-yellow-500"></div>
  <div class="absolute top-[10px] left-0 w-full border-t-[6px] border-yellow-600"></div>

  <!-- derecha punteada -->
  <div class="absolute right-0 top-0 h-full border-r-[8px] border-purple-700 border-dashed"></div>

</div>
```

---

## 🚀 Cómo usar Tailwind

1. Agrega el CDN:

```html
<script src="https://cdn.jsdelivr.net/npm/@tailwindcss/browser@4"></script>
```

2. Usa clases directamente en HTML

---

## 🎯 Conclusión

Con estos conceptos puedes:

* Crear layouts básicos
* Diseñar interfaces modernas
* Entender cómo funciona el CSS detrás de frameworks

---

## 📚 Recomendaciones

* Practica combinando `display` + `position`
* Usa `inline-block` para menús
* Usa Tailwind para prototipos rápidos
* Domina el box model

---

## 👨‍💻 Autor

Proyecto educativo para aprender fundamentos de CSS y Tailwind.
