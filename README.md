# 🛒 METRO France – Product Category Taxonomy Dataset (Food & Non-Food)

## Description

This dataset contains the full **product category taxonomy of METRO France (metro.fr)**, the wholesale supplier of food and equipment for professionals (restaurants, hotels, cafés, caterers, retailers).

It covers **1,436 categories** organised in a hierarchy of up to **5 levels**, split between:
- **Food**: 443 categories (Beverages, Grocery, Fresh, Frozen),
- **Non-food**: 993 categories (professional kitchen & catering equipment, tableware, furniture, hygiene, packaging, office supplies, high-tech, workwear…).

It is designed for:
- product classification and catalogue mapping,
- e-commerce and marketplace taxonomy alignment,
- B2B market and assortment analysis (food service / HoReCa),
- AI, RAG systems and product-matching models,
- open data projects.

The dataset is available in **CSV** and **LLM-optimized JSON** formats.

---

## Key figures

- 5 top-level categories: Beverages (Boissons), Grocery (Epicerie), Fresh (Frais), Frozen (Surgelés), Non-food (Non alimentaire)
- 27 level-2 categories
- 1,723 unique category nodes across all levels
- 1,436 end categories (leaves): 443 food / 993 non-food
- Maximum depth: 5 levels

---

## Dataset content

- `metro_product_categories.csv`: classic tabular format (one row per end category, with its full path)
- `metro_product_categories.json`: structured and hierarchical format (category tree)

### Main structure (CSV)

- `category_id`: unique identifier (METRO-CAT-0001…)
- `product_type`: `food` / `non-food`
- `product_type_fr`: `Alimentaire` / `Non alimentaire`
- `level_1` to `level_5`: category name at each level (empty when the level does not exist)
- `category_name`: name of the end category
- `category_depth`: number of levels (2 to 5)
- `category_path`: full path (e.g. `Boissons > Brasserie > Bière > Bière Ale`)
- `source`

### Main structure (JSON)

- `name`
- `product_type` / `product_type_fr` (level 1)
- `level`
- `path`
- `category_id` (end categories)
- `subcategory_count`
- `subcategories` (nested children, same structure)
- `source` (level 1)

Category names are in **French**, as published on metro.fr.

---

## Coverage

- Country: France
- Scope: METRO France online catalogue (metro.fr), food and non-food

### Top-level categories

- **Boissons** (Beverages): beer & soft drinks (Brasserie), spirits (Spiritueux), wine & champagne (Vin et champagne)
- **Epicerie** (Grocery): savoury grocery (Epicerie salée), sweet grocery (Epicerie sucrée)
- **Frais** (Fresh): cold cuts (Charcuterie)
- **Surgelés** (Frozen): meat, fish, vegetables, fruit, bread & pastry, ice cream, ready meals, appetisers…
- **Non alimentaire** (Non-food): professional catering equipment & appliances (Matériel CHR & Electroménager), furniture & fittings (Mobilier & Agencement), tableware & kitchen utensils (Art de la table & Ustensile de cuisine), office supplies (Fourniture de bureau), hygiene & cleaning (Hygiène, Entretien & Nettoyage), high-tech & IT, workwear & professional linen, disposables & food packaging, outdoor fittings, checkout & payment

---

## Use cases

- Product classification and catalogue structuring
- Mapping supplier or marketplace taxonomies to a wholesale reference
- Food service / HoReCa market studies
- AI-powered assistants, product search and RAG pipelines
- Training and evaluating product categorisation models
- Open data and research projects

---

## Methodology

- Data extracted from the METRO France product nomenclature (metro.fr)
- Cleaning and normalization (encoding fixes, whitespace removal, deduplication)
- Food / non-food flag added from the top-level category
- Structured for **human and machine consumption**
- No personal data included

---

## License

CC-BY 4.0 – Attribution: METRO France (metro.fr)

---

## Disclaimer

Data represents a snapshot in time (October 2026) and may change.
No guarantee of completeness or permanent accuracy.

---

# 🛒 METRO France – Nomenclature des produits alimentaires et non alimentaires (dataset)

## Description

Ce dataset recense l'ensemble de la **nomenclature des catégories de produits de METRO France (metro.fr)**, grossiste alimentaire et matériel pour les professionnels (restaurateurs, hôteliers, cafetiers, traiteurs, commerçants).

Il couvre **1 436 catégories** organisées selon une arborescence allant jusqu'à **5 niveaux**, réparties entre :
- **Alimentaire** : 443 catégories (Boissons, Epicerie, Frais, Surgelés),
- **Non alimentaire** : 993 catégories (matériel CHR et électroménager, art de la table, mobilier, hygiène, emballage, fourniture de bureau, high-tech, vêtement professionnel…).

Il est destiné à des usages de :
- classification produits et structuration de catalogues,
- alignement de taxonomies e-commerce et marketplace,
- analyse de marché et d'assortiment B2B (restauration / CHR),
- systèmes RAG, applications IA et modèles de rapprochement produits,
- projets open data.

Les données sont structurées et disponibles en **CSV** et **JSON optimisé pour les LLMs**.

---

## Chiffres clés

- 5 catégories de niveau 1 : Boissons, Epicerie, Frais, Surgelés, Non alimentaire
- 27 catégories de niveau 2
- 1 723 catégories uniques, tous niveaux confondus
- 1 436 catégories finales : 443 alimentaires / 993 non alimentaires
- Profondeur maximale : 5 niveaux

---

## Contenu du dataset

- `metro_product_categories.csv` : format tabulaire classique (une ligne par catégorie finale, avec son chemin complet)
- `metro_product_categories.json` : format structuré et hiérarchique (arbre des catégories)

### Structure principale (CSV)

- `category_id` : identifiant unique (METRO-CAT-0001…)
- `product_type` : `food` / `non-food`
- `product_type_fr` : `Alimentaire` / `Non alimentaire`
- `level_1` à `level_5` : nom de la catégorie à chaque niveau (vide si le niveau n'existe pas)
- `category_name` : nom de la catégorie finale
- `category_depth` : nombre de niveaux (2 à 5)
- `category_path` : chemin complet (ex. `Boissons > Brasserie > Bière > Bière Ale`)
- `source`

### Structure principale (JSON)

- `name`
- `product_type` / `product_type_fr` (niveau 1)
- `level`
- `path`
- `category_id` (catégories finales)
- `subcategory_count`
- `subcategories` (sous-catégories imbriquées, même structure)
- `source` (niveau 1)

Les libellés des catégories sont en **français**, tels que publiés sur metro.fr.

---

## Périmètre

- Pays : France
- Périmètre : catalogue en ligne METRO France (metro.fr), alimentaire et non alimentaire

### Catégories de niveau 1

- **Boissons** : brasserie (bières, softs, eaux, sirops), spiritueux, vin et champagne
- **Epicerie** : épicerie salée, épicerie sucrée
- **Frais** : charcuterie
- **Surgelés** : viande, poisson, légumes, fruits, pain et pâtisserie, glaces, plats cuisinés, apéritifs…
- **Non alimentaire** : matériel CHR et électroménager, mobilier et agencement, art de la table et ustensiles de cuisine, fourniture de bureau, hygiène et entretien, high-tech et informatique, vêtement et linge professionnel, jetable et emballage alimentaire, aménagement extérieur, encaissement et monétique

---

## Cas d'usage

- Classification produits et structuration de catalogues
- Rapprochement de taxonomies fournisseurs ou marketplace avec un référentiel grossiste
- Études de marché restauration / CHR
- Alimentation de modèles IA (RAG, agents, assistants, recherche produit)
- Entraînement et évaluation de modèles de catégorisation produits
- Projets open data et recherche

---

## Méthodologie

- Extraction à partir de la nomenclature produits de METRO France (metro.fr)
- Nettoyage et normalisation (correction d'encodage, espaces superflus, dédoublonnage)
- Ajout d'un indicateur alimentaire / non alimentaire à partir du niveau 1
- Structuration orientée **machine + humain**
- Aucune donnée personnelle

---

## Licence

CC-BY 4.0 – Attribution : METRO France (metro.fr)

---

## Avertissement

Les informations peuvent évoluer dans le temps.
Ce dataset représente un état à date (octobre 2026), sans garantie d'exhaustivité ou d'exactitude permanente.
