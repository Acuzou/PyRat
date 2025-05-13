# PyRat – Exemples d’algorithmes pour le Problème du Voyageur de Commerce (TSP)

## Présentation

Ce dépôt propose plusieurs implémentations d’algorithmes pour résoudre le Problème du Voyageur de Commerce (Travelling Salesman Problem, TSP) au sein du framework **PyRat**. Chaque notebook explore une stratégie différente, de la force brute à des heuristiques gloutonnes améliorées.

## Arborescence du projet

```
.
├── DFS_Pyrat.ipynb            # Parcours en profondeur (Depth‑First Search)
├── Greedy_1_1.ipynb           # Heuristique gloutonne (voisin le plus proche)
├── Greedy_4_4.ipynb           # Variante gloutonne 4‑4
├── Greedy_4_4_amelioré.ipynb  # Variante gloutonne 4‑4 améliorée
├── TSP_Brute.ipynb            # Recherche exhaustive (brute force)
└── README.md                  # Vous êtes ici
```

## Pré‑requis

- Python 3.9+
- pip 23+
- **JupyterLab** ou **Jupyter Notebook**
- Bibliothèques :
  - `numpy`
  - `matplotlib`
  - `networkx`

Installez‑les en une seule commande :

```bash
pip install -r requirements.txt
```

> **Astuce :** Vous pouvez générer automatiquement le fichier `requirements.txt` depuis les notebooks avec :
> ```bash
> pipreqs .
> ```

## Installation

Clonez le dépôt :

```bash
git clone https://github.com/<votre‑compte>/pyrat-tsp-examples.git
cd pyrat-tsp-examples
```

## Utilisation

1. Lancez Jupyter :
   ```bash
   jupyter lab
   ```
2. Ouvrez l’un des notebooks listés ci‑dessus.
3. Exécutez les cellules dans l’ordre pour reproduire les résultats.

Chaque notebook débute par une cellule d’initialisation qui :
- génère ou charge un graphe de test ;
- applique l’algorithme correspondant ;
- affiche la tournée et son coût.

## Détails des notebooks

| Notebook | Description rapide |
|----------|--------------------|
| **DFS_Pyrat.ipynb** | Implémente un DFS naïf pour explorer l’espace des solutions. Utile comme base de comparaison. |
| **Greedy_1_1.ipynb** | Voisin le plus proche : choisit à chaque étape la ville la plus proche non visitée. |
| **Greedy_4_4.ipynb** | Heuristique gloutonne groupant les villes par blocs de 4. |
| **Greedy_4_4_amelioré.ipynb** | Amélioration de Greedy 4‑4 via un remaniement local (2‑opt). |
| **TSP_Brute.ipynb** | Recherche exhaustive de toutes les permutations (réservé aux petits graphes !). |

## Contribuer

Les contributions sont les bienvenues !

1. Forkez le projet et créez votre branche (`git checkout -b feature/ma‑feature`).
2. Commitez vos modifications (`git commit -m 'Ajoute ma feature'`).
3. Poussez votre branche (`git push origin feature/ma‑feature`).
4. Ouvrez une *Pull Request*.

## Auteurs
- MARECHAL Luc
- CUZOU Alexandre

## Licence

Distribué sous licence MIT – voir le fichier `LICENSE` pour plus de détails.

---

> Projet développé dans le cadre du cours **PyRat** – Université XYZ, 2025.
