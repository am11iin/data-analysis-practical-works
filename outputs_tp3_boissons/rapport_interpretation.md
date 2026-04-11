# TP3 Boissons - ACP complete

## 1. Matrice R
La matrice des correlations complete est exportee dans:
- `outputs_tp3_boissons/05_matrice_R_correlations.csv`

Les liaisons les plus fortes sont:
- Fruite / Sucre: 0.931
- Gout / Rugosite: 0.859
- Odeur / Suffocant: 0.784
- Fruite / Parfume: 0.812
- Gout / Fruite: -0.802

## 2. Valeurs propres et tableau des inerties
Les 3 premiers axes expliquent 85.88% de l'inertie totale.
- Axe 1: 50.35%
- Axe 2: 23.99%
- Axe 3: 11.54%

Le tableau complet est exporte dans:
- `outputs_tp3_boissons/06_tableau_taux_inertie.csv`

## 3. Interpretation des axes
### Axe 1
Axe 1 oppose d'un cote les boissons tres Parfume (0.930), Fruite (0.913), Sucre (0.884) et de l'autre cote les boissons marquees par Gout (-0.911), Rugosite (-0.829), Amer (-0.736).

Interpretation synthese:
- Pole positif: boissons fruitees, sucrees et parfumees.
- Pole negatif: boissons plus rugueuses, avec plus de gout et davantage d'amertume.

Boissons les plus positives sur l'axe 1:
- Boisson 4 (3.204), Boisson 7 (2.696), Boisson 3 (1.761)

Boissons les plus negatives sur l'axe 1:
- Boisson 6 (-3.338), Boisson 8 (-2.140), Boisson 5 (-1.876)

Caracterisation:
- Boisson 4, Boisson 7, Boisson 3 et Boisson 9 se ressemblent par leur profil fruite, sucre et parfume.
- Boisson 6, Boisson 8, Boisson 5 et Boisson 2 se rapprochent par un profil moins fruite et plus rude en bouche.

### Axe 2
Axe 2 est surtout porte par Odeur (38.938), Piquant (23.278), Suffocant (22.673).

Interpretation synthese:
- Pole positif: boissons a odeur forte et suffocante, avec une pointe d'amertume.
- Pole negatif: boissons plus piquantes.

Boissons les plus positives sur l'axe 2:
- Boisson 1 (1.725), Boisson 2 (1.336), Boisson 7 (0.688)

Boissons les plus negatives sur l'axe 2:
- Boisson 10 (-3.811), Boisson 9 (-0.896), Boisson 5 (-0.542)

Caracterisation:
- Boisson 10 est tres atypique sur cet axe: elle concentre a elle seule 67.24% de la construction de l'axe 2.
- Boisson 1, Boisson 2, Boisson 3 et Boisson 7 sont du cote oppose et ont un profil moins odorant/suffocant.

### Axe 3
Axe 3 est domine par Acide (66.081), Amer (13.969), Suffocant (11.560).

Interpretation synthese:
- Pole positif: boissons plutot acides.
- Pole negatif: boissons plus ameres, avec davantage de gout et moins d'acidite.

Boissons les plus positives sur l'axe 3:
- Boisson 7 (1.716), Boisson 1 (1.345), Boisson 10 (0.874)

Boissons les plus negatives sur l'axe 3:
- Boisson 4 (-1.646), Boisson 9 (-0.996), Boisson 6 (-0.990)

Caracterisation:
- Boisson 7 et Boisson 1 se rapprochent par une acidite plus marquee.
- Boisson 4, Boisson 9 et Boisson 6 partagent un pole plus amer et moins acide.

## 4. Qualites de representation et contributions
Les tableaux complets sont exportes dans:
- `outputs_tp3_boissons/09_cos2_individus.csv`
- `outputs_tp3_boissons/10_contributions_individus.csv`
- `outputs_tp3_boissons/12_cos2_variables.csv`
- `outputs_tp3_boissons/13_contributions_variables.csv`

Individus tres bien representes sur les 3 premiers axes:
- Boisson 10: somme cos2 = 0.977
- Boisson 4: somme cos2 = 0.969
- Boisson 7: somme cos2 = 0.930

Variables tres bien representees sur les 3 premiers axes:
- Acide: somme cos2 = 0.888
- Amer: somme cos2 = 0.889
- Odeur: somme cos2 = 0.954

## 5. Nouvelles variables et representation dans le nouveau plan
Les nouvelles variables sont les composantes principales F1, F2, ..., F10.
Elles sont orthogonales entre elles et resumees par:
- F1: dimension fruit-sucre-parfum opposee au gout-rugosite-amertume.
- F2: dimension odeur/suffocant opposee au piquant.
- F3: dimension acidite opposee a l'amertume.

La representation des variables dans les nouveaux plans se lit dans:
- `outputs_tp3_boissons/11_coordonnees_variables.csv`
- `outputs_tp3_boissons/cercle_correlation_1_2.png`
- `outputs_tp3_boissons/cercle_correlation_1_3.png`
- `outputs_tp3_boissons/cercle_correlation_2_3.png`

## 6. Conclusion sur les boissons
On peut distinguer 4 profils principaux:
- Groupe fruite/sucre/parfume: Boissons 4, 7, 3, 9.
- Groupe plus rude et moins fruite: Boissons 6, 8, 5, 2.
- Profil tres odorant et suffocant: Boisson 10.
- Profil intermediaire mais acide: Boisson 1.

Les points communs les plus nets entre boissons sont donc:
- Boissons 4 et 7: tres proches du pole fruit-sucre-parfum.
- Boissons 6 et 8: proches du pole oppose, moins fruitees et plus neutres olfactivement.
- Boissons 1 et 7: proximite sur l'acidite.
- Boisson 10 reste la plus singuliere a cause de l'odeur et du caractere suffocant.
