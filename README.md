# 🐺 Sistema Fenrir — Terminal de Activación Táctica

**Sistema Fenrir** es una interfaz web inmersiva diseñada para activar "protocolos" mentales y físicos orientados al rendimiento. Inspirada en una terminal de control táctico, permite al usuario entrar en diferentes estados de flujo (deportivo, analítico y social) mediante secuencias de pasos, feedback visual y un sistema de gamificación.

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)

---

## 📋 Índice

- [Características principales](#-características-principales)
- [Protocolos disponibles](#-protocolos-disponibles)
- [Sistema de logros](#-sistema-de-logros)
- [Atajos de teclado](#-atajos-de-teclado)
- [Persistencia de datos](#-persistencia-de-datos)
- [Instalación y uso](#-instalación-y-uso)
- [Tecnologías utilizadas](#-tecnologías-utilizadas)
- [Capturas de pantalla](#-capturas-de-pantalla)
- [Mejoras futuras](#-mejoras-futuras)

---

## ✨ Características principales

- **3 Protocolos Tácticos**: Cada uno enfocado en un área de rendimiento diferente (deporte, estudio, liderazgo social).
- **Secuencia de Activación Inmersiva**: Barra de progreso + logs en tiempo real que simulan la carga del sistema.
- **Arte ASCII Dinámico**: La mascota Fenrir (lobo) cambia de aspecto visual según el protocolo activo.
- **Estadísticas de Uso**: Contador de activaciones y fecha del último uso para cada protocolo, guardado automáticamente.
- **Sistema de Logros (Gamificación)**: 5 logros desbloqueables con notificaciones emergentes (*toasts*) y un modal dedicado.
- **Interfaz Terminal Oscura**: Estética CRT, micro-interacciones, efectos neón y animaciones suaves.
- **Atajos de Teclado**: Navegación rápida sin necesidad de usar el ratón.
- **Persistencia Total**: Los datos (estadísticas, logros y protocolo activo) se guardan en `localStorage` y `sessionStorage`.

---

## 🎯 Protocolos disponibles

| Icono | Protocolo     | Objetivo                         | Estado activo  |
|-------|---------------|----------------------------------|----------------|
| 🐺    | **Fenrir-Furia**  | Dominación deportiva (Fútbol)    | MODO SALVAJE   |
| 🧠    | **Fenrir-Mente**  | Precisión analítica (Exámenes)   | MODO ANÁLISIS  |
| 👑    | **Fenrir-Apex**   | Presencia y carisma absoluto     | MODO ALFA      |

Cada protocolo contiene una secuencia de **4 pasos tácticos** que el usuario debe seguir para "activar" ese estado mental/físico.

---

## 🏆 Sistema de logros

El sistema monitoriza tu actividad y desbloquea logros automáticamente. Cuando consigues uno, aparece una notificación en la esquina inferior derecha y se actualiza el contador en el botón `🏆 Logros`.

| Logro               | Icono | Condición para desbloquear                        |
|---------------------|-------|---------------------------------------------------|
| **Primera Activación** | 🌟    | Activar cualquier protocolo por primera vez.      |
| **Maestro Furia**      | 🐺    | Activar `Fenrir-Furia` un total de 5 veces.       |
| **Maestro Mente**      | 🧠    | Activar `Fenrir-Mente` un total de 5 veces.       |
| **Maestro Apex**       | 👑    | Activar `Fenrir-Apex` un total de 5 veces.        |
| **Trifecta**           | 🔥    | Activar los 3 protocolos en un mismo día natural. |

---

## ⌨️ Atajos de teclado

| Tecla | Acción                                        |
|-------|-----------------------------------------------|
| `1`   | Activar el primer protocolo (**Fenrir-Furia**)  |
| `2`   | Activar el segundo protocolo (**Fenrir-Mente**) |
| `3`   | Activar el tercer protocolo (**Fenrir-Apex**)   |
| `ESC` | Volver al menú principal (cierra vistas y modales) |

---

## 💾 Persistencia de datos

Toda la información del usuario se guarda de forma local en el navegador:

| Clave en `localStorage`      | Contenido                                      |
|------------------------------|------------------------------------------------|
| `fenrir_stats`               | Objeto JSON con el contador y fecha de uso de cada protocolo. |
| `fenrir_achievements`        | Objeto JSON con el estado (desbloqueado/no) de cada logro. |
| `fenrir_last_protocol`       | (Opcional) Último protocolo usado.             |

| Clave en `sessionStorage`    | Contenido                                      |
|------------------------------|------------------------------------------------|
| `fenrir_active`              | ID del protocolo que está actualmente activo (para restaurar la sesión al recargar). |

---

## 🚀 Instalación y uso

Este proyecto es 100% frontend y no requiere dependencias externas ni servidores.

1. **Clona el repositorio** (o descarga el archivo `index.html`):
   ```bash
   git clone https://github.com/tu-usuario/sistema-fenrir.git
