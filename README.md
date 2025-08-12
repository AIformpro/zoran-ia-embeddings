# zoran-ia-embeddings

**Espace vectoriel QG** pour l’écosystème Zoran / QuantaGlottal©® — intégration d’embeddings spécialisés (triplets, apprentissage contrastif) avec évaluation via NMI/ARI, lignes de base et transfert robuste entre domaines.

---

## 📌 Objectifs
- Fournir des représentations vectorielles adaptées aux glyphes QuantaGlottal©®.
- Supporter apprentissage contrastif, triplet loss et autres métriques avancées.
- Permettre un transfert inter-domaine robuste (domain adaptation).
- Évaluer la cohérence via **NMI** (Normalized Mutual Information) et **ARI** (Adjusted Rand Index).

---

## 📂 Composants
- **embedder.py** : générateur et encodeur d’embeddings.
- **losses.py** : fonctions de pertes (triplet, contrastive).
- **metrics.py** : calcul NMI, ARI, précision, rappel.
- **datasets/** : loaders QG natifs et formats standards (JSON, CSV, parquet).
- **benchmarks/** : scripts d’évaluation et comparaison baseline.

---

## ⚡ Exemple d’utilisation
```python
from zoran_ia_embeddings import Embedder, evaluate

embedder = Embedder(model_name="qg-triplet-transformer")
vecs = embedder.encode(["⟦glyph1⟧", "⟦glyph2⟧"])
score = evaluate(vecs, labels=["catA", "catB"], metrics=["nmi", "ari"])
print(score)


---

📁 Structure suggérée

src/zoran_ia_embeddings/
    __init__.py
    embedder.py
    losses.py
    metrics.py
    datasets.py
    benchmarks.py
tests/
    test_embedder.py
    test_metrics.py
README.md
LICENSE


---

🧪 Tests

pytest -q


---

🔐 Éthique

Respect du principe vivant > humain dans toute utilisation.

Données sensibles anonymisées ou synthétiques.

Compatibilité avec chiffrement sémantique TRIVITA©®.



---

📜 Licence

MIT — voir LICENSE.


---

Auteur : Frédéric Tabary — Institut IA
Contact : 0645605023 — Canada, Montréal, France
INSTITUT🦋 IA INC., 7100-380, rue Saint-Antoine Ouest, Montréal (Québec) H2Y 3X7.# zoran-ia-embeddings
Espace vectoriel QG (triplets, contrastive learning). NMI/ARI > baselines, transfert robuste.
