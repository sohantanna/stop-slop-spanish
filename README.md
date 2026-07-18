# Basta de Relleno

Una skill para quitar los rasgos de IA de los textos en español, con cobertura de todas las variedades del idioma.

> Adaptación al español de [**Stop Slop**](https://github.com/hardikpandya/stop-slop), de [Hardik Pandya](https://hvpandya.com).

---

## 🇪🇸 Español

### Qué es esto

La escritura de IA tiene patrones: frases, estructuras y ritmos predecibles. Esta skill le enseña a Claude (o a cualquier LLM) a detectarlos y quitarlos **en español**.

No es una traducción del proyecto original. Los rasgos de IA en inglés no son los mismos que en español, así que esta versión persigue los propios de nuestro idioma:

- el carraspeo de **"Cabe destacar que"**, **"En el mundo actual"**, **"Hoy en día"**;
- los adjetivos-comodín de folleto: **"crucial"**, **"fundamental"**, **"robusto"**, **"vibrante"**;
- la estructura **"no solo… sino también"** y el **"No es X, sino Y"**;
- la **pasiva refleja** que esconde al responsable: **"se tomó la decisión"**, **"se puede observar que"**;
- el montón de adverbios en **-mente** y los calcos del inglés (**"hacer sentido"**, **"en base a"**, **"aplicar para"**).

Y añade un problema que el inglés no tiene: la **variación regional**. La IA mezcla el voseo con el tuteo, "ustedes" con "vosotros", "coche" con "carro", o cae en un **"español neutro"** sin dueño. Esta skill vigila esa incoherencia y ayuda a elegir una sola variedad y mantenerla.

### El objetivo

Prosa en español que suene humana: directa, concreta, con ritmo y con voz de un lugar concreto. Menos folleto, menos relleno, menos "neutro" de nadie.

### Estructura de la skill

```
stop-slop-spanish/
├── SKILL.md                          # Instrucciones principales
├── references/
│   ├── frases.md                     # Frases que hay que quitar
│   ├── estructuras.md                # Estructuras que hay que evitar
│   ├── variaciones-regionales.md     # Cobertura panhispánica
│   └── ejemplos.md                   # Transformaciones antes/después
├── README.md
├── CHANGELOG.md
└── LICENSE
```

### Inicio rápido

- **Claude Code:** añade esta carpeta como skill.
- **Proyectos de Claude:** sube `SKILL.md` y los archivos de `references/` al conocimiento del proyecto.
- **Instrucciones personalizadas:** copia las reglas principales de `SKILL.md`.
- **Llamadas a la API:** incluye `SKILL.md` en el *system prompt*. Los archivos de referencia se cargan cuando hacen falta.

### Qué detecta

- **Frases vetadas** — aperturas de carraspeo, muletillas de énfasis, jerga corporativa, calcos del inglés, adverbios en *-mente* vacíos, adjetivos-comodín, meta-comentario y declaraciones vagas. Ver `references/frases.md`.
- **Clichés estructurales** — contrastes binarios, "no solo… sino también", enumeración por negación, fragmentación dramática, montajes retóricos, falsa agencia, narrador a distancia, voz pasiva y pasiva refleja. Ver `references/estructuras.md`.
- **Coherencia regional** — mezclas de voseo/tuteo/ustedeo, "ustedes" frente a "vosotros", vocabulario de regiones distintas, palabras vulgares según el país y el "neutro" sin sabor. Ver `references/variaciones-regionales.md`.

### Variedades cubiertas

España, México, Guatemala, Honduras, El Salvador, Nicaragua, Costa Rica, Panamá, Cuba, República Dominicana, Puerto Rico, Colombia, Venezuela, Ecuador, Perú, Bolivia, Chile, Argentina, Uruguay, Paraguay, Guinea Ecuatorial y el español de Estados Unidos.

### Puntuación

Puntúa de 1 a 10 cada dimensión:

| Dimensión | Pregunta |
|-----------|----------|
| Franqueza | ¿Afirmaciones o anuncios? |
| Ritmo | ¿Variado o metronómico? |
| Confianza | ¿Respeta la inteligencia de quien lee? |
| Autenticidad | ¿Suena humano? |
| Densidad | ¿Sobra algo cortable? |
| Coherencia regional | ¿Una sola variedad, sin mezclas? |

Menos de 42/60: revisa.

### Créditos

Proyecto original: [**Stop Slop**](https://github.com/hardikpandya/stop-slop) de [Hardik Pandya](https://hvpandya.com). Todo el mérito de la idea, la estructura y el método es suyo. Esta es una adaptación al español que reescribe las listas y añade la cobertura regional panhispánica.

### Licencia

MIT. Úsalo con libertad, compártelo sin límites. Ver [LICENSE](LICENSE).

---

## 🇬🇧 English

**Basta de Relleno** ("Enough with the filler") is a skill for removing AI tells from Spanish-language prose, with coverage of every regional variety of the language.

It is the Spanish adaptation of [**Stop Slop**](https://github.com/hardikpandya/stop-slop) by [Hardik Pandya](https://hvpandya.com).

### What this is

AI writing has patterns: predictable phrases, structures, and rhythms. This skill teaches Claude (or any LLM) to catch and remove them **in Spanish**.

It is not a translation of the original. AI tells in English are not the same as in Spanish, so this version targets the Spanish-specific ones:

- throat-clearing openers like *"Cabe destacar que"*, *"En el mundo actual"*, *"Hoy en día"*;
- brochure-adjectives: *"crucial"*, *"fundamental"*, *"robusto"*, *"vibrante"*;
- the *"no solo… sino también"* ("not only… but also") and *"No es X, sino Y"* structures;
- the *pasiva refleja* that hides the actor: *"se tomó la decisión"*, *"se puede observar que"*;
- the pile-up of *-mente* adverbs and English calques (*"hacer sentido"*, *"en base a"*, *"aplicar para"*).

And it adds a problem English does not have: **regional variation**. AI mixes *voseo* with *tuteo*, *ustedes* with *vosotros*, *coche* with *carro*, or falls into a rootless *"español neutro"* that belongs to no one. This skill flags that inconsistency and helps you pick one variety and stay in it.

### The goal

Spanish prose that sounds human: direct, specific, varied in rhythm, and rooted in a real place. Less brochure, less filler, less no-one's-*neutro*.

### Skill structure

```
stop-slop-spanish/
├── SKILL.md                          # Core instructions
├── references/
│   ├── frases.md                     # Phrases to remove
│   ├── estructuras.md                # Structural patterns to avoid
│   ├── variaciones-regionales.md     # Pan-Hispanic coverage
│   └── ejemplos.md                   # Before/after transformations
├── README.md
├── CHANGELOG.md
└── LICENSE
```

### Quick start

- **Claude Code:** add this folder as a skill.
- **Claude Projects:** upload `SKILL.md` and the `references/` files to project knowledge.
- **Custom instructions:** copy the core rules from `SKILL.md`.
- **API calls:** include `SKILL.md` in your system prompt. Reference files load on demand.

### What it catches

- **Banned phrases** — throat-clearing openers, emphasis crutches, business jargon, English calques, empty *-mente* adverbs, filler adjectives, meta-commentary, and vague declaratives. See `references/frases.md`.
- **Structural clichés** — binary contrasts, *"no solo… sino también"*, negative listing, dramatic fragmentation, rhetorical setups, false agency, narrator-from-a-distance, passive voice, and *pasiva refleja*. See `references/estructuras.md`.
- **Regional consistency** — mixing *voseo*/*tuteo*/*ustedeo*, *ustedes* vs *vosotros*, cross-region vocabulary, region-specific vulgarities, and flavorless *neutro*. See `references/variaciones-regionales.md`.

### Varieties covered

Spain, Mexico, Guatemala, Honduras, El Salvador, Nicaragua, Costa Rica, Panama, Cuba, Dominican Republic, Puerto Rico, Colombia, Venezuela, Ecuador, Peru, Bolivia, Chile, Argentina, Uruguay, Paraguay, Equatorial Guinea, and United States Spanish.

### Scoring

Rate 1–10 on each dimension:

| Dimension | Question |
|-----------|----------|
| Directness | Statements or announcements? |
| Rhythm | Varied or metronomic? |
| Trust | Respects reader intelligence? |
| Authenticity | Sounds human? |
| Density | Anything cuttable? |
| Regional consistency | One variety, no mixing? |

Below 42/60: revise.

### Credits

Original project: [**Stop Slop**](https://github.com/hardikpandya/stop-slop) by [Hardik Pandya](https://hvpandya.com). All credit for the idea, structure, and method is his. This is a Spanish adaptation that rewrites the lists and adds pan-Hispanic regional coverage.

### License

MIT. Use freely, share widely. See [LICENSE](LICENSE).
