# Diseño de tubos HR

[![Licencia: MIT](https://img.shields.io/badge/Licencia-MIT-yellow.svg)](https://opensource.org/license/mit)

**Autores / Authors:** Emilio A. Marciaga-Torres, Mario R. García-Barragán\
**Asesor / Advisor:** Dr. Elvis A. Castillo-Camarena\
Universidad Tecnológica de Panamá (UTP) — Facultad de Ingeniería Civil, Centro Regional de Veraguas

**Aplicación en línea / Live app:** https://marciagaemilio.github.io/Diseno_Tubos_HR/

[Español](#español) · [English](#english)

---

## Español

### Qué es

**Diseño de tubos HR** es una herramienta web para el diseño de tubos de hormigón armado (HR)
enterrados por el **método indirecto (*D-load*)**, según ASTM C76, el manual de la ACPA (2011)
y la carga viva HL-93 de AASHTO LRFD.

Diseñar un tubo enterrado exige combinar varias piezas: la carga de tierra de Marston-Spangler
para la condición de instalación, la carga viva vehicular distribuida a través del relleno, el
peso del fluido y el peso propio, los factores de encamado y, al final, la comparación del
*D-load* con la resistencia de las clases de ASTM C76. La herramienta reúne todo ese cálculo,
lo actualiza al instante cuando cambia un dato y lo documenta en una memoria técnica.

Es útil para **diseño de proyectos**, **docencia** y **revisión de métodos**.

> La herramienta es un apoyo al diseño y no sustituye el criterio de un ingeniero idóneo ni las
> normas vigentes (ver [Aviso de responsabilidad](#aviso-de-responsabilidad)).

### Funciones principales

- **Pestaña DISEÑO:** con los datos del tubo, la instalación y el relleno calcula las cargas
  (tierra, fluido, peso propio y carga viva con impacto), el *D-load* y la clase mínima de
  ASTM C76. Si el uso de la clase mínima supera el umbral (95 % por defecto), recomienda la
  siguiente.
- **Tres condiciones de instalación:** zanja, proyección positiva y proyección negativa, con las
  instalaciones estándar de la ACPA (tipos 1 a 4).
- **Plano de igual asentamiento en proyección negativa:** solución exacta, corregida (método
  analítico) o simplificada *H<sub>e</sub> = p′B<sub>d</sub>*, propuesta en este trabajo, con la
  comparación de los tres métodos.
- **Verificaciones y esquema:** comprobaciones del diseño y esquema de la instalación.
- **Memoria técnica:** documento con datos, cálculos, clase recomendada, verificaciones y
  referencias, que se puede imprimir o guardar en PDF.
- **Pestaña ACADÉMICO:** tres módulos para estudiar el efecto de cada parámetro: carga de tierra,
  carga viva (distribución piramidal HL-93) y *D-load* y clase de tubo.
- Unidades imperiales o SI y tema claro u oscuro.

### Cómo usarla

1. Abre la herramienta en cualquier navegador actual (Chrome, Edge, Firefox o Safari).
2. En **DISEÑO**, define el tubo (diámetro interior y pared) y la instalación: zanja,
   proyección negativa o positiva, instalación estándar ACPA y suelo de relleno.
3. Ajusta las cargas: altura de relleno sobre la corona *H*, peso unitario del suelo, carga
   viva HL-93, peso del fluido y peso propio (en **Opciones avanzadas**: impacto, orientación
   del camión, pesos unitarios y umbral).
4. Revisa la clase recomendada y las verificaciones, y genera la memoria con **Ver memoria** o
   **Imprimir / PDF**.

**Privacidad:** todo el cálculo se hace dentro del navegador; ningún dato se envía a un
servidor.

### Uso local

Descarga `Diseno_Tubos_HR.html` y ábrelo con doble clic; no requiere instalación, servidor ni
conexión a internet, porque no carga librerías externas.

### Contenido del repositorio

| Archivo | Descripción |
|---|---|
| `index.html` | Página de inicio (bilingüe ES/EN) que presenta la herramienta y enlaza a ella |
| `Diseno_Tubos_HR.html` | La herramienta completa, en un solo archivo autocontenido |
| `Manual_Diseno_Tubos_HR.pdf` | Manual de uso |
| `fuente/` | Código fuente para modificar la herramienta (ver `fuente/LEEME.txt`). Para regenerarla se necesitan además las webapps originales de carga de tierra y carga viva, que no están en esta carpeta |
| `README.md` | Este archivo |
| `LICENSE` | Términos de la licencia (MIT) |

### Publicación en GitHub Pages

1. Sube estos archivos a la raíz de la rama `main` del repositorio.
2. En el repositorio, ve a **Settings → Pages**.
3. En **Build and deployment**, elige **Deploy from a branch**, selecciona `main` y
   `/ (root)`, y guarda.
4. Al cabo de un minuto el sitio estará disponible en
   https://marciagaemilio.github.io/Diseno_Tubos_HR/

### Base técnica

- Carga de tierra por la teoría de Marston-Spangler en zanja, proyección positiva y proyección
  negativa.
- Carga viva HL-93 (camión y tándem de diseño) con la distribución piramidal de la ACPA.
- Factores de encamado para carga de tierra y para carga viva.
- *D-load* comparado con la resistencia a la fisura de 0,01 in de las clases de ASTM C76.

### Licencia y atribución

© 2026 Emilio A. Marciaga-Torres, Mario R. García-Barragán y Elvis A. Castillo-Camarena.

Esta herramienta se distribuye bajo la [licencia MIT](https://opensource.org/license/mit).
Puedes **usarla, copiarla, modificarla y distribuirla**, incluso con fines comerciales,
**siempre que conserves el aviso de derechos de autor y de licencia**. Consulta el archivo
[`LICENSE`](LICENSE) para más detalles.

Texto de crédito sugerido:

> Diseño de tubos HR — Emilio A. Marciaga-Torres y Mario R. García-Barragán (asesor:
> Dr. Elvis A. Castillo-Camarena), Universidad Tecnológica de Panamá (UTP). Licencia MIT.

La pestaña ACADÉMICO incluye las aplicaciones de carga de tierra y de carga viva del
Dr. Elvis A. Castillo-Camarena.

Desarrollada como parte del trabajo de graduación *Formulación de las especificaciones de
diseño y construcción de tubos HR en Panamá*, Licenciatura en Ingeniería Civil, Facultad de
Ingeniería Civil, Centro Regional de Veraguas, Universidad Tecnológica de Panamá, 2026.

### Aviso de responsabilidad

Diseño de tubos HR es una herramienta de apoyo desarrollada con fines académicos como parte de
un trabajo de graduación de la Universidad Tecnológica de Panamá. Sus resultados dependen de los
datos ingresados y de las hipótesis de los métodos empleados; no sustituyen el criterio de un
ingeniero idóneo ni las normas vigentes, y deben ser revisados por el profesional responsable
del diseño antes de usarse en un proyecto. **Ni los autores, ni su asesor, ni la Universidad
Tecnológica de Panamá (UTP) asumen responsabilidad alguna** por el uso que se haga de la
herramienta o de sus resultados, ni por los daños o perjuicios que de ello puedan derivarse. La
herramienta se entrega "tal cual", sin garantía de ningún tipo.

### Cómo citarla

Si usas la herramienta en un curso, tesis, informe o publicación, por favor cítala así:

> Marciaga-Torres, E. A., y García-Barragán, M. R. (2026). *Diseño de tubos HR* [Aplicación
> web]. Universidad Tecnológica de Panamá. https://marciagaemilio.github.io/Diseno_Tubos_HR/

```bibtex
@misc{marciagatorres2026tuboshr,
  author       = {Marciaga-Torres, Emilio A. and Garc{\'\i}a-Barrag{\'a}n, Mario R.},
  title        = {{Dise{\~n}o de tubos HR}},
  year         = {2026},
  howpublished = {Aplicaci{\'o}n web, Universidad Tecnol{\'o}gica de Panam{\'a}},
  url          = {https://marciagaemilio.github.io/Diseno_Tubos_HR/}
}
```

---

## English

### What it is

**Diseño de tubos HR** (*HR pipe design*) is a web application for the design of buried
reinforced concrete (HR) pipe by the **indirect design method (*D-load*)**, following ASTM C76,
the ACPA Concrete Pipe Design Manual (2011) and the AASHTO LRFD HL-93 live load.

Designing a buried pipe means combining several pieces: the Marston-Spangler earth load for
the installation condition, the vehicle live load distributed through the fill, the fluid and
pipe weights, the bedding factors and, finally, the comparison of the *D-load* with the
strength of the ASTM C76 classes. The application brings all of that together, updates it
instantly whenever an input changes, and documents it in a technical report.

It is useful for **project design**, **teaching** and **method review**.

> The application supports design work; it does not replace the judgment of a qualified
> engineer or the applicable codes (see [Disclaimer](#disclaimer)).

### Main features

- **DISEÑO tab (design):** from the pipe, installation and fill data it computes the loads
  (earth, fluid, pipe weight and live load with impact), the *D-load* and the minimum ASTM C76
  class. When the minimum class is used above a threshold (95 % by default), it recommends the
  next one.
- **Three installation conditions:** trench, positive projection and negative projection, with
  the ACPA standard installations (types 1 to 4).
- **Plane of equal settlement in negative projection:** exact solution, corrected (analytical
  method) or the simplified *H<sub>e</sub> = p′B<sub>d</sub>* proposed in this work, with a
  comparison of the three methods.
- **Checks and sketch:** design checks and a sketch of the installation.
- **Technical report:** a document with inputs, calculations, recommended class, checks and
  references, ready to print or save as PDF.
- **ACADÉMICO tab (teaching):** three modules to study the effect of each parameter: earth load,
  live load (HL-93 pyramid distribution) and *D-load* and pipe class.
- Imperial or SI units and light or dark theme.

### How to use

1. Open the application in any current browser (Chrome, Edge, Firefox or Safari).
2. In **DISEÑO**, define the pipe (inside diameter and wall) and the installation: trench,
   negative or positive projection, ACPA standard installation and fill soil.
3. Set the loads: fill height over the crown *H*, soil unit weight, HL-93 live load, fluid
   weight and pipe weight (under **Opciones avanzadas**: impact, truck orientation, unit
   weights and threshold).
4. Review the recommended class and the checks, and produce the report with **Ver memoria** or
   **Imprimir / PDF**.

**Privacy:** all calculations run inside your browser; no data is sent to any server.

### Running locally

Download `Diseno_Tubos_HR.html` and open it with a double-click; no installation, server or
internet connection is needed, since it loads no external libraries.

### Repository contents

| File | Description |
|---|---|
| `index.html` | Home page (bilingual ES/EN) that presents the application and links to it |
| `Diseno_Tubos_HR.html` | The complete application, in a single self-contained file |
| `Manual_Diseno_Tubos_HR.pdf` | User manual (Spanish) |
| `fuente/` | Source code to modify the application (see `fuente/LEEME.txt`). Rebuilding it also requires the original earth-load and live-load web apps, which are not in this folder |
| `README.md` | This file |
| `LICENSE` | License terms (MIT) |

### Publishing on GitHub Pages

1. Push these files to the root of the repository's `main` branch.
2. In the repository, go to **Settings → Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**, select `main` and
   `/ (root)`, and save.
4. After a minute the site is available at https://marciagaemilio.github.io/Diseno_Tubos_HR/

### Technical basis

- Earth load by the Marston-Spangler theory for trench, positive projection and negative
  projection.
- HL-93 live load (design truck and tandem) with the ACPA pyramid distribution.
- Bedding factors for earth load and for live load.
- *D-load* compared with the 0.01 in crack strength of the ASTM C76 classes.

### License and attribution

© 2026 Emilio A. Marciaga-Torres, Mario R. García-Barragán and Elvis A. Castillo-Camarena.

This application is released under the [MIT License](https://opensource.org/license/mit).
You are free to **use, copy, modify and distribute** it, including commercially, **provided
you keep the copyright and license notice**. See [`LICENSE`](LICENSE) for details.

Suggested credit line:

> Diseño de tubos HR — Emilio A. Marciaga-Torres and Mario R. García-Barragán (advisor:
> Dr. Elvis A. Castillo-Camarena), Universidad Tecnológica de Panamá (UTP). Licensed under the
> MIT License.

The ACADÉMICO tab includes the earth-load and live-load web applications by
Dr. Elvis A. Castillo-Camarena.

Developed as part of the undergraduate thesis *Formulación de las especificaciones de diseño y
construcción de tubos HR en Panamá*, Bachelor of Civil Engineering, School of Civil
Engineering, Veraguas Regional Center, Universidad Tecnológica de Panamá, 2026.

### Disclaimer

Diseño de tubos HR is a support tool developed for academic purposes as part of an
undergraduate thesis at the Universidad Tecnológica de Panamá. Its results depend on the data
entered and on the assumptions of the methods it implements; they do not replace the judgment
of a qualified engineer or the applicable codes, and they must be reviewed by the professional
responsible for the design before being used in a project. **Neither the authors, their
advisor, nor the Universidad Tecnológica de Panamá (UTP) accept any responsibility or
liability** for the use of the application or of its results, or for any damage or loss arising
from such use. The application is provided "as is", without warranty of any kind.

### How to cite

If you use the application in a course, thesis, report or publication, please cite it as:

> Marciaga-Torres, E. A., & García-Barragán, M. R. (2026). *Diseño de tubos HR* [Web
> application]. Universidad Tecnológica de Panamá. https://marciagaemilio.github.io/Diseno_Tubos_HR/

```bibtex
@misc{marciagatorres2026tuboshr,
  author       = {Marciaga-Torres, Emilio A. and Garc{\'\i}a-Barrag{\'a}n, Mario R.},
  title        = {{Dise{\~n}o de tubos HR}},
  year         = {2026},
  howpublished = {Web application, Universidad Tecnol{\'o}gica de Panam{\'a}},
  url          = {https://marciagaemilio.github.io/Diseno_Tubos_HR/}
}
```
