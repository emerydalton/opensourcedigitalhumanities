# Research data

Keep a source record for every text, edition, manuscript witness, or digital resource used in the project in [`source-register.csv`](source-register.csv). Use one row per resource or witness and stable project identifiers in `record_id` and `witness_id`.

Record source URLs, catalogue references, access dates (use `YYYY-MM-DD`), and known license or reuse terms. A digitized edition and a manuscript witness are different sources; describe them separately. Do not add manuscript images or third-party transcriptions unless their rights and access terms allow redistribution. Prefer linking to an authoritative catalogue record or IIIF manifest.

TEI P5 files belong in [`tei/`](tei/). Keep those source transcriptions distinct from normalized text, token lists, or other derived data. Put derived outputs in [`derived/`](derived/) and identify their source records and processing steps.
