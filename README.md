# 🎓 Simulacro de Examen Integrador: Teoría (TP1–TP5) y Práctica en PROLOG (TP7)
## Cátedra: Laboratorio I (Inteligencia Artificial y Agentes Racionales)
### Universidad Católica de Santiago del Estero (UCSE) — Departamento Académico San Salvador (DASS)
**Carrera:** Tecnicatura Universitaria en Automatización y Robótica / Informática  
**Docente / Jefe de Trabajos Prácticos (JTP):** Ing. Fabio D. Argañaraz  
**Ciclo Lectivo:** 2026 • **Duración Sugerida:** 90 Minutos • **Puntaje Total:** 100 Puntos  

---

## 📋 Estructura del Simulacro (100 Puntos)

### 📘 Parte I: Evaluación Teórico-Conceptual (50 Puntos — 5 Ejercicios × 10 Puntos)
1. **Ejercicio T1 (TP1 — 10 pts):** Cuadrante de 4 dimensiones de Russell & Norvig, ciclo sensorial-motor, función vs. programa de agente, especificación PEAS de vehículo autónomo y Test de Turing Total.
2. **Ejercicio T2 (TP2 — 10 pts):** Formulación formal de problemas de búsqueda, distinción ontológica Nodo vs. Estado, y comparación estructural entre BFS (FIFO, $O(b^d)$) y DFS (LIFO, $O(b \cdot m)$).
3. **Ejercicio T3 (TP3 — 10 pts):** Búsqueda Voraz Primero el Mejor ($f(n)=h(n)$ y trampa de Iasi $\rightarrow$ Neamt), función de evaluación de $A^*$ ($f(n)=g(n)+h(n)$) y admisibilidad en árboles ($h(n) \le h^*(n)$).
4. **Ejercicio T4 (TP4 — 10 pts):** Arquitectura de agentes basados en conocimiento (KB + Motor de inferencia), sintaxis vs. semántica, robustez (*soundness*) y clasificación de sentencias proposicionales.
5. **Ejercicio T5 (TP5 — 10 pts):** Compromiso ontológico de LPO vs. lógica proposicional, taxonomía sintáctica (constantes, funciones, predicados, variables) y conectivos canónicos de cuantificadores ($\forall \Rightarrow$, $\exists \land$).

### 💻 Parte II: Evaluación Práctica en PROLOG (50 Puntos = 26 pts KB + 24 pts Consultas)
Cada caso práctico (25 pts) se divide en **Sección A (13 pts: 9 hechos $\times 1\text{ pt}$ + 2 reglas $\times 2\text{ pts}$)** codificada en el Editor de Base de Conocimientos con Linter Sintáctico en Tiempo Real y evaluada por normalización $\alpha$-canónica, y **Sección B (12 pts: 6 consultas $\times 2\text{ pts}$)**:
1. **Ejercicio P1 (`caso1_hospital.pl` — 25 pts): Guardia y Triaje del Hospital Universitario**
   - Modelado de médicos, especialidades (`cardiologia`, `traumatologia`, `pediatria`), turnos (`manana`, `noche`) y nivel de complejidad (`alta`, `media`).
   - Reglas deductivas: `guardia_critica(Medico)` y `especialista_manana(Medico, Especialidad)`.
2. **Ejercicio P2 (`caso2_agro_iot.pl` — 25 pts): Red de Sensores IoT y Riego Inteligente Agroindustrial**
   - Modelado de lotes agrícolas (`lote_norte`, `lote_central`, `lote_sur`), cultivos (`vid`, `olivo`, `tabaco`), estado de humedad (`seco`, `optimo`) y sistema de riego (`goteo`, `aspersion`).
   - Reglas deductivas: `requiere_riego_urgente(Lote)` y `lote_goteo_seco(Lote, Especie)`.

---

## 🚀 Instrucciones Paso a Paso

1. Abre `index.html` en tu navegador web.
2. Completa tus datos de identificación (Nombre y Apellido, Matrícula/DNI, Correo UCSE y Comisión).
3. Inicia el cronómetro de **90 minutos** en la barra superior institucional.
4. Resuelve los 5 bloques teóricos (Parte I) y codifica las 2 Bases de Conocimiento Prolog + sus 12 consultas usando el Editor con Linter en vivo y el laboratorio SWISH integrado (Parte II).
5. Al alcanzar el **100% (34 de 34 completados)**, descarga `respuestas_simulacro.json` (que incluye tus respuestas y tus 2 Bases de Conocimiento en `prolog_kb`) y guárdalo en esta carpeta.
6. Ejecuta el autoevaluador oficial en Python 3:
   ```bash
   python autograder_simulacro.py respuestas_simulacro.json
   ```
7. Sube tu entrega al repositorio mediante Git:
   ```bash
   git add respuestas_simulacro.json
   git commit -m "Entrega Simulacro de Examen - [Tu Nombre y Apellido]"
   git push origin main
   ```

