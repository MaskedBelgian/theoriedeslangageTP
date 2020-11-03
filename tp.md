## 1. Liens entre langages finis et réguliers
1. *Tout langage fini est régulier*
	**Vrai**

	Tout langage fini est régulier. On pourra tjrs faire l'union de 2 langages réguliers et ça donnera un langage régulier. On pourra regex un langage fini.

2. *Tout langage régulier est fini*
	**Faux**

	L'étoile de Kleene rend la chose impossible.

3. *Tout langage qu'on peut représenter par une expression régulière est fini*
	**Faux**

	Idem que 2.

4. *Tout langage fini peut être représenté par une expression régulière*
	**Vrai**
	
	Voir 1.

## 2. Reconnaitre des langages finis et réguliers

*Pour chacun des langages suivants, définis sur l'alphabet {1,0}, déterminez s'il est fini et/ou
régulier*

5. *Le langage des mots d'au plus deux symboles*

	**Fini** car {€,0,1,01,10,00,11} et **Régulier** €|0|1|01|10|00|11
	
6. *Le langage des mots de taille 2*

	**Fini** car {01,10,00,11} et **Régulier** 01|10|00|11 ou (0|1).(0|1)

7. *Le langage des mots qui commencent et finissent par 1*

	**Régulier** car 1.(0|1)*.1 et donc pas fini à cause de l'étoile de Kleene

8. *Le langage des nombres impaires en représentation binaire*

	**Régulier** car (0|1)*.1

9. *Le langage des nombres binaires qui ont un nombre impair de 1*

	**Irrégulier** car {1,101,1011,10101,...} on ne peut pas "retenir" de mot et on ne peut pas le représenter en format régulier

10. *Le langage composé des mots présents dans les oeuvres de Victor Hugo, qui auraient été codées en morse (1=-, 0= .)*

	**Finis** car on peut prendre tous les mots de ses livres, les encoder et faire l'union 

11. *Le langage des mots d'au moins deux symboles*

	**Régulier** car (0|1).(0|1).(0|1).*

12. *Le langage des mots de taille 3 qui commencent et finissent par le même symbole*

	**Finis** car {101,010,111,000} et **Régulier** car 1.(0|1).1 | 0.(0|1).0

13. *Le langage des mots qui commencent et finissent par 1 et qui contiennent exactement trois 1*

	**Régulier** 1.0*.1.0*.1

14. *Le langage des mots qui ne contiennent aucun 0*

	**Régulier** car 1.*

15. *Le langage des mots qui contiennent exactement deux fois chaque symbole de l'alphabet*

	**Finis** car {1100,1010,0011,0101,0110,1001}

16. *Le langage des mots qui commencent et finissent par le même symbole*

	**Régulier** car 0 | 1 | ( 1.(0 | 1)\*.1) | ( 0.( 0 | 1 )*.0 )
	
![](https://github.com/MaskedBelgian/theoriedeslangageTP/blob/main/Capture%20d%E2%80%99%C3%A9cran%202020-10-27%20195951.png)

## 3. Automates finis

17. *Donnez, pour l'automate suivant, un exemple de mot de taille 1, 2, 3, 4 et 5 qui sont reconnus. L'un de ces mots doit contenir un c. Donnez ensuite un exemple de mot non reconnu par cet automate (sur l'alphabet {a,b,c})*

![](https://i.ibb.co/whq6gnS/Capture-d-cran-2020-10-26-175054.png)

1: {b}
2: {a,a}
3: {a,b,a}
4: {a,c,a,a}
5: {a,c,a,b,a}

Non reconnu: {c} ou {a} ou {c,b,b,b} etc

18.  *Dessinez les automates finis qui correspondent aux langages décrits dans les exercices 7 à 9*

7 et 8:

![](https://github.com/MaskedBelgian/theoriedeslangageTP/blob/main/TP1-Th%C3%A9orieLangage.jpg)

9:

![](https://github.com/MaskedBelgian/theoriedeslangageTP/blob/main/TP1-Th%C3%A9orieLangage2.jpg)

19. *Utilisez explicitement les règles de traduction d'automate fini à expression régulière pour traduire l'expression régulière de l'exercice 16 en automate fini*

## 4. Complément d'un langage régulier

20. *Pour l'automate fini de l'exercice 17, déterminez l'expression régulière qui lui est équivalente*

		(ab*c)*(b|ab*a)

21.  *Le complément d'un langage régulier est-il toujours régulier ? Prouvez votre réponse*

22. *Déterminez le complément des langages définis aux exercices 7 à 9*

23. *Déterminez l'expression régulière représentant le complément du langage reconnu par l'automate fini suivant. Pour ce faire, déterminisez-le, minimisez-le, complétez-le, inversez les états finaux et non finaux et transformez-le en expression régulière*

![](https://i.ibb.co/syYdWTd/Capture-d-cran-2020-10-26-183623.png)
