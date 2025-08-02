# Bibliothèque de Recherche et Tri en C

Ce projet propose une bibliothèque en langage C pour effectuer différentes opérations de recherche et de tri sur des tableaux d'entiers.

## Fichiers
- `recherche.c` / `recherche.h` : Fonctions de recherche (linéaire, binaire, interpolée, par saut)
- `tri.c` / `tri.h` : Fonctions de tri (à compléter selon vos besoins)

## Fonctions de recherche
- **Recherche linéaire** : Parcourt le tableau pour trouver la valeur cible.
- **Recherche binaire** : Recherche efficace dans un tableau trié.
- **Recherche interpolée** : Variante de la recherche binaire, adaptée aux tableaux uniformément répartis.
- **Recherche par saut (Jump Search)** : Recherche par blocs dans un tableau trié.

## Utilisation
Inclure les fichiers d'en-tête dans votre projet :
```c
#include "recherche.h"
#include "tri.h"
```

Compiler avec :
```sh
gcc recherche.c tri.c -o mon_programme -lm
```

## Exemple
```c
int tab[] = {1, 3, 5, 7, 9};
int n = 5;
int index = rechercheBinaire(tab, n, 7);
if(index != -1) {
    printf("Trouvé à l'indice %d\n", index);
} else {
    printf("Non trouvé\n");
}
```

## Auteur
Mendrika Randriamora

## Licence
Ce projet est open source, libre d'utilisation et de modification.
