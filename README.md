# HDC_Investigation

**Hyperdimensional Computing (HDC) aplicado a la predicción de propiedades moleculares.**

Repositorio de investigación en curso sobre el uso de computación hiperdimensional para clasificación molecular, con foco en la **fusión de representaciones estructurales y fisicoquímicas** mediante combinación ponderada de hipervectores.

---

## Motivación

La computación hiperdimensional representa la información en vectores de muy alta dimensión (típicamente ≥10.000), donde las operaciones de *binding*, *bundling* y *permutación* permiten codificar y razonar sobre datos de forma robusta al ruido, eficiente en cómputo y con buena capacidad de aprendizaje incremental.

Estas propiedades la hacen atractiva como alternativa liviana a las redes profundas para tareas de **predicción de propiedades moleculares**, donde el costo de entrenamiento y la interpretabilidad son factores relevantes. La pregunta central de esta investigación es cómo **integrar distintos tipos de información molecular** —estructural y fisicoquímica— dentro de un mismo espacio hiperdimensional sin degradar la señal.

---

## Enfoque

El trabajo gira en torno a la clasificación sobre el dataset **BBBP** (Blood–Brain Barrier Penetration), prediciendo la permeabilidad de la barrera hematoencefálica a partir de la estructura molecular.

Las líneas principales son:

- **Representación dual.** Codificación estructural vía fingerprints **ECFP** combinada con descriptores **fisicoquímicos**, mapeando ambas fuentes a hipervectores.
- **Fusión ponderada de hipervectores.** En lugar de un *bundling* uniforme, se asignan pesos a cada representación para controlar su contribución relativa al hipervector de clase.
- **Aprendizaje adaptativo.** Ajuste de los pesos de combinación durante el entrenamiento, buscando que el modelo aprenda el balance óptimo entre información estructural y fisicoquímica.
- **Saturación de signo en el bundling ponderado.** Análisis del fenómeno por el cual el *bundling* con pesos satura el signo de las componentes y limita el aporte real de cada fuente, junto con estrategias para mitigarlo.

---

## Marco de referencia

La investigación dialoga con literatura reciente de HDC y de aprendizaje de representaciones moleculares, entre otras:

- **OnlineHD** — entrenamiento adaptativo e incremental de modelos HDC.
- **BiHDTrans** — incorporación de mecanismos de atención / Transformer al paradigma hiperdimensional.
- **MolCLR** — aprendizaje contrastivo de representaciones moleculares como punto de comparación con enfoques basados en grafos.

La carpeta `papers/` reúne la bibliografía de base y `docs/` la documentación y notas de la investigación.

---

## Estado

Proyecto en desarrollo activo. Los experimentos viven en `notebooks/` y se irán incorporando resultados, métricas y documentación de reproducibilidad a medida que avance la investigación.

---

## Autoría

Investigación desarrollada por la estudiante Alexia Aurrecochea. 
En el marco del curso de Introducción a la Investigación Intermedio (Sem1/2026) de Computación Hiperdimensional, a cargo del docente Dr. Gustavo Vazquéz.

Universidad Católica del Uruguay Dámaso Antonio Larrañaga.

<img width="432" height="155" alt="image" src="https://github.com/user-attachments/assets/8fe04c25-f403-4ead-998b-51b1023fe351" />

