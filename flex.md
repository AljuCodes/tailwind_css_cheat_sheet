# Tailwind CSS Flex Examples Cheat Sheet

---

## Flex Container Properties

- **`.flex`**: Defines a flex container.  
- **`.flex-row`**: Arranges children in a row (default).  
- **`.flex-col`**: Arranges children in a column.  
- **`.flex-wrap`**: Allows wrapping of children onto multiple lines.  
- **`.flex-nowrap`**: Prevents wrapping of children.  
- **`.flex-wrap-reverse`**: Wraps children in reverse order.  

### Example:
```html
<div class="flex flex-wrap">
  <div class="p-4 bg-gray-200">Child 1</div>
  <div class="p-4 bg-gray-300">Child 2</div>
  <div class="p-4 bg-gray-400">Child 3</div>
</div>
```

---

## Flex Item Properties

- **`.flex-1`**: The item will grow to fill the available space.  
- **`.flex-auto`**: The item will shrink and grow as needed, based on the content.  
- **`.flex-initial`**: The item will not grow or shrink and will stay at its initial size.  
- **`.flex-none`**: The item will not grow or shrink, taking up only as much space as needed.  
- **`.basis-{value}`**: Sets the initial size of the flex item (e.g., `.basis-1/2` or `.basis-[200px]`).  

### Example:
```html
<div class="flex">
  <div class="flex-1 p-4 bg-blue-200">Flexible Child</div>
  <div class="p-4 bg-blue-400">Fixed Child</div>
</div>
```

---

## Alignment and Justification

- **`.justify-start`**: Aligns items to the start of the container (left).  
- **`.justify-center`**: Centers items in the container.  
- **`.justify-end`**: Aligns items to the end of the container (right).  
- **`.justify-between`**: Distributes items evenly, with the first item at the start and the last item at the end.  
- **`.justify-around`**: Distributes items with equal space around them.  
- **`.justify-evenly`**: Distributes items with equal space between them.  
- **`.items-start`**: Aligns items to the top of the container.  
- **`.items-center`**: Aligns items to the center of the container.  
- **`.items-end`**: Aligns items to the bottom of the container.  
- **`.items-stretch`**: Stretches items to fill the container (default).  

### Example:
```html
<div class="flex justify-between items-center">
  <div class="p-4 bg-green-200">Item 1</div>
  <div class="p-4 bg-green-300">Item 2</div>
  <div class="p-4 bg-green-400">Item 3</div>
</div>
```

---

## Flex Direction

- **`.flex-row`**: Horizontal direction (default).  
- **`.flex-row-reverse`**: Horizontal direction, reversed.  
- **`.flex-col`**: Vertical direction.  
- **`.flex-col-reverse`**: Vertical direction, reversed.  

### Example:
```html
<div class="flex flex-col-reverse">
  <div class="p-4 bg-red-200">Item 1</div>
  <div class="p-4 bg-red-300">Item 2</div>
  <div class="p-4 bg-red-400">Item 3</div>
</div>
```

---

## Order

- **`.order-{number}`**: Controls the order of items. Lower numbers are displayed first.
- **`.order-first`**, **`.order-last`**, **`.order-none`** for specific placement.

### Example:
```html
<div class="flex">
  <div class="order-2 p-4 bg-purple-200">Item 1</div>
  <div class="order-1 p-4 bg-purple-300">Item 2</div>
  <div class="order-3 p-4 bg-purple-400">Item 3</div>
</div>
```

---

