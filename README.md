<div align="center">
<picture>
    <source srcset="https://imgur.com/5bYAzsb.png" media="(prefers-color-scheme: dark)">
    <source srcset="https://imgur.com/Os03JoE.png" media="(prefers-color-scheme: light)">
    <img src="https://imgur.com/Os03JoE.png" alt="Escudo UNAL" width="350px">
</picture>

<h3>Curso de Fundamentos de Robótica Móvil</h3>

<h1>Introducción a la navegación con robots</h1>

<h2>Guía 3 - Navegación basada en comportamientos</h2>

<h5>Pedro F. Cárdenas<br>
    Ricardo Ramírez<br>
    Juan S. Daleman</h5>

<h6>Universidad Nacional de Colombia<br>
    Facultad de Ingeniería<br>
    Departamento de Ingeniería Mecánica y Mecatrónica<br>
    Bogotá, Colombia<br>
    2025</h6>
</div>

<details>
    <summary>🗂️ Tabla de Contenido</summary>

<!-- TOC -->
- [1. 📖 Introducción](#1--introducción)
- [2. 🎯 Objetivos](#2--objetivos)
- [3. 🧰 Herramientas Necesarias](#3--herramientas-necesarias)
  - [3.1. 🔭🛠️ Equipos](#31-️-equipos)
  - [3.2. 🖥️💾 Software](#32-️-software)
- [4. 🔧➡️🚀 Procedimiento](#4-️-procedimiento)
  - [4.1. 🔍📚 Búsqueda bibliográfica](#41--búsqueda-bibliográfica)
  - [4.2. 🏎️↪️🧱 Misión 1: Evite los obstáculos](#42-️️-misión-1-evite-los-obstáculos)
    - [4.2.1. 🎯 Objetivo](#421--objetivo)
    - [4.2.2. 📋 Requerimientos](#422--requerimientos)
    - [4.2.3. 🏎️📍⛳✅ Ejemplo](#423-️-ejemplo)
  - [4.3. 🏎️🔀🏁 Misión 2: Supere el laberinto](#43-️-misión-2-supere-el-laberinto)
    - [4.3.1. 🎯 Objetivo](#431--objetivo)
    - [4.3.2. 📋 Requerimientos](#432--requerimientos)
    - [4.3.3. 🏎️🏁✅🎉 Ejemplo](#433-️-ejemplo)
- [5. 📝📊🗂️ Registro de resultados](#5-️-registro-de-resultados)
- [6. 📑📊🖥️ Presentación de los resultados](#6-️-presentación-de-los-resultados)
- [7. 📚🔗 Recursos](#7--recursos)
- [8. 📚🗄️ Referencias](#8-️-referencias)



</details>

---

<h1> 🗺️🧭🤖 Guía 2: Introducción a la navegación con robots </h1>

## 1. 📖 Introducción

La navegación en robótica móvil se refiere a la capacidad de un robot para desplazarse desde una posición inicial hasta un objetivo, basándose en el conocimiento parcial de su entorno y la información proporcionada por sus sensores. El objetivo es alcanzar el destino de forma eficiente, segura y confiable, adaptándose a las condiciones del entorno.

Existen dos enfoques principales de navegación en robótica móvil, tradicionalmente considerados opuestos, pero que pueden combinarse para mejorar el rendimiento del sistema:

- **Navegación planeada o deliberativa:** Se fundamenta en la inteligencia artificial (IA) simbólica o clásica, y se apoya en la construcción de un modelo interno del entorno. El robot utiliza esta representación para planificar rutas mediante algoritmos, evaluando el mejor camino hacia el objetivo. Este enfoque requiere tiempo de procesamiento y conocimiento previo del entorno o la capacidad de mapearlo.

 - **Navegación reactiva:** Se basa en comportamientos simples que permiten responder directamente a los estímulos de los sensores sin necesidad de un modelo del entorno. Emplea técnicas de IA conexionista o de comportamiento, como control por reglas o redes neuronales, permitiendo al robot reaccionar rápidamente ante obstáculos u otros cambios dinámicos. Este enfoque es especialmente útil en entornos desconocidos o altamente cambiantes.

En la práctica, ambos enfoques se pueden integrar en lo que se conoce como un sistema de navegación híbrido. Este enfoque combina la planificación de alto nivel de la navegación deliberativa con la capacidad de respuesta inmediata de la navegación reactiva. La inteligencia artificial juega un papel clave en esta integración, permitiendo el uso de algoritmos de aprendizaje automático y técnicas adaptativas para mejorar la toma de decisiones en tiempo real. Así, los sistemas híbridos ofrecen una solución más robusta y flexible para enfrentar los desafíos de la navegación autónoma en entornos complejos.


## 2. 🎯 Objetivos

- Identificar las características de los distintos tipos de navegación.

- Reconocer los algoritmos de tipo BUG y los algoritmos de resolución de laberintos.

- Aplicar al menos dos algoritmos basados en comportamientos.

## 3. 🧰 Herramientas Necesarias

### 3.1. 🔭🛠️ Equipos

- Robot Lego EV3.
- Computador. 
- Accesorios del robot Lego EV3.
- Tabla o piso.
- Tablillas y postes para formar obstaculos.

### 3.2. 🖥️💾 Software

- Software que considere adecuado.

## 4. 🔧➡️🚀 Procedimiento 

### 4.1. 🔍📚 Búsqueda bibliográfica

1. Menciona al menos dos características de la navegación planeada y de la navegación basada en comportamientos, y cómo influyen en el tipo de respuesta del robot.

2. Investigaciones destacadas y robots desarrollados por los robotistas Rodney Brooks y Mark Tilden (máximo dos párrafos de cada uno).

3. Mencione al menos tres algoritmos de planificación de rutas para espacios con obstáculos.

4. Describa brevemente los algoritmos Bug 0, Bug 1 y Bug 2.

5. Describa al menos un algoritmo de solución de laberintos (maze algorithm) aplicado en robótica móvil.

>[!IMPORTANT]
>Es necesario crear los espacios de trabajo (laberinto) requeridos y adaptar el robot EV3 de manera adecuada para realizar dos misiones a cumplir. Estas misiones se deben resolver utilizando navegacion basada en comportamientos.


### 4.2. 🏎️↪️🧱 Misión 1: Evite los obstáculos

#### 4.2.1. 🎯 Objetivo

Utilizar uno de los algoritmos Bug para navegar desde la Posición 1 (P1), o punto de partida, hasta la Posición 2 (P2), o meta.

#### 4.2.2. 📋 Requerimientos

- El espacio de trabajo debe contener al menos dos obstáculos que intercepten una línea recta entre la posición 1 y la posición 2.

<div align="center">
  <img src="https://imgur.com/x8dVyz5.jpg" alt="Ejemplo_espacio_trabajo_misión_1" width="600px">
</div>

- El espacio entre los obstáculos debe ser lo suficientemente amplio para que el EV3 pueda pasar sin dificultad.
- La línea que une P1 y P2 debe estar marcada con una cinta o material similar.
- Se debe garantizar que el robot pueda completar el trayecto sin requerir intervención manual durante el proceso.

>[!NOTE]
>Como el algoritmo requiere conocer la pose del robot durante su recorrido, se pueden utilizar odometría visual, odometría por las ruedas o reconocimiento por imágenes. Una alternativa permitida es combinar el algoritmo BUG con un seguidor de línea. La línea puede formar parte de la preparación de la zona de operación del robot.

#### 4.2.3. 🏎️📍⛳✅ Ejemplo

<div align="center">
  <a href="https://www.youtube.com/watch?v=WM9kOitkGEo">
    <img src="https://img.youtube.com/vi/WM9kOitkGEo/0.jpg" alt="Robotic motion planning: bug 2 algorithm" width="400px">
  </a>
</div>

### 4.3. 🏎️🔀🏁 Misión 2: Supere el laberinto

#### 4.3.1. 🎯 Objetivo

Utilizar uno de los algoritmos MAZE para ir desde la entrada P1 hasta la salida P2 del laberinto.

#### 4.3.2. 📋 Requerimientos

- El laberinto debe tener como mínimo unas dimensiones de 6L × 2L, donde L debe estar entre 1,5 y 2,0 veces el largo del EV3.

- El mundo utilizado en el [video](https://www.youtube.com/watch?v=Ro7T3q14uDY) de referencia tiene una forma similar a la presentada. El laberinto debe contar con una entrada y una salida claramente marcadas.

>[!IMPORTANT]
>Cada grupo puede emplear un mundo diferente al mostrado. 

<div align="center">
  <img src="https://imgur.com/75YlgU1.jpg" alt="Ejemplo_espacio_trabajo_misión_2" width="600px">
</div>

- Al cumplir la misión, el algoritmo debe resolver al menos una vez cada una de las situaciones presentadas.

<div align="center">
  <img src="https://imgur.com/WCLTkSl.jpg" alt="Situaciones_a_superar" width="600px">
</div>

- Se debe garantizar que el robot pueda completar el trayecto sin requerir intervención manual durante el proceso.

#### 4.3.3. 🏎️🏁✅🎉 Ejemplo

<div align="center">
  <a href="https://www.youtube.com/watch?v=Ro7T3q14uDY">
    <img src="https://img.youtube.com/vi/Ro7T3q14uDY/0.jpg" alt="Maze Solving Lego EV3 Robot" width="400px">
  </a>
</div>

## 5. 📝📊🗂️ Registro de resultados

Verificar que el EV3 cumpla con cada misión asignada, registrando el resultado de cada una en un video individual. Este video debe ser subido a YouTube y compartido a través del enlace. Además, debe incluir una introducción de la UN, la [introducción del Labsir](https://drive.google.com/file/d/1DlKOyC3ZSt2-_NJSycJGmiu0EZ9OTABb/view?usp=drive_link) y la información de los estudiantes, profesores y curso, tal como se aprecia en el video [Vid Intro Lab Sir.mp4](https://drive.google.com/file/d/1T7b_PQ_8sVyVTFEyEwVkW3QkONyT4-Jt/view?usp=drive_link).

## 6. 📑📊🖥️ Presentación de los resultados

Se debe presentar para cada misión:

  - Una descripción textual de la solución seleccionada.

  - El algoritmo utilizado, descrito en pseudocódigo.

  - Link del video. Se recomienda usar las etiquetas `<a>` y `<img>`.

    ```md
    <a href="https://www.youtube.com/watch?v=<Identificador>">
    <img src="https://img.youtube.com/vi/<Identificador>/0.jpg" alt="<Texto_altenterno>" width="<apropiado_para_la_imagen>">
    </a>
    ```

## 7. 📚🔗 Recursos

<details>
  <summary>🏎️↪️🧱 Misión 1: Evite los obstáculos</summary>

- [Lego Mindstorms ev3: Seguir una línea](https://www.youtube.com/watch?v=EacY_9Ixh68)
- [Lego MINDSTORMS EV3 || Seguidor de líneas proporcional](https://www.youtube.com/watch?v=yo8CHAsn2Pg)
- [Detección de objetos y seguimiento de línea en Open Robert Lab Lego EV3](https://www.youtube.com/watch?v=MPDn0l8AEUA)

</details>


<details>
  <summary>🏎️🔀🏁 Misión 2: Supere el laberinto</summary>

- [funciones en laberinto open roberta](https://www.youtube.com/watch?v=FxrHdQhvIjI)
- [Laberinto con LEGO](https://www.youtube.com/watch?v=EyPH8WHZM74)

</details>

## 8. 📚🗄️ Referencias

**[1]** R. Siegwart, *Introduction to Autonomous Mobile Robots* (2nd ed.), The MIT Press, 2011, pp. 391 y siguientes.

**[2]** Wikipedia, "Behavior-based Robotics," [Online]. Available: [https://en.wikipedia.org/wiki/Behavior-based_robotics](https://en.wikipedia.org/wiki/Behavior-based_robotics). [Accessed: Mar. 30, 2023].

**[3]** Tamie.org, "Behaviour Based Robotics & Deliberative Robotics," [Online]. Available: [https://web.archive.org/web/20100612151345/http://www.tamie.org/bbr.html](https://web.archive.org/web/20100612151345/http://www.tamie.org/bbr.html). [Accessed: Mar. 25, 2023].

**[4]** P. Corke, *Robotics, Vision and Control: Fundamental Algorithms in MATLAB®*, Springer-Verlag Berlin Heidelberg, 2011.

**[5]** K. Wolff, "Autonomous Agents course, Quarters III and IV, spring semester 2008," [Online]. Available: [https://www.am.chalmers.se/~wolff/AA/AutonomousAgents.html](https://www.am.chalmers.se/~wolff/AA/AutonomousAgents.html). [Accessed: Apr. 3, 2023].

**[6]** F. Bullo and S. L. Smith, *Lectures on Robotic Planning and Kinematics Version v0.93 – Jan 1, 2022*, [Online]. Available: [https://ucsb.app.box.com/v/LecturesRobotics](https://ucsb.app.box.com/v/LecturesRobotics).
