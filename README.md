# HqllrBenchmarks — Performance & Scaling
*Measuring the future of sovereign AI.*

Hqllr is built for speed and verifiability. This repository showcases benchmark results across devices, corpora, and cluster scales.

---

## Highlights
- **Rapid Ingestion** — millions of words processed per second per core.  
- **Atomisation** — sentence- and paragraph-level indexing with zero duplication.  
- **Scalable** — parallel ingestion scales linearly with cores.  
- **Efficient** — optimised storage with filesystem compression.  
- **Portable** — consistent performance across mobile, desktop, and clusters.

---

## Recent Milestones
- 📚 *12,600 books (Project Gutenberg corpus) ingested in 4.5 minutes on an 8-core tablet (using 4 cores).*  
- ⚡ *Throughput doubled in the revised engine (Sep 2025), hitting new record speeds per core.*  
- 📊 *Consistent scaling: near-linear atoms/sec increase with core count.*  

---

## Methodology
- Benchmarks run on reference hardware (documented per test).  
- Tests are repeatable, using public corpora (e.g., Project Gutenberg).  
- Results reported in:
  - Files/sec
  - Atoms/sec (sentence, paragraph, page modes)
  - Scaling per core
  - Memory footprint (RSS)

---

## Roadmap
- [ ] Regular milestone benchmarks  
- [ ] Comparative scaling (mobile vs. desktop vs. cluster)  
- [ ] Public benchmark harness (later release)  
- [ ] Community benchmark submissions

---

## Why Benchmarks?
Performance is not just speed — it’s sovereignty:
- Fast enough to run locally, even on constrained devices.  
- Efficient enough to scale to enterprise clusters.  
- Transparent enough to verify.  


