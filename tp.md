## 1. Liens entre langages finis et réguliers
1. Tout langage fini est régulier
	**Faux**

	Un langage fini n'est pas nécessairement régulier. Il est à lui seul un langage, pour qu'il soit un langage régulier il devra se construire sur d'autres langages finis.

2. Tout langage régulier est fini
	**Vrai**

	Un langage est régulier si on peut le construire à partir de langages (un ou plusieurs) eux même finis. 

	Il sera par conséquent également un langage fini s'il n'est composé que de langage finis.

3. Tout langage qu'on peut représenter par une expression régulière est fini
	**Faux**

	Ca sera un langage régulier.

4. Tout langage fini peut être représenté par une expression régulière
	**Vrai**

## 2. Reconnaitre des langages finis et réguliers

*Pour chacun des langages suivants, définis sur l'alphabet {1,0}, déterminez s'il est fini et/ou
régulier*

5. Le langage des mots d'au plus deux symboles
	**Régulier**
	
6. Le langage des mots de taille 2
	**Fini**

7. Le langage des mots qui commencent et finissent par 1
	**Régulier**

8. Le langage des nombres impaires en représentation binaire
	**Fini**

9. Le langage des nombres binaires qui ont un nombre impair de 1
	**Régulier**

10. Le langage composé des mots présents dans les oeuvres de Victor Hugo, qui auraient été codées en morse (1=-, 0= .)
	**Finis**

11. Le langage des mots d'au moins deux symboles
	**Régulier**

12. Le langage des mots de taille 3 qui commencent et finissent par le même symbole
	**Régulier**

13. Le langage des mots qui commencent et finissent par 1 et qui contiennent exactement trois 1
	**Régulier**

14. Le langage des mots qui ne contiennent aucun 0
	**Régulier**

15. Le langage des mots qui contiennent exactement deux fois chaque symbole de l'alphabet
	**Régulier**

16. Le langage des mots qui commencent et finissent par le même symbole
	**Régulier**

## 3. Automates finis

17. Donnez, pour l'automate suivant, un exemple de mot de taille 1, 2, 3, 4 et 5 qui sont reconnus. L'un de ces mots doit contenir un c. Donnez ensuite un exemple de mot non reconnu par cet automate (sur l'alphabet {a,b,c})

![](https://i.ibb.co/whq6gnS/Capture-d-cran-2020-10-26-175054.png)

1: {b}
2: {a,a}
3: {a,b,a}
4: {a,c,a,a}
5: {a,c,a,b,a}

Non reconnu: {c} ou {a} ou {c,b,b,b} etc

18.  Dessinez les automates finis qui correspondent aux langages décrits dans les exercices 7 à 9.

7
![](https://github.com/MaskedBelgian/theoriedeslangageTP/blob/main/TP1-Th%C3%A9orieLangage.jpg)

8
