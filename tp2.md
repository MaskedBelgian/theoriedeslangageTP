## 1. Liens entre langages réguliers, finis et hors-contexte
1. *Tout langage régulier est hors-contexte*

**Vrai**

Une grammaire hors contexte est plus puissante qu'un langage régulier.

2. *Tout langage hors-contexte est régulier*

**Faux**

Les langages hors-contexte comprennent les langages réguliers.

![](https://www.gaudry.be/img/language/chomsky.gif)

3. *Tout langage fini est hors-contexte*

**Vrai**

4. *Tout langage hors-contexte est fini*

**Faux**

5. *Toute expression régulière est exprimable sous la forme d'une grammaire horscontexte*

**Vrai**

6. *Toute grammaire hors-contexte est exprimable sous la forme d'une expression régulière*

**Faux**

7. *Pour prouver qu'un langage est hors-contexte, il sufit de trouver une grammaire
hors-contexte qui le représente*

**Vrai**

Comme pour un LR, il suffit de pouvoir l'exprimer sous forme d'une grammaire hors-contexte, il sera alors un langage hors-contexte.

8. *Tout sous-langage d'un langage régulier est régulier*

**Vrai**

9. *Comment prouver qu'un langage n'est pas régulier ?*

Voir Lemme de pompage

10. *Comment prouver qu'un langage n'est pas hors contexte ?*

Voir Lemme de pompage


## 2. Langages hors-contexte

11. *Le langage des mots qui contiennent autant de a que de b et aucun c*

![](https://i.ibb.co/CQS04L6/Capture-d-cran-2020-11-03-185620.png)

12. *Le langage des mots de la forme a^n c^n c^n(n ≥ 0)*

S -> E | aScc

13. *Le langage des mots de la forme a
nban(n ≥ 0)*

S -> b | aSa

14. *Le langage des mots de la forme a^n b^m(n > m ≥ 0)

S -> a | aSb | aS

15. *Le langage des palindromes (mots qui peuvent se lire de gauche à droite ou de
droite à gauche)*

S -> E | a | b | c | aSa | bSb | cSc

16. *Le langage des mots de la forme c(a|b)^n c(a|b)^n c*

