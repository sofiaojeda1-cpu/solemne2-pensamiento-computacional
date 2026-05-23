# solemne2-pensamiento-computacional
Encargo Solemne II

### ● Información del proyecto
* **Nombre del proyecto:** Abanico Paramétrico Reactivo
* **Autor:** Sofia Ojeda Vidal.

### ● Descripción objetiva 
**Qué es el proyecto:** Es un sistema visual generativo, dinámico e interactivo que traduce las acciones del usuario en transformaciones geométricas en tiempo real.
**Qué se ve en pantalla:** Se visualiza una estructura radial centralizada compuesta por múltiples líneas vectoriales, que simulan la forma de un abanico o un engranaje cinético que se expande,
rota y altera su densidad morfológica continuamente.
* **Qué elementos visuales aparecen:** Aparece un fondo oscuro de contraste variable, una rejilla paramétrica de líneas con degradado cromático reactivo (rosado/azul), y circulos pequeños
 en los extremos exteriores de cada linea.
**Qué inputs utiliza:** La posición horizontal del cursor (`mouseX`), si se mueve el mouse a la izquierda se dibujan pocas líneas. si se mueve a la derecha el abanico se llena de líneas, aumentando
  la densidad geométrica. La posición vertical del cursor (`mouseY`), al mover el mouse verticalmente hacia abajo, hace que cada línea de la estructura gire en diferentes velocidades,
  generando un efecto visual de espiral dinámico, y el estado de presión del mouse (`mouseIsPressed`), cuando el usuario hace click en cualquier parte del lienzo, todas las líneas del abanico
  se engrosan instantáneamente, dándole mucho más peso visual y contraste a la composición.
**Qué outputs genera:** Genera un output visual dinámico y reactivo en el lienzo, que consiste en la alteración inmediata de la cantidad de líneas en pantalla, la velocidad/ángulo de su rotación,
  el grosor de los trazos y el tono lumínico del fondo.
 
### ● Descripción conceptual 
**Idea central del proyecto:** La idea central es explorar cómo la interactividad directa puede alterar los parámetros de una estructura geométrica ordenada, transformando un sistema de reglas
matemáticas rígidas en una pieza visual orgánica a través del movimiento.
**Corriente o referente de diseño con el que dialoga:** El proyecto dialoga directamente con el **Diseño Paramétrico** y el **Arte Cinético**.
No busca imitar una ilustración estática, sino codificar algoritmos basados en variables alterables para crear variaciones infinitas.
**Descripción de referentes visuales, teóricos o históricos:**
    * *John Maeda (Diseño y Computación):* Teórico y diseñador clave que postula el uso del código como un medio de expresión artística y matemática flexible.
    * *Casey Reas y Ben Fry (Creadores de Processing):* Sus exploraciones de sistemas vivos basados en reglas computacionales y geometrías iterativas sirven de base para esta estructura abstracta.
    * *Escultura Cinética:* Referente histórico en la búsqueda de incorporar el movimiento real o percibido como un componente estético fundamental de la obra de arte.
**Principio de diseño explorado:** Se explora el principio de **Variación y Repetición mediante Reglas Algorítmicas**. 
El diseño se organiza mediante un bucle iterativo donde la simetría y el ritmo visual cambian no por azar, sino bajo parámetros lógicos bien definidos.


### ● Input / Output y sistema
La cantidad de subdivisiones del sistema está directamente ligada a la coordenada horizontal del mouse. El ángulo de torsión de la estructura 
depende del movimiento vertical del cursor. El grosor de las líneas del abanico está condicionado al estado del click del usuario.El sistema reacciona de manera continua sin interrupciones lineales. 
El usuario no es solo un espectador, sino lo que hace que se modifiquen los parámetros que dan forma final a la composición geométrica.
**Qué datos entran, cómo se procesan y transforman:** * Entrada de datos numéricos flotantes desde `mouseX` y `mouseY`. Estos datos entran a la función propia `dibujarSistemaParametrico()` y se procesan
matemáticamente usando la función `map()`, la cual normaliza el rango de la pantalla y lo traduce a propiedades de cantidad (de 10 a 100 líneas) y color.
Este codigo roduce una animación interactiva fluida donde el abanico se abre o se cierra compactando sus líneas, gira sobre su propio eje central y cambia el grosor de sus lineas en tiempo real.

### ● Diagrama de flujo
<img width="740" height="2876" alt="diagrama_de_flujo" src="https://github.com/user-attachments/assets/362eb455-4b29-4dd0-bdfe-bc8e3f0f5993" />


### ● Imágenes
fotos de refernte)
<img width="815" height="658" alt="Captura de pantalla 2026-05-22 185209" src="https://github.com/user-attachments/assets/531e1eb6-f238-4ede-bcc7-89d232d188f2" />
<img width="1022" height="648" alt="Captura de pantalla 2026-05-22 185318" src="https://github.com/user-attachments/assets/e0e23929-aaa3-4cf8-8a46-bb8ffef89650" />
<img width="821" height="570" alt="Captura de pantalla 2026-05-22 185235" src="https://github.com/user-attachments/assets/c4c219ee-cbe9-4857-b173-e8b989c5240d" />



#### Capturas del Proceso:
1. *Estado Inicial (Mouse a la izquierda - Pocas líneas geométricas).*
2. *Estado de Alta Densidad (Mouse a la derecha - Multiplicación de la forma).*
3. *Interacción de Click (Aumento en el grosor estructural del abanico).*

**Link al Sketch editable en p5.js:** https://editor.p5js.org/sofia.ojeda1/sketches/s0lFNMj4y
**Link al Sketch para visualizar en p5.js:** https://editor.p5js.org/sofia.ojeda1/full/s0lFNMj4y

