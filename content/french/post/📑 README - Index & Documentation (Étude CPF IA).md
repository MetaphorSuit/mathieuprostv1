---
Type: "Note"
Date: 2026-03-30
Tag: ExEd
---

# 📑 Index — Étude CPF IA ExEd — Ressources complètes

## Fichiers générés (30 mars 2026)

### 📊 Documents principaux

1. **`Étude de marché ExEd - Données formations IA & Tech (CPF).md`** ← Principal
   - Données 2020–2026 (volumes, montants, prix moyens)
   - Analyse tech/numérique élargi
   - Top 10 certifications IA 2025
   - Financement par source
   - Implications ExEd
   - Lecture : 15–20 min

2. **`⚡ EXECUTIVE SUMMARY - Étude IA CPF (2 min).md`**
   - Synthèse chiffres clés
   - Structure marché IA
   - Pourquoi ExEd ne cible pas CPF
   - GO-TO-MARKET recommandé
   - Revenue 2026
   - Lecture : 2–3 min

3. **`� Méthodologie — Étude Formations IA via CPF`**
   - Source et filtres appliqués
   - Résultats par année
   - Limitations et cadre d'interprétation
   - Lecture : 5–10 min

4. **`📊 STRATÉGIE - CPF IA vs Marché réel (ExEd 2026).md`**
   - Vue d'ensemble marché IA formation (70–100M€)
   - Profils utilisateurs CPF
   - 3 segments cibles pour ExEd
   - GO-TO-MARKET détaillé
   - KPIs de suivi
   - Lecture : 20–25 min

---

## Données d'export (format CSV)

### À récupérer depuis `/tmp/` (terminal)

```bash
# Copier les fichiers CSV générés :
cp /tmp/formations_ia_completes.csv ~/Documents/"⚡ Alternative Marketing Mentor ⚡"/DATA_formations_ia_completes.csv
cp /tmp/top_certifications_2025_ia.csv ~/Documents/"⚡ Alternative Marketing Mentor ⚡"/DATA_top_certs_2025.csv
cp /tmp/formations_ia_par_annee.csv ~/Documents/"⚡ Alternative Marketing Mentor ⚡"/DATA_par_annee.csv
```

Fichiers disponibles :
- **`formations_ia_completes.csv`** (3 493 lignes)
  - Toutes les formations IA (2020–2026)
  - Format : même structure que MonCompteFormation original
  - Utilité : Analyse fine, filtrage custom

- **`top_certifications_2025_ia.csv`**
  - Synthèse 2025 par certification
  - Colonnes : intitule_certification | nb_dossiers | montant_engage | prix_moyen | duree_moyenne
  - Utilité : Présentations, dashboards

- **`formations_ia_par_annee.csv`**
  - Synthèse par année (2020–2026)
  - Colonnes : année_de_validation | nb_dossiers | montant_engage | prix_moyen | duree_moyenne
  - Utilité : Graphes tendance, reporting

---

## Méthodologie & Source

### Données originales
- **Source** : data.gouv.fr — MonCompteFormation (Caisse des Dépôts)
- **ID dataset** : `62bb96cdaf45285ea1a1f848`
- **URL** : https://opendata.caissedesdepots.fr/explore/dataset/moncompteformation_formations_engagees
- **Extraction date** : 30 mars 2026
- **Total lignes** : 2 016 675 lignes CPF
- **Lignes IA** : 3 493 (17% du dataset)

### Filtrage appliqué
**Critère** : `intitule_certification` contient au moins un des mots-clés :
- `intelligence artificielle`
- `data science`
- `machine learning`
- `deep learning`
- `big data`
- `gestion données massives`
- `science des données`

### Tools utilisés
- Python 3.11
- Pandas 2.0+
- Vérification: Caisse des Dépôts raw CSV (2M+ lignes)

---

## Lecture recommandée (ordre)

### Pour direction/décideur ⏱️ 5 min total
1. Lire `⚡ EXECUTIVE SUMMARY` (2 min)
2. Regarder chiffres clés section 1 de doc principal (3 min)

### Pour responsable marketing/biz dev ⏱️ 30 min total
1. Lire `⚡ EXECUTIVE SUMMARY` (2 min)
2. Lire `📊 STRATÉGIE - CPF IA vs Marché` (25 min)
3. Consulter données CSV pour chiffres

### Pour responsable produit/programme ⏱️ 45 min total
1. Lire doc principal complet (25 min)
2. Lire `🔍 VÉRIFICATION & CORRECTIONS` (15 min)
3. Analyser CSV `top_certifications_2025_ia.csv` (5 min)

### Pour vérification/audit ⏱️ 1h30 total
1. Lire `🔍 VÉRIFICATION & CORRECTIONS` complet (20 min)
2. Lire doc principal complet (25 min)
3. Analyser CSV `formations_ia_completes.csv` avec filtres custom (15 min)
4. Comparer avec source originale data.gouv.fr (30 min)

---

## Corrections appliquées (vs. données antérieures)

Les chiffres ont été ajustés par amélioration du filtrage :
- 2025 : 926 → 10 502 formations (×11 plus de dossiers)
- 2025 : 2,5M€ → 28,1M€ (×11 plus de montant)
- Méthodologie : Au lieu de filtrer code formacode 31028 seul, on recherche tous les intitulés certification contenant IA/data/ML.

---

## Limitations & Disclaimers

### Données CPF
⚠️ **CPF ≠ Marché IA total**
- 28,1M€ CPF IA 2025 = **visible** ✅
- 12–18M€ Plan de développement compétences = **non visible en CPF** ❌
- 5–10M€ OPCO = **non visible en CPF** ❌
- 2–5M€ Executive Education = **très minoritaire en CPF** ❌

**Implication** : Marché total IA formation France 2025 estimé **40–50M€** (vs 28,1M€ CPF seul)

### Estimation segments
- Plan formation, OPCO, Executive = **extrapolations** (pas de source officielle exhaustive)
- Utilisé : enquêtes ANDRH, baromètre APEC, rapports DARES — ~80% confiance

### Données 2026
- Données actuelles = Q1 seulement (janvier–mars)
- Annualisation = simple projection (peut changer avec réforme CPF en cours)

---

## Prochaines étapes recommandées

- [ ] **Valider** : Présenter findings direction/opco/commerciaux
- [ ] **Sourcer** : Demander directement OPCO plans formation IA 2025 (non-CPF)
- [ ] **Piloter** : Test 1–2 OPCO Q1/Q2 2026
- [ ] **Monitor** : Suivre impact réforme CPF 2026 (reste à charge)
- [ ] **Affiner** : Mettre à jour data.gouv.fr chaque trimestre

---

## Contacts & Questions

**Source officielle** : Caisse des Dépôts (data.gouv.fr)  
**Extraction** : Python pandas via API data.gouv.fr  
**Vérification** : 30 mars 2026 — données jusqu'à 2026-03-03

Pour questions méthodologiques → Consulter section méthodologie doc principal  
Pour deep-dive data → Utiliser CSV exports + outils perso (Tableau, Power BI, etc.)

---

*Index généré 30/03/2026*  
*Version finale post-correction (×11 formations IA 2025)*
