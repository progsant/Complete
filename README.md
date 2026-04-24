# Programador de vigilantes

App web para resolver ejercicios de programación de turnos de investigación de operaciones. Pega el enunciado del profesor y la app detecta automáticamente turnos, puestos y ciclo. Luego puedes editar todo manualmente haciendo clic en la tabla.

## Qué hace

Calcula el número mínimo de vigilantes necesarios para cubrir un conjunto de puestos distribuidos en varios turnos al día, respetando un ciclo de trabajo-descanso.

Fórmula:

```
vigilantes mínimos = (puestos_totales × turnos × días_ciclo) ÷ días_trabajo
```

## Características

- Analizador automático de enunciados. Pega el texto del ejercicio y la app detecta número de turnos, duración, ciclo de trabajo-descanso y puestos con su cantidad.
- Editor completamente manual: días de ciclo, número de turnos con horarios, puestos con su cantidad.
- Clic directo en la tabla para mover la "A" de cualquier fila.
- Presets cargados para los ejercicios típicos: vigilantes 2 turnos 3+2, fábrica 3 turnos 4+2.
- Exportación a PNG y modo imprimir.
- Diseño tipo cuaderno de ingeniería, sin dependencias, todo en un solo archivo HTML.

## Cómo usar el analizador

Pega el enunciado en el campo amarillo arriba del sidebar. Ejemplos que funcionan:

- "Trabajan 2 turnos de 12 horas consecutivas y descansan 2 días. Se requiere 1 portero y 2 ronderos."
- "3 turnos de 8 horas, trabajar 4 días y 2 de descanso. Puestos: Torno, Fresa, Corte, Soldadura"
- "2 turnos de 12 horas con ciclo de 3 dias laborando y 2 descansando. 2 bodegueros y 3 cargadores por turno."

Si algo no se detecta, el parser te avisa y usa valores por defecto que puedes ajustar en los paneles.

## Cómo probarla local

Descarga `index.html` y ábrelo con doble clic.

## Cómo publicarla en GitHub Pages

1. Crea un repositorio público en github.com.
2. Sube `index.html` con "Add file > Upload files".
3. Settings → Pages → Source: "Deploy from a branch", branch `main`, carpeta `/ (root)`.
4. Guarda. En 1-2 minutos tendrás la URL pública.

## Tecnología

HTML, CSS y JavaScript vanilla. Sin frameworks, sin build.
