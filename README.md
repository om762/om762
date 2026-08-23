<div align="center">

<img src="./assets/desk.png" width="100%" alt="Omprakash Rawat's engineering desk — laptop, dual monitors, iPad with handwritten note 'I like solving problems that annoy me', earbuds, cold coffee, sticky notes with ideas, data pipeline sketch showing source → Spark → data flow, and a to-do list: focus, build, iterate." />

<br>

`software · data · systems`

</div>

<br>

<sub>currently thinking about →</sub>

### currently

```
→ building Vibely
→ getting deeper into Databricks
→ learning Agentic AI
→ exploring DevOps workflows
```

<sub>last scribbled · 26.08.23</sub>

---

## things I build

> I tend to build things when something starts annoying me.

<br>

### BlockFit

> Notion couldn't handle the thing I wanted to paste into it.

Long, richly formatted LLM responses can hit Notion's paste payload limit. Splitting them manually destroys formatting — browser text selection and an LLM's native Copy button use different clipboard pipelines.

There was no good existing solution. So I built the missing piece.

`React` · `TypeScript` · `DOMPurify` · `react-window`

<details>
<summary>&nbsp;how it works →</summary>

<br>

The interesting part wasn't the UI.

It was understanding what actually happens inside the clipboard:

```
HTML clipboard data
      ↓
plain text clipboard data
      ↓
browser clipboard APIs
      ↓
OS clipboard behavior
      ↓
format preservation
      ↓
safe chunking
      ↓
virtualized rendering
```

The splitter has to divide long formatted content without destroying the structure. You can't just split HTML at arbitrary byte boundaries — you need to understand the DOM tree, preserve nesting, and handle edge cases in block vs. inline elements.

I ended up learning more about clipboard formats than I expected.

</details>

<br>

[`live →`](https://blockfit-om762.vercel.app)&ensp;·&ensp;[`source`](https://github.com/om762/BlockFit)

---

### Roadmap

> Learning something new shouldn't mean losing track of where you are.

Started as a personal learning tool. Evolved into a full platform — creating, sharing, following roadmaps, and tracking progress. Community-driven, publicly accessible, built entirely solo.

> The difficult part wasn't creating a roadmap.  
> It was changing one without breaking somebody else's progress.

When an owner edits a published roadmap, users following the old version need to keep their progress intact. The system handles roadmap versioning — version changes don't destroy existing progress, silently overwrite user state, or break old references.

`Django` · `React` · `MySQL` · `custom CSS`

<details>
<summary>&nbsp;what made it interesting →</summary>

<br>

The versioning problem sits at the intersection of:

- complex relational data modeling
- state consistency across users
- progress tracking against a moving target
- keeping old references valid while supporting new structure

This isn't a CRUD app with a roadmap skin. The data model has to handle version branches, user-progress snapshots, and structural changes without creating orphaned or inconsistent states.

Still maintaining it.

</details>

<br>

[`live →`](https://om762.pythonanywhere.com)&ensp;·&ensp;[`source`](https://github.com/om762/Roadmap)&ensp;·&ensp;`still maintaining`

---

### Vibely

> Your likes are data. Why are they still a mess?

Likes and saves across Spotify, YouTube, Pinterest — they all become one giant unsorted pile. Vibely explores using AI to automatically organize saved content into playlists, boards, and collections that actually make sense.

`React Native` · `Python` · `PostgreSQL` · `AWS` · `Redis` · `Docker` · `AI/LLMs`

[`source`](https://github.com/om762/Vibely)&ensp;·&ensp;`currently cooking 🍳`

---

## small things

### Typestrike

> A terminal typing test because leaving the terminal felt unnecessary.

Interactive terminal rendering in Node.js. Zero dependencies. Distributed as a single executable using Node.js SEA.

`Node.js` · `zero dependencies` · `SEA`&ensp;·&ensp;[`source`](https://github.com/om762/Typestrike)&ensp;·&ensp;`released`

<br>

### TeamFinder

> Find people to build with.

`Next.js` · `TypeScript` · `TailwindCSS` · `AWS DynamoDB` · `S3`&ensp;·&ensp;[`live →`](https://team-finder-xi.vercel.app/)&ensp;·&ensp;[`source`](https://github.com/om762/teamFinder)

---

## why I build

<div align="center">
<img src="./assets/why-i-build.svg" width="100%" alt="Three handwritten principles: 01 — solve the annoying thing, not the theoretical thing; 02 — hide complexity until it's needed, like Notion does; 03 — make the final thing better than the first idea, don't just make it work." />
</div>

---

## rabbit holes

Things I keep going deeper into instead of sleeping:

`AI agents` · `data systems` · `system design` · `minimal interfaces` · `micro-optimizations` · `building niche products`

<br>

<div align="center">
<img src="./assets/rabbit-hole.svg" width="65%" alt="Notebook card: rabbit hole #04 — how much abstraction is actually useful before it starts hiding the system? Currently investigating." />
</div>

---

## by day

<div align="center">
<img src="./assets/by-day.svg" width="100%" alt="Data engineering pipeline: different data sources flow through migration and ingestion into Databricks lakehouse, then processed via Spark and SQL into useful data. Technologies: Databricks, Azure, Azure Data Factory, PySpark, Spark SQL, Python, SQL." />
</div>

---

## what's on the desk

```
Python          SQL             JavaScript
Django          React           PySpark
Spark           Databricks      Azure
AWS             Docker          PostgreSQL
TypeScript      Node.js         React Native
```

<sub>no proficiency bars. the projects speak.</sub>

---

<details>
<summary>&ensp;things I'm figuring out</summary>

<br>

```
→ DevOps — pipelines, repos, test plans
→ Databricks Asset Bundles
→ Agentic AI — how agents actually work, not just the API calls
```

What I want to learn next:

```
→ AI function calling
→ AWS SageMaker
→ MLOps
```

This section grows as I experiment.

</details>

---

## elsewhere

[`GitHub`](https://github.com/om762)&ensp;·&ensp;[`LinkedIn`](https://www.linkedin.com/in/om762/)&ensp;·&ensp;[`Website`](https://om762.pythonanywhere.com)&ensp;·&ensp;[`X`](https://x.com/OmPrakash_762)

---

<div align="center">
<img src="./assets/footer.svg" width="60%" alt="desk status: still building — Omprakash Rawat, 2026" />
</div>
