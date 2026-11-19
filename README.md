# Diseño de tubos HR

Herramienta web para el diseño de tubos de hormigón armado (HR) enterrados por el **método indirecto (*D-load*)**, según ASTM C76, el manual de la ACPA (2011) y la carga viva HL-93 de AASHTO LRFD.

**Abrir la herramienta:** https://marciagaemilio.github.io/Diseno_Tubos_HR/
<!-- Cambie USUARIO por su nombre de usuario de GitHub después de publicar. -->

## Qué hace

- **Pestaña DISEÑO.** Con los datos del tubo, la instalación y el relleno calcula las cargas (tierra, fluido, peso propio y carga viva con impacto), el *D-load* y la clase mínima de ASTM C76. Si el uso de la clase mínima supera el umbral (95 % por defecto), recomienda la siguiente. Muestra las verificaciones del diseño y genera una memoria técnica que se puede imprimir o guardar en PDF.
- **Tres condiciones de instalación:** zanja, proyección positiva y proyección negativa, con las instalaciones estándar de la ACPA.
- **Plano de igual asentamiento en proyección negativa:** solución exacta, corregida (método 2) o simplificada *H<sub>e</sub> = p′B<sub>d</sub>*.
- **Pestaña ACADÉMICO.** Tres módulos para estudiar el efecto de cada parámetro: carga de tierra, carga viva (distribución piramidal HL-93) y *D-load* y clase de tubo.
- Unidades imperiales o SI y tema claro u oscuro.

## Uso

No requiere instalación. Es un solo archivo HTML, sin dependencias externas: funciona en línea desde el enlace anterior o descargado, al abrirlo con cualquier navegador actual (Chrome, Edge, Firefox o Safari).

## Contenido de la carpeta

| Archivo | Descripción |
|---|---|
| `Diseno_Tubos_HR.html` | La herramienta completa, en un solo archivo. |
| `index.html` | Abre `Diseno_Tubos_HR.html`, para que el enlace de GitHub Pages lleve directo a la herramienta. |
| `Manual_Diseno_Tubos_HR.pdf` | Manual de uso. |
| `fuente/` | Código fuente para modificar la herramienta (ver `fuente/LEEME.txt`). Para regenerarla se necesitan además las webapps originales de carga de tierra y carga viva, que no están en esta carpeta. |
| `LICENSE` | Licencia de uso. |

## Base técnica

- Carga de tierra por la teoría de Marston-Spangler en zanja, proyección positiva y proyección negativa.
- Carga viva HL-93 (camión de diseño y tándem) con la distribución piramidal de la ACPA.
- Factores de encamado para carga de tierra y para carga viva.
- *D-load* comparado con la resistencia a la fisura de 0.01 in de las clases de ASTM C76.

## Autores

- Emilio A. Marciaga-Torres
- Mario R. García-Barragán

Asesor: Dr. Elvis A. Castillo-Camarena, autor también de las aplicaciones de carga de tierra y de carga viva que se incluyen en la pestaña ACADÉMICO.

Desarrollada como parte del trabajo de graduación *Formulación de las especificaciones de diseño y construcción de tubos HR en Panamá*, Licenciatura en Ingeniería Civil, Facultad de Ingeniería Civil, Centro Regional de Veraguas, Universidad Tecnológica de Panamá, 2026.

## Cómo citar

Marciaga-Torres, E. A., y García-Barragán, M. R. (2026). *Diseño de tubos HR* [Aplicación web]. Universidad Tecnológica de Panamá. https://marciagaemilio.github.io/Diseno_Tubos_HR/

## Aviso

Herramienta de apoyo con fines académicos y de diseño. No sustituye el criterio de un ingeniero idóneo ni las normas vigentes: los resultados deben revisarse antes de usarse en un proyecto.

## Licencia

Se distribuye bajo la licencia MIT (archivo `LICENSE`). En resumen, se permite usar, copiar, modificar y distribuir la herramienta, incluso con fines comerciales, siempre que se conserve el aviso de autoría y de licencia. Se entrega "tal cual", sin garantía de ningún tipo.
