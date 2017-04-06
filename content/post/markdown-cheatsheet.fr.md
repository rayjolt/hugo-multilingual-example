+++
date = "2017-03-30T20:04:17"
title = "Markdown Cheatsheet"
tags = ["démarques", "exemples", "antisèche"]
categories = ["exemples"]
slug = "markdown-cheatsheet"
draft = false

+++

Le cheatsheet suivant est extrait de <https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet>, par [Adam Pritchard](https://github.com/adam-p).

---

## Têtes

```no-highlight
# H1
## H2
### H3
#### H4
##### H5
###### H6

Sinon, pour H1 et H2, un style underline-ish:

Alt-H1
======

Alt-H2
------
```

# H1
## H2
### H3
#### H4
##### H5
###### H6

Sinon, pour H1 et H2, un style underline-ish:

Alt-H1
======

Alt-H2
------

## L'accent

```no-highlight
L'accent, alias italique, avec *astérisques* ou _underscores_.

L'accent, alias gras, avec des **astérisques** ou __underscores__.

Combiné avec l'accent astérisques **et _underscores_**.

Biffés utilise ~~deux tildes~~.
```

L'accent, alias italique, avec *astérisques* ou _underscores_.

L'accent, alias gras, avec des **astérisques** ou __underscores__.

Combiné avec l'accent astérisques **et _underscores_**.

Biffés utilise ~~deux tildes~~.


## Listes

(Dans cet exemple, les espaces de fin sont représentés avec des points: ⋅)

```no-highlight
1. Premier élément de liste ordonnée
2. Un autre élément
⋅⋅ * sous-liste non ordonnée.
1. Les chiffres réels ne sont pas importants, juste que c'est un certain nombre
⋅⋅1. Sous-liste ordonnée
4. Et un autre élément.

⋅⋅⋅You peut avoir correctement indenté les paragraphes dans les éléments de liste. Notez la ligne vide au-dessus, et les espaces principaux (au moins un, mais nous allons utiliser trois ici pour aligner également la première Markdown).

⋅⋅⋅To ont un saut de ligne sans paragraphe, vous devez utiliser deux spaces.⋅⋅ arrière
⋅⋅⋅Note que cette ligne est distincte, mais dans le même paragraph.⋅⋅
⋅⋅⋅ (ce qui est contraire au comportement de saut de ligne GFM typique, où les espaces de fin ne sont pas nécessaires.)

* Liste non ordonnée peut utiliser des astérisques
- Ou inconvénients
+ Ou points positifs
```

1. Premier élément de liste ordonnée
2. Un autre élément
  * Sous-liste non ordonnée.
1. Les chiffres réels ne sont pas importants, juste que c'est un certain nombre
  1. sous-liste ordonnée
4. Et un autre élément.

   Vous pouvez avoir correctement indenté les paragraphes dans les éléments de liste. Notez la ligne vide au-dessus, et les espaces principaux (au moins un, mais nous allons utiliser trois ici pour aligner également la première Markdown).

   Avoir un saut de ligne sans paragraphe, vous devez utiliser deux espaces de fin.
   Notez que cette ligne est distincte, mais dans le même paragraphe.
   (Ce qui est contraire au comportement de saut de ligne GFM typique, où les espaces de fin ne sont pas nécessaires.)

* Liste non ordonnée peut utiliser des astérisques
- Ou inconvénients
+ Ou points positifs

## Liens

Il y a deux façons de créer des liens.

```no-highlight
[Je suis un lien de style en ligne](https://www.google.com)

[Je suis un lien de style en ligne avec le titre](https://www.google.com « page d'accueil de Google »)

[Je suis un lien de style de référence][texte de référence insensible à la casse arbitraire]

[Je suis une référence par rapport à un fichier de dépôt](../ blob / master / licence)

[Vous pouvez utiliser des numéros pour les définitions de lien de style de référence][1]

Ou le laisser vide et utiliser le [texte du lien lui-même].

URL et les URL entre crochets sera automatiquement transformés en liens.
http://www.example.com ou <http://www.example.com> et parfois
example.com (mais pas sur Github, par exemple).

Une partie du texte pour montrer que les liens de référence peuvent suivre plus tard.

[texte de référence insensible à la casse arbitraire]: https://www.mozilla.org
[1]: http://slashdot.org
[texte du lien lui-même]: http://www.reddit.com
```

[Je suis un lien de style en ligne](https://www.google.com)

[Je suis un lien de style en ligne avec le titre](https://www.google.com « page d'accueil de Google »)

[Je suis un lien de style de référence][texte de référence insensible à la casse arbitraire]

[Je suis une référence par rapport à un fichier de dépôt](../ blob / master / licence)

[Vous pouvez utiliser des numéros pour les définitions de lien de style de référence][1]

Ou le laisser vide et utiliser le [texte du lien lui-même].

URL et les URL entre crochets sera automatiquement transformés en liens.
http://www.example.com ou <http://www.example.com> et parfois
example.com (mais pas sur Github, par exemple).

Une partie du texte pour montrer que les liens de référence peuvent suivre plus tard.

[texte de référence insensible à la casse arbitraire]: https://www.mozilla.org
[1]: http://slashdot.org
[texte du lien lui-même]: http://www.reddit.com

## Images

```no-highlight
Voici notre logo (vol stationnaire pour voir le texte du titre):

De style en ligne:
![Texte Alt](https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png "Titre Texte du logo 1")

Style de référence:
![Texte Alt][logo]

[logo]: https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png "Logo Titre Texte 2"
```

Voici notre logo (vol stationnaire pour voir le texte du titre):

De style en ligne:
![Texte Alt](https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png "Titre Texte du logo 1")

Style de référence:
![Texte Alt][logo]

[logo]: https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png "Logo Titre Texte 2"

## Code et la coloration syntaxique

Les blocs de code font partie de la spécification Markdown, mais la mise en évidence de la syntaxe n'est pas cependant, de nombreux équarrisseurs - comme de Github et *Markdown Here* - mise en évidence de la syntaxe. Soutenir les langues supportées et comment ces noms linguistiques doivent être rédigés variera. générateur de renderer *Markdown Here* prend en charge mettant en lumière des dizaines de langues (et non-vraiment-langues, comme les diffs et les en-têtes HTTP) pour voir la liste complète, et la façon d'écrire les noms de langue, consultez le [highlight.js démo page](http://softwaremaniacs.org/media/soft/highlight/test.html).

```no-highlight
Inline `code` back-recueil HSC `tiques` around il.
```

Inline `code` back-recueil HSC `tiques` around il.

Les blocs de code sont soit clôturées par des lignes avec trois arrière-tiques <code>```</code>, ou sont en retrait avec quatre espaces que je recommande en utilisant uniquement les blocs de code clôturé - Ils sont plus faciles et seulement ils soutiennent la syntaxe mise en évidence.

<pre lang = "no-highlight"><code>```javascript
var = "syntaxe JavaScript de mise en évidence";
alerte (s);
```
 
```python
s = "syntaxe Python mise en évidence"
print s
```
 
```
Aucune langue indiquée, donc pas la coloration syntaxique.
Mais nous allons jeter dans un &lt;b&gt;&lt;/b&gt;.
```
</code> </pre>

```javascript
var = "syntaxe JavaScript de mise en évidence";
alerte (s);
```
 
```python
s = "syntaxe Python mise en évidence"
print s
```
 
```
Aucune langue indiquée, donc pas la coloration syntaxique.
Mais nous allons jeter dans un &lt;b&gt;&lt;/b&gt;.
```

## Tableaux

Les tableaux ne font pas partie de la spécification Markdown de base, mais ils font partie de GFM et * Markdown ici * les soutient Ils sont un moyen facile d'ajouter des tables à votre e-mail -. Une tâche qui nécessiteraient du copier-coller d'une autre application .

```no-highlight
Colons peuvent être utilisés pour aligner les colonnes.

| Tables | Y | cool |
| ------------- | -------------: | -----: |
| Col 3 est | aligné à droite | 1600 $ |
| Col 2 est | centré | $ 12 |
| Zébrures | sont propres | $ 1 |

Il doit y avoir au moins 3 tirets séparant chaque cellule d'en-tête.
Les tubes extérieurs (|) sont facultatifs, et vous n'avez pas besoin de faire la
ligne Markdown cru jusqu'à joli. Vous pouvez également utiliser Markdown en ligne.

Markdown | Moins | Jolie
--- | --- | ---
*Toujours* | `renders` | **bien**
1 | 2 | 3
```

Colons peuvent être utilisés pour aligner les colonnes.

| Tables | Y | cool |
| ------------- | -------------: | -----: |
| Col 3 est | aligné à droite | 1600 $ |
| Col 2 est | centré | $ 12 |
| Zébrures | sont propres | $ 1 |

Il doit y avoir au moins 3 tirets séparant chaque cellule en-tête Les tubes extérieurs (|). Sont facultatifs, et vous n'avez pas besoin de faire la ligne Markdown brute jusqu'à Vous pouvez également joliment utiliser Markdown en ligne.

Markdown | Moins | Jolie
--- | --- | ---
*Toujours* | `renders` | **bien**
1 | 2 | 3

## Blocs de Texte

```no-highlight
> Sont très pratiques citations en blocs dans le courrier électronique pour émuler texte de réponse.
> Cette ligne fait partie de la même citation.

Citation briser.

> Ceci est une très longue ligne qui va encore être cité correctement quand il enveloppe. Oh boy, nous allons continuer à écrire pour faire assez sûr que ce soit longtemps pour envelopper vraiment pour tout le monde. Oh, vous pouvez * mettre * ** ** Markdown dans un blockquote .
```

> Sont très pratiques citations en blocs dans le courrier électronique pour émuler texte de réponse.
> Cette ligne fait partie de la même citation.

Citation briser.

> Ceci est une très longue ligne qui va encore être cité correctement quand il enveloppe. Oh boy, nous allons continuer à écrire pour faire assez sûr que ce soit longtemps pour envelopper vraiment pour tout le monde. Oh, vous pouvez * mettre * ** ** Markdown dans un blockquote .

## Inline HTML

Vous pouvez également utiliser HTML brut dans votre Markdown, et il va la plupart du temps assez bien.

```no-highlight
<dl>
  <dt>Liste de définitions</dt>
  <dd>Est-ce quelque chose de gens utilisent parfois.</dd>
  
  <dt>Markdown en HTML</dt>
  <dd>ne *pas* travail **très** bien. Utilisez HTML <em>balises</ em>.</dd>
</dl>
```

<dl>
  <dt>Liste de définitions</dt>
  <dd>Est-ce quelque chose de gens utilisent parfois.</dd>
  
  <dt>Markdown en HTML</dt>
  <dd>ne *pas* travail **très** bien. Utilisez HTML <em>balises</em>.</dd>
</dl>

## Règle horizontale

```
Trois ou plus ...

---

Les traits d'union

***

Asterisks

___

underscores
```

Trois ou plus ...

---

Les traits d'union

***

Asterisks

___

underscores

## Sauts de ligne

Ma recommandation de base pour apprendre retour à la ligne est d'expérimenter et de découvrir - Hit &lt;Entrée&gt; une fois (c.-à insérer un saut de ligne), puis appuyez deux fois (c.-à-insérer deux nouvelles lignes), voir ce qui se passe, vous allez bientôt apprendre à obtenir ce que vous voulez. «Markdown Toggle» est votre ami.

Voici quelques choses à essayer:

```no-highlight
Voici une ligne pour nous de commencer.

Cette ligne est séparée de celle ci-dessus par deux nouvelles lignes, donc ce sera un *paragraphe distinct*.

Cette ligne est également un paragraphe séparé, mais ...
Cette ligne est séparée par un seul saut de ligne, il est donc une ligne distincte dans le *même paragraphe*.
```

Voici une ligne pour nous de commencer.

Cette ligne est séparée de celle ci-dessus par deux nouvelles lignes, donc ce sera un *paragraphe distinct*.

Cette ligne est également un paragraphe séparé, mais ...
Cette ligne est séparée par un seul saut de ligne, il est donc une ligne distincte dans le *même paragraphe*.

---

- Droit d'auteur: [Adam Pritchard](https://github.com/adam-p)
- Licence: [CC-BY](https://creativecommons.org/licenses/by/3.0/)