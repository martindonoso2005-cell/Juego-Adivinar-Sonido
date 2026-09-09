# Juego de Adivinar el Sonido (Experiencia Educativa Interactiva)
**Asignatura:** Taller de Interfaces (2026) | Universidad Adolfo Ibáñez  
**Estudiante:** Martín Donoso  
**Profesor:** Jorge Forero  
**Aplicación Web:** [Ver Juego Desplegado](https://martindonoso2005-cell.github.io/Juego-Adivinar-Sonido/)  

---

## 1. Concepto Pedagógico y Mecánica de Interacción
La aplicación consiste en una experiencia educativa e interactiva diseñada para el entrenamiento auditivo y la asociación de estímulos acústicos. A diferencia de interfaces con sonido pasivo o música de fondo, en este juego el audio actúa como interfaz activa principal de toma de decisiones.

* **Tema:** Reconocimiento y discriminación auditiva de animales.
* **Mecánica Lúdica:** El sistema reproduce un estímulo sonoro aleatorio y el usuario debe identificar a qué animal corresponde entre las opciones presentadas.
* **Feedback:** Proporciona retroalimentación inmediata (sonora/visual) ante aciertos y errores.

---

## 2. Banco de Sonidos y Edición de Audio
El proyecto integra 7 registros de audio de animales recortados y procesados individualmente para su interacción web:

| Archivo | Elemento Representado | Formato |
| :--- | :--- | :--- |
| `cerdo.wav` | Cerdo | WAV Audio |
| `gallina.wav` | Gallina | WAV Audio |
| `gato.wav` | Gato | WAV Audio |
| `leon.wav` | León | WAV Audio |
| `oveja.wav` | Oveja | WAV Audio |
| `perro.wav` | Perro | WAV Audio |
| `pollito.wav` | Pollito | WAV Audio |
| `vaca.wav` | Vaca | WAV Audio |

* **Tratamiento Técnico:** Recortes de transientes, normalización de volumen y limpieza para garantizar que los audios se reproduzcan de forma clara y sin latencia al activarse por la interacción del usuario.

---

## 3. Diagrama de Flujo del Juego

```text
[ INICIO ]
    │
    ▼
[ Carga de la aplicación web (index.html) ]
    │
    ▼
[ Sistema selecciona y reproduce un estímulo sonoro (.wav) ]
    │
    ▼
[ Usuario escucha y selecciona una opción ]
    │
    ├─► ¿Opción Correcta?
    │       ├── SÍ ──► Feedback de acierto
    │       └── NO ──► Feedback de error
    │
    ▼
[ Sistema pasa al siguiente estímulo sonoro ]
