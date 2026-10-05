# TESSERA v1.1 and PREDICTS relative abundance

Predicts within-study relative abundance at PREDICTS sites (studies from 2000 on) from TESSERA v1.1 embeddings with a mixed-effects random forest (MERF) on 32 principal components.

```
uv sync
uv run jupyter nbconvert --execute --to notebook --inplace tessera_v11_abundance.ipynb
```

The PREDICTS extract is in `data/PREDICTs_coords.csv`. The first run streams ~18k embedding windows from Source Cooperative, which takes several minutes, and caches them in `data/`.
