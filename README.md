<a id="top"></a>

<div align="center">
  <img src="assets/icons/logisim.png" width="64" alt="Logisim">
  <img src="assets/icons/ASM.png" width="64" alt="Assembly">
  <img src="assets/icons/cpu.png" width="64" alt="CPU" >
  <h1>Arquitectura de Computadoras</h1>
  <p><em>Diseño de microprocesadores S-MIPS en Logisim · Programación en ensamblador</em></p>
</div>

<p align="center">
  <a href="http://www.cburch.com/logisim/" target="_blank">
    <img src="https://img.shields.io/badge/made%20with-logisim-FF6B6B.svg" alt="Hecho con Logisim">
  </a>
  <a href="https://opensource.org/licenses/MIT" target="_blank">
    <img src="https://img.shields.io/badge/license-MIT-green.svg" alt="Licencia">
  </a>
  <a href="https://github.com/matcom" target="_blank">
    <img src="https://img.shields.io/badge/curso-2026--2027-blue.svg" alt="Curso 2026-2027">
  </a>
</p>

<div align="center">
  <a href="#acerca">Acerca del Repositorio</a>
  <span>&nbsp;✦&nbsp;</span>
  <a href="#notaciones">Notaciones</a>
  <span>&nbsp;✦&nbsp;</span>
  <a href="#tecnologias">Tecnologías</a>
  <span>&nbsp;✦&nbsp;</span>
  <a href="#empezar">Cómo Empezar</a>
  <span>&nbsp;✦&nbsp;</span>
  <a href="#documentacion">Documentación</a>
  <span>&nbsp;✦&nbsp;</span>
  <a href="#contribuciones">Contribuciones</a>
  <span>&nbsp;✦&nbsp;</span>
  <a href="#licencia">Licencia</a>
  <span>&nbsp;✦&nbsp;</span>
  <a href="#soporte">Soporte</a>
</div>

<br>

<a id="acerca"></a>

## 📜 Acerca del Repositorio
Hola, soy **José Rafael** 👋.

Este repositorio contiene todas las **conferencias, clases prácticas, soluciones y el proyecto final** de la asignatura **Arquitectura de Computadoras** (curso 2026–2027) en la Facultad de Matemática y Computación ([MATCOM](https://github.com/matcom)) de la Universidad de La Habana.

> [!TIP]
> Si eres estudiante de la misma asignatura, siéntete libre de explorar, aprender y contribuir.

<p align="right">(<a href="#top">Volver al inicio 🔝</a>)</p>

<a id="notaciones"></a>

## 📐 Notaciones

En las soluciones uso la siguiente notación para representar las operaciones lógicas:

| Símbolo | Notación | Operación | Descripción |
| :---: | :---: | :--- | :--- |
| <img src="assets/icons/simbolos/NOT.svg" width="24"  alt="NOT"> | `¬` | NOT | Negación |
| <img src="assets/icons/simbolos/AND.svg" width="24"  alt="AND"> | `∧` | AND | Conjunción |
| <img src="assets/icons/simbolos/OR.svg" width="24"  alt="OR"> | `∨` | OR | Disyunción |
| <img src="assets/icons/simbolos/XOR.svg" width="24"  alt="XOR"> | `⊕` | XOR | Disyunción exclusiva |

<p align="right">(<a href="#top">Volver al inicio 🔝</a>)</p>

<a id="tecnologias"></a>

## 🧰 Tecnologías

- [**Logisim 2.7.1**](http://www.cburch.com/logisim/) – Simulador de circuitos digitales (versión usada en clase).
- [**Markdown**](https://www.markdownguide.org/) – Para la documentación de los ejercicios.
- [**Git**](https://git-scm.com/) – Control de versiones y colaboración.

<p align="right">(<a href="#top">Volver al inicio 🔝</a>)</p>

<a id="empezar"></a>

## 🚀 Cómo Empezar

### Requisitos

- **Logisim 2.7.1** (o superior).

### Clonar el repositorio

```bash
git clone https://github.com/joserafael0160/Arquitectura-Computadoras.git
cd Arquitectura-Computadoras
```

### Abrir un ejercicio

1. Abre **Logisim 2.7.1**.
2. Navega a la carpeta `CPs/Soluciones/CP1/1-Primeros-Pasos-Logisim/`.
3. Abre el archivo `circuito.circ`.
4. Prueba el circuito usando la herramienta **"Mano"** (Pin).

### Revisar la documentación

Cada ejercicio tiene su documentación en `solucion.md` dentro de su propia carpeta. Allí encontrarás la explicación teórica, ecuaciones y tablas de verdad.

<p align="right">(<a href="#top">Volver al inicio 🔝</a>)</p>

<a id="documentacion"></a>

## 📖 Documentación

Dentro de cada carpeta de solución encontrarás:

- **`solucion.md`** – Archivo Markdown con la solución detallada, ecuaciones, tablas de verdad y pasos de diseño.
- **`circuito.circ`** – Archivo de Logisim con la implementación.

Luego, en `Conferencias/` verás todas las conferencias impartidas por el profesor.

Además, en `Bibliografía/` tienes los libros de referencia recomendados por el profesor:

- **Harris & Harris** – *Digital Design and Computer Architecture*.
- **Patterson & Hennessy** – *Computer Organization and Design*.
- **Carter** – *PC Assembly Language*.

<p align="right">(<a href="#top">Volver al inicio 🔝</a>)</p>

<a id="contribuciones"></a>

## 🤝 Contribuciones

Las contribuciones son bienvenidas. Si encuentras un error o quieres mejorar alguna solución, sigue estos pasos:

1. Haz un [_fork_](https://github.com/joserafael0160/Arquitectura-Computadoras/fork) del proyecto.
2. Clona tu fork (`git clone <URL del fork>`).
3. Añade el repositorio original como remoto (`git remote add upstream <URL del original>`).
4. Crea una rama para tu mejora (`git switch -c feature/mejora-ejercicio`).
5. Realiza tus cambios y haz commit (`git commit -m 'Mejora: descripción'`).
6. Push a tu rama (`git push origin feature/mejora-ejercicio`).
7. Abre un [_pull request_](https://github.com/joserafael0160/Arquitectura-Computadoras/pulls).

<p align="right">(<a href="#top">Volver al inicio 🔝</a>)</p>

<a id="licencia"></a>

## 🔑 Licencia

Este proyecto está bajo la licencia MIT. Consulta el archivo [LICENSE](LICENSE) para más detalles.

<p align="right">(<a href="#top">Volver al inicio 🔝</a>)</p>

<a id="soporte"></a>

## 🙏 Soporte
¿Preguntas, sugerencias o dudas? Abre un issue en el repositorio.

Si te resulta útil, no olvides dejar una estrella ⭐️: [**Dar estrella**](https://github.com/joserafael0160/Arquitectura-Computadoras)

<p align="right">(<a href="#top">Volver al inicio 🔝</a>)</p>
<br>
<hr>

<p align="center">
  ⚙️ <strong>De la lógica al procesador</strong> ⚙️
</p>

<p align="center">
  <sub>
    Un proyecto creado con ❤️ por <a href="https://github.com/joserafael0160">@joserafael0160</a>
  </sub>
</p>