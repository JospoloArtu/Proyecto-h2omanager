# 💧 H2O Manager - Sistema de Gestión de Botellones

Sistema completo de gestión para distribuidoras de agua purificada en botellones. Desarrollado con React + Vite para ofrecer una experiencia moderna, rápida e intuitiva.

## 🌟 Características Principales

### 📊 Dashboard Analítico

- Vista general de ventas y estadísticas en tiempo real
- Gráficos interactivos de rendimiento
- Indicadores clave de negocio (KPIs)
- Resumen de clientes activos y morosos

### 👥 Gestión de Clientes

- **Registro completo de clientes** con información detallada
- Búsqueda y filtrado avanzado
- Estados de cuenta: Activo, Moroso, Inactivo
- Control de saldos y cuentas por cobrar
- Vista de historial de compras por cliente
- Diseño moderno con avatares personalizados

### 💰 Módulo de Ventas Inteligente

- **Wizard de ventas en 4 pasos** para proceso guiado
  1. **Selección de cliente**: Registrado o nuevo cliente express
  2. **Productos**: Catálogo visual con stock en tiempo real
  3. **Resumen y pago**: Métodos de pago y notas
  4. **Confirmación**: Resumen final e impresión de factura

- **Características destacadas:**
  - ✅ Registro rápido de clientes no registrados
  - ✅ Productos con capacidad específica (15L, 20L)
  - ✅ Visualización de stock disponible
  - ✅ Carrito de compras interactivo
  - ✅ **Precios duales**: USD y Bolívares con conversión automática
  - ✅ Múltiples métodos de pago
  - ✅ **Impresión de facturas** con todos los detalles

### ⚙️ Configuración Avanzada

- **Gestión de usuarios** del sistema
- **Configuración de moneda**
  - Moneda principal: Bolívares (VES)
  - Tasa de cambio configurable
  - IVA personalizable
  - Visualización dual en toda la aplicación
- **Cambio de contraseña** con validaciones de seguridad
- **Precios por litro** configurables
  - Precio base por litro
  - Botellones de 18L y 20L
  - Tarifa de delivery
- **Configuración general** de la empresa

### 🎨 Diseño y UX

- Interfaz moderna y profesional
- Diseño responsive (Desktop, Tablet, Mobile)
- Animaciones suaves y transiciones
- Notificaciones toast interactivas
- Sidebar colapsable
- Tema de colores consistente
- Iconografía con react-icons

## 🛠️ Tecnologías Utilizadas

### Frontend

- **React 18** - Biblioteca de UI
- **Vite** - Build tool y dev server ultrarrápido
- **React Router DOM** - Navegación
- **React Hot Toast** - Notificaciones elegantes
- **React Icons** - Iconografía completa

### Estilos

- **CSS Modules** - Estilos modulares
- **CSS Custom Properties** - Variables CSS
- **Flexbox & Grid** - Layouts modernos
- **Gradientes y Animaciones** - UI premium

### Gestión de Estado

- **React Context API** - Estado global compartido
- **LocalStorage** - Persistencia de configuración
- **Custom Hooks** - Lógica reutilizable

### Servicios

- Arquitectura modular con servicios separados
- Preparado para integración con backend REST API

## 📦 Instalación

### Requisitos Previos

- Node.js 16+
- npm o yarn

### Pasos de Instalación

1. **Clonar el repositorio**

```bash
git clone <url-del-repositorio>
cd Proyecto
```

2. **Instalar dependencias**

```bash
npm install
```

3. **Iniciar servidor de desarrollo**

```bash
npm run dev
```

4. **Abrir en el navegador**

```
http://localhost:5173
```

## 🚀 Scripts Disponibles

```bash
# Modo desarrollo
npm run dev

# Compilar para producción
npm run build

# Vista previa de producción
npm run preview

# Linter
npm run lint
```

## 📁 Estructura del Proyecto

```
Proyecto/
├── src/
│   ├── components/          # Componentes reutilizables
│   │   ├── Navbar.jsx       # Barra de navegación superior
│   │   └── Sidebar.jsx      # Menú lateral
│   │
│   ├── context/             # Contextos globales
│   │   ├── AuthContext.jsx  # Autenticación
│   │   └── ConfigContext.jsx # Configuración global
│   │
│   ├── pages/               # Páginas principales
│   │   ├── Dashboard.jsx    # Dashboard principal
│   │   ├── Clientes.jsx     # Gestión de clientes
│   │   ├── Ventas.jsx       # Módulo de ventas
│   │   ├── Configuracion.jsx # Configuración
│   │   └── Login.jsx        # Autenticación
│   │
│   ├── services/            # Servicios y API
│   │   ├── api.js          # Cliente HTTP base
│   │   └── dataService.js  # Servicios CRUD
│   │
│   ├── styles/              # Estilos CSS
│   │   ├── App.css
│   │   ├── Clientes.css
│   │   ├── Ventas.css
│   │   ├── Configuracion.css
│   │   └── ...
│   │
│   ├── App.jsx              # Componente raíz
│   └── main.jsx             # Punto de entrada
│
├── public/                  # Archivos estáticos
├── index.html              # HTML base
├── package.json            # Dependencias
├── vite.config.js          # Configuración Vite
└── README.md               # Este archivo
```

## 🎯 Uso

### Login

El sistema incluye autenticación mockup. Credenciales de prueba:

- **Usuario**: admin
- **Contraseña**: admin123

### Configurar Tasa de Cambio

1. Ve a **Configuración → Moneda**
2. Ajusta la **Tasa de Cambio** (ej: 36.5)
3. Guarda los cambios
4. Los precios se actualizarán automáticamente en todo el sistema

### Realizar una Venta

1. Ve al módulo **Ventas**
2. **Paso 1**: Selecciona un cliente o registra uno nuevo
3. **Paso 2**: Agrega productos al carrito
4. **Paso 3**: Revisa el resumen y selecciona método de pago
5. **Paso 4**: Confirma e imprime la factura

### Gestionar Clientes

1. Accede a **Clientes**
2. Usa la barra de búsqueda para filtrar
3. Clic en un cliente para ver detalles
4. Usa los botones para editar o eliminar

## 💡 Características Destacadas

### Precios Duales (USD/Bs)

- Todos los precios se muestran en **dólares** y **bolívares**
- Conversión automática basada en la tasa configurada
- Actualización en tiempo real al cambiar la tasa

### Sistema de Facturas

- Generación automática de facturas
- Incluye toda la información del cliente y productos
- Formato profesional para impresión
- Conversión de precios incluida

### Responsive Design

- Adaptable a cualquier dispositivo
- Mobile-first approach
- Grid system flexible

## 🔧 Configuración Avanzada

### Variables de Entorno

Crea un archivo `.env` en la raíz:

```env
VITE_API_BASE_URL=http://localhost:3000/api
VITE_APP_NAME=H2O Manager
```

### Backend API

El sistema está preparado para conectarse a un backend REST. Edita `src/services/api.js` para configurar la URL base.

## 📝 Próximas Características

- [ ] Integración con backend real
- [ ] Reportes y estadísticas avanzadas
- [ ] Gestión de proveedores
- [ ] Módulo de servicios
- [ ] Sistema de rutas de delivery
- [ ] Exportación de datos (Excel, PDF)
- [ ] Notificaciones push
- [ ] Multi-usuario con roles

## 🤝 Contribuciones

Las contribuciones son bienvenidas. Por favor:

1. Fork el proyecto
2. Crea una rama para tu feature (`git checkout -b feature/AmazingFeature`)
3. Commit tus cambios (`git commit -m 'Add some AmazingFeature'`)
4. Push a la rama (`git push origin feature/AmazingFeature`)
5. Abre un Pull Request

## 📄 Licencia

Este proyecto está bajo la Licencia MIT.

## 👨‍💻 Autor

Desarrollado con ❤️ para optimizar la gestión de distribuidoras de agua

## 📞 Soporte

Para reportar bugs o solicitar features, abre un issue en el repositorio.

---

**H2O Manager** - Gestión inteligente para tu negocio de agua 💧
