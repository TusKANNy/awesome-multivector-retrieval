# CLAUDE.md

Guidelines for adding entries to this awesome list. This is a **hand-crafted, curated** list of resources on late-interaction multivector retrieval.

## Who decides what goes in

**The person proposing an addition decides whether it is worth including.** They may ask the agent for an opinion on relevance, quality, or placement, but that is a second opinion, not a gatekeeper — the agent can misjudge scope, misread a paper, or hallucinate details.

## Scope test

Include resources about **late-interaction / multivector retrieval**: ColBERT-style token-level embeddings scored with MaxSim, and the models, algorithms, engines, and kernels around them. Theory and analysis count, as long as they concern multivector retrieval. Blog posts count when highly relevant — for instance a model release with no accompanying paper.

## Where entries go

- **Models** → `Foundational Models`, `General Models & Training`, `Compression & Token Pruning`, `Multimodal & Vision`, or `Theory & Analysis`.
- **Retrieval** → `Indexing & Search Algorithms` or `Scoring Kernels`.
- **Software Libraries** → `Training & Inference Frameworks`, `Retrieval Engines & Indexes`, or `Scoring Kernels`. Code libraries, linked by their repo or homepage.
- **Model Checkpoints** → `General-Purpose` or `Specialized / Domain`. Released model weights, usually HuggingFace.
- **Datasets and Encodings** → datasets and their precomputed embeddings.
- **Multimedia Resources** → talks, podcasts, videos.

Papers and blog posts both belong in the Models and Retrieval sections, placed by topic. If unsure, put the entry next to the most thematically similar existing one.

**Within a section, entries run oldest first.** Insert by year rather than appending — only an entry from the newest year belongs at the end.

## How to add

### Papers

1. Add to `README.md` in the right section.
2. **Also add to `biblio.bib`** — every paper appears in both.

README entry format (indent continuation lines with tabs):

```markdown
- *Title*<br>
	Author One, Author Two, Author Three<br>
	Venue, Year<br>
	📄 [paper](https://arxiv.org/abs/...) | 🛠️ [code](https://github.com/...)
```

- **Paper link: the version a reader can actually open.** In order of preference: the publisher DOI when it is open access, the arXiv abstract page when the DOI is paywalled (ACM, Springer), an author-hosted PDF when there is no arXiv version, and the paywalled DOI when nothing open exists — it is still the record of the paper. `biblio.bib` keeps the published DOI either way. Check accessibility from outside an institutional network: a link that works on campus may be paywalled for everyone else.
- Add `🛠️ [code](...)` **only if code is publicly available**. Repeat the whole pair for a second repository.
- Venue: the published venue (`SIGIR, 2026`), `arXiv, 2026` for a preprint, or `<Workshop> Workshop, 2026` for a workshop paper — name the workshop, not its parent conference (`LIR Workshop, 2026`, not `ECIR (LIR Workshop), 2026`).

`biblio.bib` entry — tab indentation, fields ordered `title`, `author`, `booktitle`/`journal`, `year`, `pages` (optional), `doi`, `url`:

- Published venue, conference or workshop → `@inproceedings` with the full `booktitle`.
- arXiv preprint → `@article` with `journal={arXiv preprint arXiv:XXXX.XXXXX}` and `doi={10.48550/arXiv.XXXX.XXXXX}`.
- Include `doi` whenever one exists; omit the field entirely when the venue never assigned one (some NeurIPS and ACL Anthology proceedings).
- Citation key `lastnameYEARshortname`, where shortname is the resource's acronym or a one-or-two-word handle — `wang2026plaidprf`, `jha2026xtr`. Never a slug of the whole title.

ACM assigns some proceedings a `10.5555` placeholder prefix that **does not resolve through doi.org**. For those, link `https://dl.acm.org/doi/10.5555/...` directly and leave the `doi` field as the bare `10.5555/...` string.

### Blog posts (not papers)

README only — **do not** add to `biblio.bib`. Same list format, blog icon, `Blog` as the venue:

```markdown
- *Title*<br>
	Author or Org<br>
	Blog, Year<br>
	📝 [blog](https://...)
```

When the work was presented at a workshop but never published, name that workshop as the venue instead of `Blog`, keeping the 📝 icon and the blog link.

### Model checkpoints

`Model Checkpoints` section, **not** in `biblio.bib`. Always the full `org/model-name` taken from the HuggingFace URL, never a bare model name:

```markdown
- [org/model-name](https://huggingface.co/org/model-name)<br>
	*One-line description: size, base model, what makes it notable.*
```

### Software libraries

`Software Libraries` section, **not** in `biblio.bib`. Include a language logo image and a one-line description:

```markdown
- [Name](https://github.com/...) <img src="images/python-logo.svg" height="16" alt="Python"/><br>
	*One-line description.*
```

Logos available in `images/`: `python-logo.svg` (height 16), `rust-logo.png` (height 22), `cpp-logo.svg` (height 20), `java-logo.png` (height 16). Use several when a library has bindings in more than one language.

### Datasets and encodings

One `###` subsection per dataset: corpus stats as bullets, then one table row per available encoding.

```markdown
### `Dataset name`
- **Documents**: `1,234,567`
- **Queries** [`split`]: `1,000`
- **Reference Metric**: `MRR@10`

| Encoding | Link | Vector dim | Avg vectors per doc | Avg vectors per query | MRR@10 |
|---|---|---:|---:|---:|---:|
| `model` | [link](https://huggingface.co/datasets/...) | 128 | 67 | 32 | 0.397 |
```

Write `` `N/A` `` for a metric that was never measured, and add the new subsection to `## Contents`.

### Multimedia resources

One line, no icon:

```markdown
- Title, or a short description of the talk. [Link](https://...)
```

## Conventions

- Indent list continuation lines with **tabs**, matching surrounding entries.
- Icons: 📄 paper, 🛠️ code, 📝 blog. Separate multiple links with ` | `.
- Keep descriptions to one line; only cite performance numbers that come from the resource itself.
- Verify every link resolves and that authors, venue, and year are correct before adding.
- `## Contents` is hand-maintained — update it when adding or renaming a section.
