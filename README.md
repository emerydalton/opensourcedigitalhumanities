# Open Source Digital Humanities

An open, reproducible workspace for textual research on Indo-European languages, beginning with Pali and Latin texts transmitted in Theravada and Catholic manuscript traditions.

## Research scope

Pali is a Middle Indo-Aryan language and Latin an Italic language; both belong to the Indo-European family. The project may compare their linguistic histories, texts, and transmission, but surviving Pali and Latin texts are not direct records of Proto-Indo-European. Language, textual tradition, and religious community should be described as distinct parts of each source's context.

## Standards and tools

- **Git** versions research materials and makes changes reviewable.
- **TEI P5 XML** is the preferred format for transcriptions and text editions. Use its manuscript description and source description elements to document witnesses and editorial choices.
- **IIIF** manifests or stable catalogue links can identify manuscript images. Link to images rather than copying them into this repository unless their reuse terms permit it.
- **Python and Jupyter notebooks** are suitable for reproducible text analysis; pandas can support tabular work and lxml can support XML processing. Keep tool and dependency versions with an analysis when code is added.
- **OpenRefine** can help clean and reconcile manuscript metadata before it is incorporated into the source register.

These are recommendations, not required dependencies. This starter repository does not yet include analysis code or a software environment.

## Repository layout

```text
data/
  source-register.csv   # Bibliographic, witness, and access information
  tei/                  # TEI transcriptions and editions
  derived/              # Reproducible, analysis-ready outputs
docs/                   # Research and editorial protocols
notebooks/              # Exploratory, reproducible analyses
scripts/                # Reusable processing steps
```

## Suggested workflow

1. Record each work, edition, manuscript witness, repository, shelfmark, and source URL in `data/source-register.csv`. Give each witness a stable project identifier.
2. Record access dates and reuse terms. Prefer stable catalogue records or IIIF manifests for images; do not assume that an online edition represents a particular manuscript witness.
3. Transcribe or encode texts in TEI P5, documenting the witness, editorial policy, and any supplied, corrected, or uncertain readings.
4. Preserve source transcriptions. Put normalized or otherwise transformed text in a clearly identified derived output, and document every transformation (including Unicode normalization and tokenization).
5. Keep analysis notebooks reproducible: state inputs, assumptions, and tool versions, and avoid editing source files from a notebook.
6. Cite editions, manuscript catalogues, and image sources in research outputs. Check rights and access conditions before redistributing any text or image.

## Getting started

Start by adding source records and research protocols. There is no installation step yet. When analysis code is introduced, use a project-local Python environment and record dependencies so that notebooks and scripts can be rerun.

See [`data/README.md`](data/README.md) for corpus and provenance guidance and [`data/tei/README.md`](data/tei/README.md) for TEI conventions.
