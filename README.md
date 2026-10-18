# IA Local Casa Marketplace

Catálogo público de complementos del proyecto IA Local Casa para ChatGPT y Codex. Reúne habilidades reutilizables para apoyar las tareas del proyecto.

## Qué incluye

Actualmente, el catálogo ofrece `vercel-curated-skills` (versión `0.1.0`), una selección de habilidades de Vercel. Una habilidad es un conjunto de instrucciones que guía al asistente en una tarea:

| Habilidad | Para qué sirve |
| --- | --- |
| [Web Design Guidelines](plugins/vercel-curated-skills/skills/web-design-guidelines/SKILL.md) | Revisar código de interfaces web según las pautas de Vercel, incluida la accesibilidad |
| [Writing Guidelines](plugins/vercel-curated-skills/skills/writing-guidelines/SKILL.md) | Revisar textos y documentación para mejorar su claridad, estructura y estilo |

Ambas consultan las pautas publicadas por Vercel antes de cada revisión, por lo que necesitan acceso a internet.

## Añadir el marketplace en ChatGPT

La forma más sencilla es desde la interfaz de ChatGPT Desktop:

1. Abre **Configuración → Complementos**.
2. Selecciona **Añadir → Añadir un marketplace**.
3. En **Origen**, escribe `ilus78/IA-Local-Casa-Marketplace`.
4. En **Referencia de Git**, deja `main`.
5. Deja **Rutas dispersas** vacío.
6. Selecciona **Añadir marketplace**.
7. En la sección **Personales**, abre **IA Local Casa**.

El identificador interno del marketplace es `ia-local-casa`.

## Instalar vercel-curated-skills

Añadir el marketplace permite explorar su catálogo. Para instalar el complemento:

1. Dentro de **IA Local Casa**, abre `vercel-curated-skills`.
2. Selecciona **Instalar complemento**.
3. Confirma que aparecen las habilidades **Web Design Guidelines** y **Writing Guidelines**.
4. Abre un chat nuevo para usarlas.

Por ejemplo:

> Usa la habilidad Writing Guidelines para revisar el README. No modifiques nada; indica qué mejorarías.

## Alternativa con Codex CLI

Para usuarios que prefieran la terminal y dispongan de Codex CLI, el marketplace también se puede registrar con:

```bash
codex plugin marketplace add ilus78/IA-Local-Casa-Marketplace
```

Después puede comprobarse con:

```bash
codex plugin marketplace list
```

## Alcance

Este repositorio es público y contiene únicamente el marketplace, sus metadatos y las skills publicadas. La configuración privada, documentación interna, históricos y otros materiales del proyecto permanecen en el repositorio privado `IA-Local-Casa`.
