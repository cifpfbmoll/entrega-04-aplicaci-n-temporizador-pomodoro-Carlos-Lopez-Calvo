[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/c6IViGy8)

# 🍅 Pomodoro Timer App

Una aplicación moderna de temporizador Pomodoro construida con Angular 20, diseñada para mejorar la productividad mediante la técnica Pomodoro. Cuenta con un diseño dark mode elegante con efectos glassmorfismo y una interfaz intuitiva.

## ✨ Características

- **⏱️ Temporizador Pomodoro Completo**
  - Sesiones de trabajo personalizables
  - Descansos cortos y largos
  - Transición automática entre sesiones
  - Contador de sesiones completadas

- **🎨 Interfaz Moderna**
  - Diseño dark mode con tema cyan/turquesa
  - Efectos de glassmorfismo y backdrop blur
  - Animaciones suaves y transiciones elegantes
  - Barra de progreso animada con efectos shimmer
  - Diseño responsive para móviles y escritorio

- **⚙️ Configuración Personalizable**
  - Duración de sesión de trabajo (1-60 minutos)
  - Duración de descanso corto (1-60 minutos)
  - Duración de descanso largo (1-60 minutos)
  - Número de sesiones antes del descanso largo (1-10)

- **🔊 Notificaciones de Audio**
  - Sonido de notificación al completar cada sesión
  - Audio generado mediante Web Audio API

- **♿ Accesibilidad**
  - Navegación por teclado completa
  - Etiquetas ARIA para lectores de pantalla
  - Roles semánticos apropiados

## 🛠️ Tecnologías Utilizadas

- **Framework**: Angular 20.3.8 (Standalone Components)
- **Lenguaje**: TypeScript 5.7
- **Estilos**: SCSS con animaciones CSS personalizadas
- **Gestión de Estado**: Angular Signals
- **Iconos**: Lucide Angular
- **Build**: Angular CLI con optimizaciones de producción

## 📦 Instalación

1. **Clonar el repositorio**
```bash
git clone <repository-url>
cd entrega-04-aplicaci-n-temporizador-pomodoro-Carlos-Lopez-Calvo
```

2. **Instalar dependencias**
```bash
npm install
```

3. **Iniciar el servidor de desarrollo**
```bash
ng serve
```

4. **Abrir en el navegador**
```
http://localhost:4200/
```

## 🚀 Comandos Disponibles

| Comando | Descripción |
|---------|-------------|
| `ng serve` | Inicia el servidor de desarrollo |
| `ng build` | Compila el proyecto para producción |
| `ng test` | Ejecuta las pruebas unitarias |
| `npm start` | Alias para `ng serve` |

## 📁 Estructura del Proyecto

```
src/
├── app/
│   ├── components/
│   │   ├── timer/              # Componente principal del temporizador
│   │   │   ├── timer.component.ts
│   │   │   ├── timer.component.html
│   │   │   └── timer.component.scss
│   │   └── settings/           # Componente de configuración
│   │       ├── settings.component.ts
│   │       ├── settings.component.html
│   │       └── settings.component.scss
│   ├── services/
│   │   └── pomodoro.service.ts # Lógica del temporizador Pomodoro
│   ├── app.ts                  # Componente raíz
│   ├── app.html
│   ├── app.scss
│   └── app.config.ts           # Configuración de la aplicación
├── styles.scss                 # Estilos globales
└── index.html
```

## 🎯 Uso de la Aplicación

1. **Iniciar una sesión**: Haz clic en el botón "Iniciar" para comenzar una sesión de trabajo
2. **Pausar/Reanudar**: Usa el botón de pausa para pausar y reanudar el temporizador
3. **Detener**: Detiene el temporizador y lo reinicia al tiempo original
4. **Saltar**: Salta a la siguiente sesión (trabajo o descanso)
5. **Reiniciar**: Reinicia todo el ciclo Pomodoro
6. **Configurar**: Abre el modal de configuración para personalizar los tiempos

## 🔄 Ciclo Pomodoro

La aplicación implementa el ciclo clásico de Pomodoro:

1. 🔴 **Sesión de Trabajo** (25 min por defecto)
2. 🟢 **Descanso Corto** (5 min por defecto)
3. 🔴 **Sesión de Trabajo** (25 min)
4. 🟢 **Descanso Corto** (5 min)
5. 🔴 **Sesión de Trabajo** (25 min)
6. 🟢 **Descanso Corto** (5 min)
7. 🔴 **Sesión de Trabajo** (25 min)
8. 🔵 **Descanso Largo** (15 min por defecto)

Después del descanso largo, el ciclo se repite.

## 🎨 Características de Diseño

- **Tema Dark Mode**: Colores oscuros navy/slate para reducir la fatiga visual
- **Gradientes Luminosos**: Efectos cyan/turquesa con resplandor
- **Glassmorfismo**: Tarjetas translúcidas con backdrop blur
- **Animaciones**: Transiciones suaves con cubic-bezier personalizado
- **Efectos de Hover**: Elevación y sombras brillantes en botones
- **Barra de Progreso**: Animación shimmer continua con resplandor

## 🧩 Componentes Principales

### PomodoroService
Servicio principal que gestiona:
- Estado del temporizador (usando Angular Signals)
- Lógica del ciclo Pomodoro
- Configuración personalizable
- Notificaciones de audio

### TimerComponent
Muestra:
- Temporizador con cuenta regresiva
- Barra de progreso visual
- Controles (Iniciar/Pausar/Detener/Saltar/Reiniciar)
- Contador de sesiones completadas

### SettingsComponent
Permite configurar:
- Duración de las sesiones
- Número de sesiones antes del descanso largo
- Modal con validación de valores

## 🌐 Compatibilidad

- Chrome/Edge 90+
- Firefox 88+
- Safari 14+
- Opera 76+

## 📝 Notas Técnicas

- Utiliza **Angular Signals** para gestión de estado reactivo
- Componentes **standalone** (sin módulos NgModule)
- **Web Audio API** para notificaciones sonoras
- **CSS Grid** y **Flexbox** para layouts responsive
- **SCSS** con variables CSS personalizadas
- **TypeScript** con tipado estricto

## 🔮 Mejoras Futuras

- [ ] Persistencia de datos en localStorage
- [ ] Historial de sesiones completadas
- [ ] Gráficos de productividad
- [ ] Temas de color personalizables
- [ ] Notificaciones del navegador
- [ ] Sonidos personalizables
- [ ] Integración con calendario
- [ ] Modo enfocado sin distracciones

## 👨‍💻 Autor

Carlos López Calvo

## 📄 Licencia

Este proyecto fue desarrollado como parte de una asignación académica.

---

**Generado con** [Angular CLI](https://github.com/angular/angular-cli) version 20.3.8
