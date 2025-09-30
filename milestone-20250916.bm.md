----

# Hǫllr Benchmark


## Number Of CPU Cores: 4

### [MODE: msgpack CPU: 4] - RUN A (clean bloom + backend tmp)
🔍 Corpus: /literature, 
⚙️ Backend: msgpack, 👷 Workers: 4, 🔪 Splitter: Sentence, 🔪 N-Gram: 123 

```
👷 W1: starting with fresh bloom, 21 files, 67539 atoms, 45163 atoms/s, dedup: hit=6338, miss=61201
👷 W2: starting with fresh bloom, 20 files, 68819 atoms, 41950 atoms/s, dedup: hit=3524, miss=65295
👷 W0: starting with fresh bloom, 21 files, 72600 atoms, 43343 atoms/s, dedup: hit=3768, miss=68832
👷 W3: starting with fresh bloom, 20 files, 105184 atoms, 49750 atoms/s, dedup: hit=6853, miss=98331
✅ Ingestion complete, elapsed=0:02.90 user=6.37 sys=0.50 maxrss=45392KB CPU=237%
```

### [MODE: msgpack CPU: 4] - RUN B (reuse bloom + data)
🔍 Corpus: /literature, 
⚙️ Backend: msgpack, 👷 Workers: 4, 🔪 Splitter: Sentence, 🔪 N-Gram: 123
``` 
👷 W1: bootstrapped from cached worker bloom, 21 files, 67539 atoms, 74114 atoms/s, dedup: hit=67539, miss=0
👷 W2: bootstrapped from cached worker bloom, 20 files, 68819 atoms, 73755 atoms/s, dedup: hit=68819, miss=0
👷 W0: bootstrapped from cached worker bloom, 21 files, 72600 atoms, 69827 atoms/s, dedup: hit=72600, miss=0
👷 W3: bootstrapped from cached worker bloom, 20 files, 105184 atoms, 85762 atoms/s, dedup: hit=105184, miss=0
✅ Ingestion complete, elapsed=0:01.98 user=3.96 sys=0.34 maxrss=32508KB CPU=216%
```

---
