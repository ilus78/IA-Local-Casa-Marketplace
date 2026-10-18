# IA Local Casa Marketplace

Catálogo público de complementos del proyecto IA Local Casa para ChatGPT y Codex. Reúne habilidades reutilizables para apoyar las tareas del proyecto.

## Qué incluye

Actualmente, el catálogo ofrece `vercel-curated-skills` (versión `0.1.0`), una selección de habilidades de Vercel. Una habilidad es un conjunto de instrucciones que guía al asistente en una tarea:

| Habilidad | Para qué sirve |
| --- | --- |
| [Web Design Guidelines](plugins/vercel-curated-skills/skills/web-design-guidelines/SKILL.md) | Revisar código de interfaces web según las pautas de Vercel, incluida la accesibilidad |
| [Writing Guidelines](plugins/vercel-curated-skills/skills/writing-guidelines/SKILL.md) | Revisar textos y documentación para mejorar su claridad, estructura y estilo |

Ambas consultan las pautas publicadas por Vercel antes de cada revisión, por lo que necesitan acceso a internet.

## Añadir el marketplace en ChatGPT/Codex

Esta ruta requiere Codex CLI instalado y la aplicación de escritorio con acceso al directorio de complementos.

1. Ejecuta este comando en la terminal para registrar el repositorio como fuente:

   ```bash
   codex plugin marketplace add ilus78/IA-Local-Casa-Marketplace
   ```

2. Reinicia la aplicación de escritorio de ChatGPT/Codex.
3. Abre **Plugins** (complementos) y selecciona **IA Local Casa** en las fuentes del directorio.

El identificador del marketplace es `ia-local-casa`. Si no aparece, comprueba las fuentes registradas:

```bash
codex plugin marketplace list
```

Consulta la [documentación oficial sobre marketplaces](https://developers.openai.com/plugins/build/plugins#add-a-marketplace-from-the-cli) si tu versión no ofrece estas opciones.

## Instalar vercel-curated-skills

Añadir el marketplace permite explorar su catálogo. Para instalar el complemento:

1. Dentro de **IA Local Casa**, abre `vercel-curated-skills`.
2. Selecciona la opción de instalación.
3. Abre un chat nuevo para usar las habilidades.

Por ejemplo, con el README disponible en el chat o proyecto:

> Usa la habilidad Writing Guidelines para revisar el README. No modifiques nada; indica qué mejorarías.

Consulta la [guía oficial de complementos](https://learn.chatgpt.com/docs/plugins) para conocer las superficies compatibles y las opciones de instalación.
