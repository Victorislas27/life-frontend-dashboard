# B-Life Store - Frontend Dashboard (Nuxt 3 + Quasar)

Dashboard administrativo interactivo desarrollado en **Nuxt 3 (Vue 3)** y componentes de **Quasar Framework**, diseñado para conectarse a la API REST Serverless de B-Life.

---

## 🚀 Características

1. **Gestión de Catálogo y Productos:**
   - Creación y edición de productos con múltiples presentaciones/variantes.
   - Validación de SKUs únicos por variante.
   - Listado paginado con filtros en tiempo real (búsqueda por nombre/descripción y categoría).
   - Acciones de eliminación segura y visualización de variantes asociadas.

2. **Registro y Consulta de Ventas:**
   - Alta de órdenes de venta especificando canal (Amazon, Mercado Libre, Shopify, etc.).
   - Selección dinámica de productos y cálculo automático de totales e inventarios.
   - Historial paginado con filtros por canal, estado y rango de fechas.

3. **Dashboard de Indicadores Clave (KPIs):**
   - **Top Productos:** Ranking de los suplementos más vendidos por unidades e ingresos.
   - **Rentabilidad Financiera:** Cálculo de margen bruto (%) y utilidad neta por canal o período.
   - **Participación por Canal:** Porcentaje de ventas distribuido entre canales de distribución.
   - **Recomendaciones Cruzadas:** Productos frecuentemente comprados juntos para estrategias de cross-selling.

---

## 🛠️ Tecnologías

- **Framework:** Nuxt 3 (SSR desactivado, modo SPA para dashboard)
- **UI & Componentes:** Quasar Framework v2
- **Librería de Iconos:** Material Icons + Roboto Font
- **Cliente HTTP:** Ofetch ($fetch integrado en Nuxt)
- **Gestor de Paquetes:** pnpm

---

## ⚙️ Instalación y Uso

### 1. Requisitos Previos
- Node.js >= 20.x
- pnpm instalado (`npm install -g pnpm`)
- API Serverless de B-Life en ejecución (por defecto en `http://localhost:3000/api`)

### 2. Configurar Variables de Entorno
```bash
cp .env.example .env
```
Ajusta la URL de la API si es necesario en `.env`:
```env
API_BASE_URL=http://localhost:3000/api
```

### 3. Instalar Dependencias
```bash
pnpm install
```

### 4. Modo Desarrollo
```bash
pnpm dev
```
La aplicación estará disponible en [http://localhost:3001](http://localhost:3001).

### 5. Compilación para Producción
```bash
pnpm build
```
O para previsualizar el build de producción:
```bash
pnpm preview
```
