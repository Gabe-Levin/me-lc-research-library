---
title: ME/CFS + Long COVID Research Library
---

> [!tip] 💬 Chat with this library
> Synthesize across notes with **[NotebookLM](https://notebooklm.google.com/notebook/65dbf737-6de4-4d61-bf8d-911f06ce97c8)** — ask questions like *"compare LDN and rapamycin for Long COVID"* or *"which interventions does Dr. Chia recommend for the enterovirus subset?"* and get cited answers.

A queryable knowledge graph (~70 interlinked notes) covering [[ME-CFS]], [[Long COVID]], and related infection-associated chronic illnesses ([[IACCs]]): conditions, mechanisms, pathogens, treatments, and the researchers behind them.

Browse via the **graph view** in the sidebar, the **explorer** (folder tree), or jump straight to an entry point below.

## Attribution

This is a **graph-structured restructuring** of the public Google Doc maintained by **Sarah Healing** ([@sarahhhhealing](https://www.instagram.com/sarahhhhealing/) on Instagram), a medical student who has compiled and synthesized the research while sick herself. **All factual content, study citations, and clinical framings are hers.** This site only adds the graph structure — splitting sections into linked nodes, tagging them, and rendering the connections.

If you find this useful, please follow and credit her work directly.

> [!warning] Not medical advice
> Sarah is not a physician. The patient population this covers is sensitive to interventions — bring anything you read here to a qualified clinician before trying it.

## Entry points

### Conditions
[[ME-CFS]] · [[Long COVID]] · [[Post-Exertional Malaise]] · [[POTS]] · [[Dysautonomia]] · [[MCAS]] · [[EDS Hypermobility]] · [[Craniocervical Instability]] · [[Fibromyalgia]] · [[CIRS]] · [[IACCs]]

### Mechanisms
[[Mitochondrial Dysfunction]] · [[Oxidative Stress]] · [[Neuroinflammation]] · [[Viral Persistence and Reactivation]] · [[Microclots]] · [[HPA Axis Dysfunction]] · [[Autonomic Autoantibodies]] · [[Warburg Effect]]

### Pathogens
[[SARS-CoV-2]] · [[EBV]] · [[HHV-6]] · [[CMV]] · [[Enteroviruses]] · [[Lyme Bartonella Babesia]] · [[Mold Mycotoxins]]

### Treatments — categories
[[Mitochondrial Support]] · [[Antivirals]] · [[Immunotherapy]] · [[Anticoagulant Therapy]] · [[Nervous System Regulation]]

### Treatments — high-traffic specific nodes
[[Oxaloacetate]] · [[Methylene Blue]] · [[NAD Plus]] · [[Phosphatidylcholine]] · [[Red Light Therapy]] · [[HBOT]] · [[IVIG SCIG]] · [[Low Dose Naltrexone]] · [[Low Dose Rapamycin]] · [[Stem Cells]] · [[Stellate Ganglion Block]] · [[Ampligen]] · [[Immunoadsorption]] · [[Valacyclovir]] · [[Truvada]] · [[Maraviroc]] · [[Paxlovid]] · [[Remdesivir]] · [[Oxymatrine Equilibrant]] · [[Dihydroquercetin]] · [[Low Dose Abilify]]

### People
[[Sarah Healing]] (author) · [[Dr Putrino]] · [[Dr Chia]] · [[Dr Davis]] · [[Dr Klimas]] · [[Dr Liu]] · [[Dr Hanson]] · [[Dr Lerner]] · [[Dr Younger]]

## Tag taxonomy

Every note has YAML frontmatter tags:

- **`type/`** — `condition` · `mechanism` · `pathogen` · `treatment` · `treatment-category` · `person` · `symptom` · `concept`
- **`system/`** — `mito` · `immune` · `neuro` · `autonomic` · `vascular` · `endocrine` · `connective` · `structural`
- **`class/antiviral`** — for antiviral treatments

In the **graph view**, you can color-code by tag group. In the **tag pane**, the tag tree gives you a clickable index by `type/X` or `system/X`.

## Graph overview

```mermaid
graph TD
  IACC[IACCs / Infection-Associated]
  ME[ME-CFS]
  LC[Long COVID]
  PEM[Post-Exertional Malaise]

  Mito[Mitochondrial Dysfunction]
  Neuro[Neuroinflammation]
  Viral[Viral Persistence / Reactivation]
  Auto[Autonomic Autoantibodies]
  Clots[Microclots]
  Ox[Oxidative Stress]

  POTS[POTS / Dysautonomia]
  MCAS[MCAS]
  EDS[EDS / Hypermobility]
  CCI[CCI / AAI / Chiari]

  EBV[EBV]
  HHV6[HHV-6]
  EV[Enteroviruses]
  Lyme[Lyme+]
  Mold[Mold / Mycotoxins]
  CoV[SARS-CoV-2]

  IACC --> ME
  IACC --> LC
  ME -.PEM hallmark.-> PEM
  LC -.~50% meet ME criteria.-> ME

  PEM --> Mito
  PEM --> Clots
  PEM --> Neuro
  PEM --> Viral

  CoV --> LC
  CoV --> EBV
  EBV --> ME
  HHV6 --> ME
  EV --> ME
  Lyme -.subset.-> ME
  Mold -.CIRS subset.-> ME

  ME --> POTS
  ME --> MCAS
  ME --> EDS
  ME --> CCI
  Auto --> POTS
  Auto --> ME
```

## Use this content elsewhere

- **AI chat (this library):** [NotebookLM notebook](https://notebooklm.google.com/notebook/65dbf737-6de4-4d61-bf8d-911f06ce97c8)
- **As your own Obsidian vault:** clone the [GitHub repo](https://github.com/gabe-levin/me-lc-research-library), open `content/` as a vault
- **AI chat (custom):** the markdown is plain text — drop into Claude Projects, a Custom GPT, or any RAG pipeline

## License

[CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/). Source content credit to Sarah Healing. Attribution required; share-alike for derivative works.
