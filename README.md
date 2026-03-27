# SSL — Dashboard de Estudio

Dashboard interactivo para preparar el examen final de **Sintaxis y Semantica de los Lenguajes** (SSL) — UTN FRM, ISI 2026.

**[Abrir Dashboard](https://jbarrancogit.github.io/dashboard-ssl-utn/)**

---

## Que es

Un archivo HTML autocontenido que funciona como plataforma completa de estudio. Reemplaza bibliografia, campus y apuntes en un solo lugar. Todo el progreso se guarda en localStorage del navegador.

## Modulos

| Modulo | Descripcion |
|--------|-------------|
| **Panel Principal** | Progreso general, racha de estudio, meta semanal, estadisticas por unidad |
| **Ejercicios** | 82 ejercicios con enunciado y solucion completa, organizados por unidad (U1-U7) |
| **Teoria** | Tarjetas de teoria expandibles con contenido completo de las 7 unidades |
| **Flashcards** | 35 flashcards interactivas con flip, filtro por unidad y tracking de dominio |
| **Practica Oral** | Simulador de coloquio (3ra etapa): sortea unidad, lista temas, califica practica |
| **Modo Examen** | Simulador de las 3 etapas del examen real con timer (cuestionario 50min, problemas 40min) |
| **Examenes Probables** | 10 modelos de examen con resoluciones completas basados en frecuencia real |
| **Material Campus** | Links a videos de la catedra, TPs, bibliografia y recursos del campus |
| **Pomodoro** | Timer 50/10 con estadisticas de sesiones y horas acumuladas |
| **Plan Semanal** | Plan de 4 semanas con milestones y checkboxes de progreso |
| **Prediccion Final** | Analisis estadistico de ~35 examenes reales, banco de frases, V/F, errores S/SE/SD, 10 simulacros formato Campus |

## Prediccion de examen

El modulo de prediccion esta basado en el analisis exhaustivo de **142 archivos** (imagenes JPG, PDFs, DOCX) de examenes finales y globales de la catedra Leon/Brachetta (2015-2026):

- **Pasada 1:** Lectura visual de 109 imagenes de examenes fotografiados
- **Pasada 2:** Extraccion de 113 paginas de PDFs-imagen con pymupdf + 4 DOCX con python-docx
- Se excluyeron 2 examenes de Paradigmas de Programacion mezclados en la carpeta
- **~35 examenes SSL unicos** verificados contra el programa oficial de 7 unidades

### Frecuencia real de temas

| # | Tema | Frecuencia |
|---|------|-----------|
| 1 | AFD/AFND (construir, minimizar, convertir) | 94% |
| 2 | Alcance est/din + vinculacion prof/superf | 91% |
| 3 | Registros de activacion / Stack / Display | 89% |
| 4 | Gramaticas: Chomsky, BNF, EBNF, diagramas | 83% |
| 5 | Analisis errores en codigo C/JS | 71% |
| 6 | Completar frases / definiciones | 66% |
| 7 | Tipos datos / memoria / arreglos | 63% |
| 8 | Expresiones regulares | 51% |
| 9 | Pasaje de parametros | 49% |
| 10 | Automatas de pila | 43% |

### Tendencias 2024-2026

- Clasificacion de errores S/SE/SD y punteros/malloc en C estan **creciendo**
- Automatas de pila esta **decreciendo**
- V/F y multiple choice son mas frecuentes en formato Campus digital

## Features

- **Dark mode** con toggle y persistencia (46 reglas CSS dedicadas)
- **Busqueda global** con shortcut `/` — busca en ejercicios, teoria, flashcards, quiz y frases
- **Sidebar navigation** en desktop, hamburger menu en mobile
- **SOS Ansiedad** — respiracion 4-7-8 y tips para manejar nervios en el examen
- **Responsive** — funciona en desktop, tablet y celular
- **Offline** — no requiere conexion despues de cargar

## Las 7 unidades de SSL

1. **U1** — Gramaticas y lenguajes formales (Chomsky, BNF, EBNF, notaciones)
2. **U2** — Maquinas secuenciales y automatas (AFD, AFND, AP, Moore/Mealy, Turing)
3. **U3** — Maquinas y lenguajes (analisis lexico, parsers LL/LR, semanticas)
4. **U4** — Lenguajes y traductores (compiladores, interpretes, tabla de simbolos)
5. **U5** — Semantica de enunciados (sentencias de control, codigo intermedio)
6. **U6** — Semantica de datos (tipos, memoria, arreglos, GC, punteros)
7. **U7** — Semantica de subprogramas (parametros, registros de activacion, alcance)

## Datos de la materia

| Campo | Detalle |
|-------|---------|
| Codigo | 13 |
| Profesor titular | Leon, Oscar Alfredo |
| Adjunta | Brachetta, Mariana Ines |
| Horas catedra | 128 (64 teoria + 64 practica) |
| Formato examen | 3 etapas: cuestionario (50min) + problemas (40min) + coloquio oral (20min) |
| Aprobacion | 60% minimo en cada etapa |

## Stack

- HTML + CSS + vanilla JS (archivo unico, sin dependencias)
- GitHub Pages para hosting
- localStorage para persistencia de progreso

---

*Juan Ignacio Barranco Bastan — Leg. 44041 — UTN FRM — ISI 2026*
