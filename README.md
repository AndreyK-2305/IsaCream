# Isa Cream Inventory

Aplicacion Next.js para controlar inventario, ventas y reportes de Isa Cream.

## Setup

1. Instala dependencias:

```bash
npm install
```

2. Crea un proyecto en Supabase y ejecuta `supabase/schema.sql` en el SQL Editor.

3. Copia `.env.example` a `.env.local` y configura:

```bash
NEXT_PUBLIC_SUPABASE_URL=...
NEXT_PUBLIC_SUPABASE_PUBLISHABLE_KEY=...
```

4. Ejecuta la app:

```bash
npm run dev
```

## Notas

- El catalogo base se puede cargar desde Inventario con el boton "Cargar menu base".
- Las ventas se registran con una funcion transaccional de Supabase para descontar stock de forma segura.
- La primera version usa un usuario administrador autenticado en Supabase Auth.
