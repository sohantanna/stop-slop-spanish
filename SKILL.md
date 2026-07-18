---
name: basta-de-relleno
description: Elimina los rasgos de escritura de IA en textos en español. Úsala al redactar, editar o revisar prosa para quitar las marcas predecibles de la IA, con cobertura de todas las variedades del español.
metadata:
  trigger: Redactar prosa, editar borradores o revisar contenido en busca de patrones de IA en cualquier variedad del español
  author: Adaptación al español de "Stop Slop" de Hardik Pandya (https://hvpandya.com)
  original: https://github.com/hardikpandya/stop-slop
---

# Basta de Relleno

Elimina los patrones predecibles de la escritura de IA en textos en español.

Los rasgos de IA en español no son los mismos que en inglés. Esta guía persigue los propios del español: el carraspeo de "Cabe destacar que", los adjetivos-comodín ("crucial", "robusto", "vibrante"), la estructura "no solo… sino también", la pasiva refleja que esconde al agente ("se tomó la decisión") y el montón de adverbios en *-mente*. Además vigila un problema que el inglés no tiene: mezclar variedades del español (vos con tú, ustedes con vosotros, coche con carro) o caer en un "neutro" sin sabor.

## Reglas principales

1. **Corta el relleno.** Quita las aperturas de carraspeo ("Cabe destacar que", "En el mundo actual", "Hoy en día"), las muletillas de énfasis ("Y punto", "Así de simple") y los adverbios en *-mente* vacíos. Ver [references/frases.md](references/frases.md).

2. **Rompe las estructuras de fórmula.** Evita los contrastes binarios ("No es X, es Y"), el "no solo… sino también", las enumeraciones por negación, la fragmentación dramática, los montajes retóricos ("¿Y si te dijera que…?") y la falsa agencia. Ver [references/estructuras.md](references/estructuras.md).

3. **Usa voz activa.** Cada oración necesita un sujeto humano que hace algo. Nada de pasiva perifrástica ("fue creado") ni de pasiva refleja que oculta al agente ("se decidió", "se puede observar que"). Nada de objetos inanimados con verbos humanos ("los datos nos dicen", "la queja se convierte en mejora").

4. **Sé concreto/a.** Nada de declaraciones vagas ("Las razones son estructurales"). Nombra la cosa. Nada de extremos perezosos ("todo", "siempre", "nunca") haciendo trabajo vago. Nada de adjetivos-comodín de IA ("clave", "fundamental", "robusto", "vibrante", "invaluable").

5. **Mete a quien lee en la escena.** Nada de voz de narrador a distancia ("Nadie diseñó esto"). "Tú"/"vos"/"usted" gana a "la gente". Lo concreto gana a lo abstracto.

6. **Varía el ritmo.** Mezcla longitudes de oración. Dos elementos ganan a tres (cuidado con la regla de tres). Nada de rayas (—) para pausas dramáticas. Cuidado con la muletilla del gerundio de consecuencia ("logrando así", "permitiendo").

7. **Confía en quien lee.** Di los hechos directo. Sáltate el suavizado, la justificación y el tutelaje. No encadenes conectores de relleno ("Además… Asimismo… Por otro lado… En este sentido…").

8. **Corta las frases de calendario.** Si suena a cita motivacional o a titular de LinkedIn, reescríbelo.

9. **Elige UNA variedad y mantenla.** No mezcles voseo con tuteo, vosotros con ustedes, ni vocabulario de regiones distintas. Evita términos vulgares en la región destino. El "español neutro" sin dueño también es un rasgo de IA. Ver [references/variaciones-regionales.md](references/variaciones-regionales.md).

## Comprobaciones rápidas

Antes de entregar un texto:

- ¿Adverbios en *-mente* vacíos ("realmente", "simplemente", "profundamente")? Elimínalos.
- ¿Voz pasiva o pasiva refleja ("se decidió", "fue creado", "se puede observar que")? Encuentra al agente y ponlo de sujeto.
- ¿Cosa inanimada con verbo humano ("la decisión surge", "el mercado premia")? Nombra a la persona.
- ¿Arranque de carraspeo ("Cabe destacar que", "Es importante mencionar que", "En la era digital")? Ve al grano.
- ¿Contraste "No es X, sino Y" / "No se trata de X, sino de Y"? Afirma Y directo.
- ¿"No solo… sino también"? Reescríbelo.
- ¿Tres oraciones seguidas con la misma longitud? Rompe una.
- ¿Pregunta retórica de arranque ("¿Alguna vez te has preguntado…?", "¿Qué pasaría si…?")? Córtala.
- ¿Raya (—) para dramatizar? Quítala. Usa comas o puntos.
- ¿Adjetivo-comodín ("crucial", "fundamental", "clave", "robusto", "vibrante") sin nombrar lo concreto? Nombra lo concreto.
- ¿Cierre de fórmula ("En resumen", "En conclusión", "En definitiva")? Que el texto cierre solo.
- ¿Calco del inglés ("hacer sentido", "aplicar para", "en base a", "remover", "jugar un papel", "impactar algo")? Corrígelo.
- ¿Gerundio de consecuencia ("logrando así", "permitiendo que")? Reescribe en oraciones separadas.
- ¿Mezclas de variedad (vos con tú, ustedes con vosotros, "coche" con "carro")? Unifica a una sola.

## Puntuación

Puntúa de 1 a 10 cada dimensión:

| Dimensión | Pregunta |
|-----------|----------|
| Franqueza | ¿Afirmaciones o anuncios? |
| Ritmo | ¿Variado o metronómico? |
| Confianza | ¿Respeta la inteligencia de quien lee? |
| Autenticidad | ¿Suena humano? |
| Densidad | ¿Sobra algo cortable? |
| Coherencia regional | ¿Una sola variedad, sin mezclas ni "neutro" sin sabor? |

Menos de 42/60: revisa.

## Ejemplos

Ver [references/ejemplos.md](references/ejemplos.md) para transformaciones de antes/después, incluida la corrección de mezclas regionales.

## Licencia

MIT. Adaptación al español de [Stop Slop](https://github.com/hardikpandya/stop-slop) de Hardik Pandya.
