# WhatsApp Clone - Trabajo Final 

## Descripción del Desafío

Este proyecto es un clon funcional de WhatsApp desarrollado como desafío técnico. La aplicación replica las funcionalidades principales de WhatsApp incluyendo:

- Lista de chats con búsqueda en tiempo real
- Chat individual con envío de mensajes
- Información detallada de contactos
- Navegación fluida entre diferentes vistas
- Diseño responsive y accesible

## Funcionalidades Implementadas

### 🏠 Página Principal (\`/\`)
- Lista de chats con avatares y últimos mensajes
- Barra de búsqueda funcional
- Navegación por pestañas (Chats, Novedades, Comunidades, Llamadas)
- Contadores de mensajes no leídos

### 💬 Chat Individual (\`/message/:id\`)
- Vista de conversación completa
- Envío de mensajes en tiempo real
- Respuestas automáticas simuladas
- Header con información del contacto
- Botones de acción (llamada, videollamada)

### 👤 Información de Contacto (\`/contactInfo/:id\`)
- Detalles completos del contacto
- Avatar, nombre, estado y número
- Opciones de interacción
- Historial de medios compartidos

## Librerías Utilizadas

### Dependencias Principales
- **React 18**: Framework principal para la interfaz de usuario
- **React Router DOM 6**: Manejo de rutas y navegación
- **Lucide React**: Iconografía moderna y consistente

### Dependencias de Desarrollo
- **Next.js 14**: Framework de React para desarrollo y producción
- **Tailwind CSS**: Framework de utilidades CSS (solo para componentes base)

## Arquitectura del Proyecto

\`\`\`
src/
├── components/
│   ├── common/           # Componentes reutilizables
│   ├── chat/            # Componentes específicos de chat
│   └── ui/              # Componentes de interfaz base
├── context/             # Contextos de React
├── pages/               # Páginas principales
├── styles/              # Estilos CSS puros
├── utils/               # Utilidades y helpers
└── data/                # Datos simulados
\`\`\`

## Características Técnicas

### 🎯 Cumplimiento de Especificaciones

✅ **Responsividad**: Diseño adaptativo de 320px a 2000px  
✅ **Accesibilidad**: Contrastes adecuados y navegación por teclado  
✅ **React**: Desarrollado completamente en React 18  
✅ **Estados**: Uso extensivo de useState y useReducer  
✅ **Contextos**: Context API para estado global  
✅ **React Router**: Enrutamiento completo con parámetros  
✅ **Formularios**: Múltiples formularios funcionales  
✅ **Componentes**: Arquitectura modular y reutilizable  
✅ **Múltiples Páginas**: 3 páginas principales con parámetros  

### 🏗️ Principios de Programación

- **DRY (Don't Repeat Yourself)**: Componentes reutilizables y hooks personalizados
- **YAGNI (You Aren't Gonna Need It)**: Implementación enfocada en requisitos específicos
- **KISS (Keep It Simple, Stupid)**: Código limpio y fácil de mantener

## Dificultades Presentadas y Soluciones

### 1. **Gestión de Estado Complejo**
**Problema**: Manejar el estado de múltiples chats, mensajes y navegación.  
**Solución**: Implementación de Context API con useReducer para estado global centralizado.

### 2. **Enrutamiento Dinámico**
**Problema**: Navegación fluida entre diferentes vistas con parámetros.  
**Solución**: Uso de React Router DOM con parámetros dinámicos y navegación programática.

### 3. **Responsividad Extrema**
**Problema**: Mantener funcionalidad en rangos de 320px a 2000px.  
**Solución**: CSS Grid y Flexbox con media queries específicas y diseño mobile-first.

### 4. **Accesibilidad en Tema Oscuro**
**Problema**: Mantener contraste adecuado en diferentes temas.  
**Solución**: Paleta de colores cuidadosamente seleccionada con ratios de contraste WCAG AA.

### 5. **Simulación Realista**
**Problema**: Crear una experiencia convincente sin backend real.  
**Solución**: Datos simulados con respuestas automáticas y persistencia en localStorage.

## Instalación y Uso

\`\`\`bash
# Clonar el repositorio
git clone [url-del-repositorio]

# Instalar dependencias
npm install

# Ejecutar en desarrollo
npm run dev

# Construir para producción
npm run build
\`\`\`

## Estructura de Rutas

- \`/\` - Página principal con lista de chats
- \`/message/:id\` - Chat individual con ID específico
- \`/contactInfo/:id\` - Información detallada del contacto

## Consideraciones de Accesibilidad

- Contraste mínimo WCAG AA (4.5:1)
- Navegación por teclado completa
- Etiquetas ARIA apropiadas
- Texto alternativo para imágenes
- Indicadores de estado para lectores de pantalla

## Optimizaciones Implementadas

- Lazy loading de componentes
- Memoización de componentes pesados
- Debounce en búsquedas
- Optimización de re-renders
- CSS puro para mejor rendimiento

---

**Desarrollado con ❤️ usando React y CSS puro**