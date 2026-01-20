# Élements de corrections

## Séance 2.

### Questions

- **Question 3.** Vous êtes trop précis.

- **Question 7.** Vous écrivez une liste de méthode. Vous ne les catégorisez pas.

- **Question 11.** La distribution statistique est la projection des fréquences observées par classe.

### Code

- Excellent !

## Séance 3.

### Questions

- **Question 1.** Le caractère qualitatif est le plus général.

- **Question 5.** Vous n'avez pas compris ce qu'était une variance et un écart type.

### Code

- Excellent !

## Séance 4

### Questions

- Pas assez précis.

### Code

- Excellent !

## Séance 5

### Questions

- Trop superficiel !

### Code

- Où est le commentaire demandé dans votre rapport ?

- Il y a un problème d'appel de la bibliothèque :

```
    stat1, p1 = stats.shapiro(test1['Test'])
    stat2, p2 = stats.shapiro(test2['Test'])
```

Il faut écrire :

```
    stat1, p1 = scipy.stats.shapiro(test1['Test'])
    stat2, p2 = scipy.stats.shapiro(test2['Test'])
```

## Séance 6

### Questions

- Trop superficiel !

### Code

- Où est le commentaire demandé dans votre rapport ?

- Problème d'encodage !

- Il y a un problème d'appel de la même bibliothèque.

- Le code suivant est faux :

```
    rho, p_spearman = scipy.stats.spearmanr(rangs_pop, rangs_dens)
    tau, p_kendall = scipy.stats.kendalltau(rangs_pop, rangs_dens)
```

Il fallait écrire :


- Le code suivant est faux :

```
    rho_pop, p_spearman_pop = scipy.stats.spearmanr(rangs_pop_2007, rangs_pop_2025)
    tau_pop, p_kendall_pop = scipy.stats.kendalltau(rangs_pop_2007, rangs_pop_2025)

    rho_dens, p_spearman_dens = scipy.stats.spearmanr(rangs_dens_2007, rangs_dens_2025)
    tau_dens, p_kendall_dens = scipy.stats.kendalltau(rangs_dens_2007, rangs_dens_2025)
```

Il fallait comparer une même variable à deux années différentes.

## Humanités numériques

- Aucun rendu.

## Remarques générales

- Aucun dépôt régulier sur `GitHub`.

- Il fallait rédiger le rapport. L'ensemble de vos réponses est trop décousu.

- Attention ! Il ne faut jamais utiliser l'adresse absolue `C:/Users/HP/Desktop/Cours M1/Python/src/data/resultats-elections-presidentielles-2022-1er-tour.csv"`, mais l'adresse relative `./data/resultats-elections-presidentielles-2022-1er-tour.csv"`.
