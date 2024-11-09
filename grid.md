# Tailwind CSS Grid Examples Cheat Sheet

---

## Grid Container Properties

- **`.grid`**: Defines a grid container.  
- **`.grid-cols-{n}`**: Sets the number of columns (e.g., `.grid-cols-3`).  
- **`.grid-rows-{n}`**: Sets the number of rows (e.g., `.grid-rows-2`).  
- **`.gap-{n}`**: Adds a gap between rows and columns (e.g., `.gap-4`).  
- **`.gap-x-{n}`**: Adds horizontal gap between columns (e.g., `.gap-x-2`).  
- **`.gap-y-{n}`**: Adds vertical gap between rows (e.g., `.gap-y-2`).  

### Example:
```html
<div class="grid grid-cols-3 gap-4">
  <div class="p-4 bg-gray-200">Grid Item 1</div>
  <div class="p-4 bg-gray-300">Grid Item 2</div>
  <div class="p-4 bg-gray-400">Grid Item 3</div>
  <div class="p-4 bg-gray-500">Grid Item 4</div>
</div>
```

---

## Grid Column and Row Span

- **`.col-span-{n}`**: Makes an item span `n` columns (e.g., `.col-span-2`).  
- **`.row-span-{n}`**: Makes an item span `n` rows (e.g., `.row-span-2`).  

### Example:
```html
<div class="grid grid-cols-4 gap-4">
  <div class="col-span-2 p-4 bg-blue-200">Span 2 Columns</div>
  <div class="p-4 bg-blue-300">Item 2</div>
  <div class="p-4 bg-blue-400">Item 3</div>
  <div class="p-4 bg-blue-500">Item 4</div>
</div>
```

---

## Grid Template Areas

- **`.grid-areas`**: Defines grid template areas using custom CSS.  
- Use **`grid-area: name`** to place grid items into specific areas.  

### Example:
```html
<div class="grid grid-rows-2 grid-cols-2 gap-4" style="grid-template-areas: 'header header' 'sidebar main'">
  <div class="p-4 bg-green-200" style="grid-area: header;">Header</div>
  <div class="p-4 bg-green-300" style="grid-area: sidebar;">Sidebar</div>
  <div class="p-4 bg-green-400" style="grid-area: main;">Main Content</div>
</div>
```

---

## Alignment and Justification

- **`.place-items-center`**: Centers items in both directions.  
- **`.place-content-center`**: Centers the entire grid content.  
- **`.justify-items-start`**, **`.justify-items-center`**, **`.justify-items-end`**, **`.justify-items-stretch`**: Aligns grid items along the inline axis.  
- **`.items-start`**, **`.items-center`**, **`.items-end`**, **`.items-stretch`**: Aligns grid items along the block axis.  

### Example:
```html
<div class="grid grid-cols-3 place-items-center gap-4">
  <div class="p-4 bg-red-200">Item 1</div>
  <div class="p-4 bg-red-300">Item 2</div>
  <div class="p-4 bg-red-400">Item 3</div>
</div>
```

---

## Responsive Grid Layouts

- Use **`sm:grid-cols-{n}`**, **`md:grid-cols-{n}`**, **`lg:grid-cols-{n}`**, **`xl:grid-cols-{n}`** for responsive design.  

### Example:
```html
<div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 lg:grid-cols-4 gap-4">
  <div class="p-4 bg-yellow-200">Responsive Item 1</div>
  <div class="p-4 bg-yellow-300">Responsive Item 2</div>
  <div class="p-4 bg-yellow-400">Responsive Item 3</div>
  <div class="p-4 bg-yellow-500">Responsive Item 4</div>
</div>
```

---

