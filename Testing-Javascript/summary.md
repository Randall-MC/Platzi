# Fundamentos de Testing en JavaScript

## Fases en el desarrollo de software

1. Diseño
2. Desarrollo
3. Pruebas
4. Producción

> "The earlier you find a mistake, the easier it is to fix"

---

## Fases de gestión de riesgo

### Statics Analysis

Runs in your editor. Finds typos, incorrect function calls, autocomplete code.

Análisis de código estático, demora muy poco y casi que es en tiempo real a medida que se escribe el código muestra feedback de en dónde se incurre en un (posible) error.

### Unit tests

Take a few seconds to verify your code does what you think it does.

Requiere de más tiempo, se asegura de que los pedazos de código que se escriben funcionen como se espera. Se pone a prueba el código con diferentes escenarios.

### Integration test

Take a few minutes to validate your system works. May catch fun edge cases.

Pruebas de integración, conjunto de pruebas unitarias, puede que funcionen viene por si solas pero la integrarse no.

### Code review

Take a few hours to validate you're following standard norms and practices of your team.

### QA

Take a few hours or days to ensure everything works together as expected.

Personas (testers) realizan pruebas automáticas o manuales, de funcionalidad (seguridad, estrés)

---

## Pirámide del Testing

![Testing pyramid](/Testing-Javascript/testing-pyramid.png)

| **Type of Test** | **Something** |
| --- | --- |
| Unit | These are the base, they are faster and cheaper. So there is more. |
| Service | Integration testing, component test, API testing |
| UI | They are more expensive, slow and there are less |

## Ice-cream Cone

![Ice-cream testing](/Testing-Javascript/ice-cream-cone.png)

## Trophy

![Trophy](/Testing-Javascript/trophy.png)

> It is recommended specially for JavaScript

## Deuda técnica

Una deuda no es mala ni buena, en realidad, puede ser una ayuda técnica. Si se utiliza de forma correcta puede ayudarnos a lograr algo que sin ella sería imposible sin olvidar que se debe pagar.

![Four stages of company growth](/Testing-Javascript/stages-company-growth.png)

![Classifying tech dept](/Testing-Javascript/classifying-tech-dept.png)

![Tech dept portfolio](/Testing-Javascript/tech-dept-portfolio.png)

---

## Recomendaciones

- Libro [Software Engineer at Google](https://www.amazon.com.mx/Software-Engineering-Google-Lessons-Programming/dp/1492082791/ref=asc_df_1492082791/?tag=gledskshopmx-20&linkCode=df0&hvadid=451124037587&hvpos=&hvnetw=g&hvrand=8446275770574180263&hvpone=&hvptwo=&hvqmt=&hvdev=c&hvdvcmdl=&hvlocint=&hvlocphy=1010043&hvtargid=pla-893850003581&psc=1)
