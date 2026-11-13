# Script oral : « L'intelligence artificielle à la rencontre du cerveau humain »

IndabaX Guinée 2026 (13 novembre 2026) — Boubacar Sow

Conventions :
- **[clic]** = passer à l'étape suivante de la slide (une animation).
- Le numéro de slide est celui affiché en bas à droite.
- Le texte est écrit pour être dit, pas lu mot à mot : garde les idées, reformule avec tes mots.

---

## Page de titre

Bonjour à toutes et à tous. Merci aux organisateurs d'IndabaX Guinée de m'avoir invité.

Je m'appelle Boubacar Sow. Aujourd'hui, je vais vous parler de la rencontre entre l'intelligence artificielle et le cerveau humain, et plus précisément de ce que l'IA nous apprend sur le langage, la mémoire et la pensée.

Si vous voulez les slides, le QR code en haut à droite permet de les télécharger. Il sera aussi sur la dernière slide.

---

## Slide 1 — Mon parcours : de Conakry à Paris

Avant d'entrer dans le sujet, quelques mots sur mon parcours, parce que tout a commencé ici, à Conakry.

J'ai eu mon bac en sciences mathématiques en 2019, à l'Institution Sainte-Marie de Dixinn. Je suis ensuite parti faire une licence d'informatique entre l'Université de Bretagne Occidentale, à Brest, et l'Université du Québec à Rimouski, au Canada.

Après, je me suis spécialisé : un master 1 en data science à l'Université Paris-Saclay, puis le master MVA, « Mathématiques, Vision, Apprentissage », à l'ENS Paris-Saclay. C'est l'un des masters de référence en apprentissage automatique en France.

J'ai ensuite été ingénieur de recherche à l'Institut Pasteur. Depuis mai 2026, je suis doctorant au Laboratoire de Sciences Cognitives et Psycholinguistique, à l'École normale supérieure, à Paris.

Mon sujet de thèse, c'est justement ce dont je vais vous parler : utiliser les modèles d'IA pour comprendre comment le cerveau humain traite le langage.

---

## Slide 2 — L'IA, ce n'est pas que ChatGPT

Quand on dit « intelligence artificielle » aujourd'hui, presque tout le monde pense à ChatGPT. Mais l'IA, c'est beaucoup plus large que les chatbots. C'est aussi devenu un instrument scientifique.

En biologie, par exemple, AlphaFold prédit la forme en trois dimensions des protéines à partir de leur séquence. Ce travail a reçu le prix Nobel de chimie en 2024.

**[clic]** En médecine, un réseau de neurones a permis à une patiente qui ne pouvait plus parler de communiquer à nouveau : il transforme son activité cérébrale en texte à l'écran. On y reviendra à la fin.

**[clic]** Et en neurosciences, ce qui nous intéresse aujourd'hui : les réseaux de neurones artificiels servent de modèles du cerveau. Ce sont des hypothèses que l'on peut tester.

**[clic]** Une image que j'aime bien : le télescope a transformé l'astronomie. L'IA est en train de devenir un outil du même genre pour étudier le cerveau.

---

## Slide 3 — Pourquoi un modèle aide à comprendre

Pourquoi un modèle d'IA nous aiderait-il à comprendre le cerveau ?

Le problème de départ est simple : le cerveau humain contient environ 86 milliards de neurones. Il est impossible de les enregistrer tous chez une personne vivante. On n'a qu'un accès très limité à ce qui se passe à l'intérieur.

**[clic]** Un modèle, lui, est entièrement accessible : chaque unité peut être mesurée et modifiée. Attention, ça ne veut pas dire qu'il est facile à comprendre. Le comprendre reste un vrai travail de recherche. Mais au moins, on a accès à tout. L'idée est alors de donner la même phrase aux deux systèmes, par exemple « Le chat dort », et de comparer leurs réponses.

**[clic]** Si le modèle se comporte comme le cerveau, il devient une hypothèse explicite sur la façon dont le cerveau calcule.

**[clic]** Autrement dit, un modèle d'IA, c'est une théorie qu'on peut faire tourner, interroger, et même casser pour voir ce qui se passe.

---

## Slide 4 — Le fil de l'exposé

Voici la question qui va nous guider : que nous apprend la comparaison entre un modèle d'IA et le cerveau humain ?

L'exposé a cinq étapes :
1. d'abord les bases, les deux systèmes qui traitent le langage ;
2. ensuite, comment on les compare ;
3. puis on ouvre la boîte, pour regarder les mécanismes : langage, pensée, mémoire ;
4. je vous présenterai mon propre travail ;
5. et on finira par une application concrète : décoder le langage à partir du cerveau.

---

## Partie 1 — Deux systèmes qui traitent le langage

Commençons par les deux systèmes : le modèle de langage d'un côté, le cerveau de l'autre.

---

## Slide 5 — Un modèle de langage : prédire le mot suivant

Regardez cette phrase : « Au marché de Madina, j'ai acheté du… ». Qu'est-ce qui vient après, à votre avis ?

*(Laisser le public répondre.)*

**[clic]** Un modèle de langage fait exactement ce que vous venez de faire : il donne une probabilité à chaque mot possible. Ici, « riz » est très probable, « poisson » aussi, « pain »… et « voiture » presque impossible.

**[clic]** Et c'est tout ce qu'il apprend à faire : prédire le mot suivant, sur des milliards de phrases.

**[clic]** Mais pour bien prédire, il est obligé de capter beaucoup de choses : la grammaire, le sens des mots, le contexte. Pour savoir qu'on achète du riz au marché, il faut savoir ce qu'est un marché.

**[clic]** ChatGPT, c'est ce même principe, avec ensuite un ajustement pour qu'il dialogue avec nous. Et le point important : aucune règle de grammaire n'est programmée à la main. Tout est appris à partir des données.

---

## Slide 6 — À l'intérieur du modèle : des vecteurs de nombres

Que se passe-t-il à l'intérieur du modèle ? On donne une phrase : « Le chat dort sur le lit ».

**[clic]** Chaque mot traverse une succession de couches de neurones artificiels.

**[clic]** À chaque couche, le mot est représenté par un vecteur, une liste d'environ mille nombres, qui dépend du contexte. Le mot « lit » n'a pas la même représentation dans « dort sur le lit » et dans « il lit un livre ».

**[clic]** Ces vecteurs sont les représentations internes du modèle. C'est eux que l'on va comparer à l'activité du cerveau.

---

## Slide 7 — Un deuxième signal : la surprise

Le modèle nous donne un deuxième signal, très simple : la surprise. C'est cette formule : moins un mot est probable, plus il est surprenant. Avec notre exemple, « riz » a une probabilité de 0,41, donc une surprise faible, 1,3 bit. « Voiture » a une probabilité de 0,001, donc une surprise forte, 10 bits.

**[clic]** Donc : mot attendu, surprise faible ; mot inattendu, surprise forte.

**[clic]** Et chez l'humain ? Un mot inattendu est en moyenne lu plus lentement. Et en EEG, il produit souvent une onde cérébrale plus marquée, environ 400 millisecondes après le mot : on l'appelle la N400.

**[clic]** Le modèle nous donne donc une prédiction chiffrée, mot par mot, de la difficulté de lecture. On a deux ponts entre l'IA et le cerveau : les représentations internes, et la surprise.

---

## Slide 8 — Pourquoi étudier le langage ? Pour soigner

Voilà pour le côté IA. Avant de passer au cerveau, une question : pourquoi s'intéresser au langage dans le cerveau ? Il y a beaucoup de raisons ; je vais en retenir une : soigner.

Après un accident vasculaire cérébral, un AVC, environ un patient sur trois perd une partie de sa capacité à parler ou à comprendre. C'est ce qu'on appelle l'aphasie.

Comprendre comment le cerveau traite le langage permet :
**[clic]** de mieux diagnostiquer ce qui est atteint,
**[clic]** de mieux rééduquer,
**[clic]** et même, on le verra à la fin, de redonner la parole.

**[clic]** Pour réparer un système, il faut d'abord comprendre comment il fonctionne.

Alors, que sait-on du langage dans le cerveau ?

---

## Slide 9 — Côté humain : le réseau du langage

Voici d'abord quelques repères anatomiques : les gyres, les « plis » du cortex, dans le lobe frontal et le lobe temporal. Le langage s'appuie sur des régions frontales et temporales, surtout dans l'hémisphère gauche.

**[clic]** En rouge, schématiquement, ce qu'on appelle le réseau du langage.

**[clic]** Ce réseau répond au langage écrit comme parlé. Une étude l'a retrouvé dans les 45 langues testées. Et il répond peu au calcul ou à la musique : on y reviendra quand on parlera de la pensée.

**[clic]** C'est l'activité de ce réseau, pendant que les gens lisent ou écoutent, que l'on va chercher à prédire avec nos modèles.

---

## Slide 10 — Mesurer le cerveau qui comprend

Comment mesure-t-on cette activité ? Il existe plusieurs techniques :
- l'**IRMf** mesure le flux sanguin. Elle est précise dans l'espace, au millimètre, mais lente ;
- la **MEG** mesure les champs magnétiques produits par les neurones, à la milliseconde près ;
- l'**EEG** mesure les potentiels électriques sur le crâne. Elle est peu coûteuse et portable ;
- les **électrodes intracrâniennes** sont placées directement sur le cortex, chez des patients opérés, par exemple pour l'épilepsie.

**[clic]** Aucune méthode ne voit tout. On combine des mesures précises dans l'espace et d'autres précises dans le temps.

---

## Slide 11 — Mesurer le comportement : le temps de lecture

On peut aussi mesurer le comportement, sans regarder le cerveau : par exemple le temps qu'on met à lire chaque mot. Soit le lecteur appuie sur une touche pour faire apparaître chaque mot, soit une caméra suit le regard.

Prenons la phrase : « Les clés que l'homme tient sont sur la table ».

**[clic]** Voici des temps de lecture typiques, mot par mot. Vous voyez qu'un mot se détache : « sont ».

**[clic]** Pourquoi ? Parce que pour lire « sont », il faut retrouver son sujet, « clés », qui est loin en arrière. Gardez cet exemple en tête, on va beaucoup en reparler.

---

## Partie 2 — Comparer le modèle au cerveau

On a nos deux systèmes. Maintenant : comment les comparer, et qu'est-ce que la comparaison nous apprend ?

---

## Slide 12 — Trois niveaux pour décrire un système qui calcule

Pour réfléchir à cette question, on utilise un cadre proposé par David Marr en 1982. Il distingue trois niveaux pour décrire un système qui calcule.

Le niveau **computationnel** : quel problème est résolu ? Par exemple, additionner deux nombres.

**[clic]** Le niveau **algorithmique** : avec quelle procédure ? On peut additionner avec les chiffres arabes et la retenue, ou en comptant des bâtonnets.

**[clic]** Le niveau de l'**implémentation** : sur quel support physique ? Des neurones, des transistors, un boulier.

**[clic]** Un même problème peut être résolu par plusieurs algorithmes, et un même algorithme peut tourner sur plusieurs supports.

---

## Slide 13 — Humains et modèles : même algorithme ?

Appliquons cela au langage. Le modèle et le cerveau résolvent le même problème : comprendre et prédire la suite d'une phrase. Le support est clairement différent : des neurones d'un côté, des puces de l'autre.

Premier scénario : la **divergence**. Ils utilisent des procédures différentes. Dans ce cas, le modèle ne nous apprend rien sur le cerveau.

**[clic]** Deuxième scénario : la **convergence**. Malgré des supports différents, ils arrivent à une même procédure. Là, le modèle devient une loupe sur le cerveau.

**[clic]** Le problème, c'est qu'on ne voit pas l'algorithme directement. On l'infère en comparant leurs réponses, mot par mot.

---

## Slide 14 — La méthode : prédire le cerveau à partir du modèle

Concrètement, voici comment on compare. On prend une même histoire. On la fait lire ou écouter à des personnes, pendant qu'on enregistre leur cerveau ou leur lecture. On la donne aussi au modèle, dont on extrait les représentations et la surprise. Puis on apprend une correspondance, une régression, entre les deux.

**[clic]** Le point clé : on apprend cette correspondance sur une partie de l'histoire, puis on prédit la suite, que le système n'a jamais vue. C'est un vrai test de prédiction.

**[clic]** Et comme les mesures du cerveau sont bruitées, on compare le score à un plafond : ce qu'un autre humain prédit du même signal. Si le modèle est proche de ce plafond, il fait presque aussi bien que possible.

---

## Slide 15 — Ce que l'on sait, ce que l'on ne sait pas

Où en est-on aujourd'hui ? Ce que l'on sait :
- les modèles de langage prédisent une partie de l'activité du réseau du langage ;
- en général, mieux un modèle prédit le mot suivant, mieux il prédit le cerveau ;
- et la surprise du modèle prédit en partie les temps de lecture.

**[clic]** Ce que l'on ne sait pas :
- si le modèle utilise le même algorithme que le cerveau ;
- pourquoi les plus grands modèles ne sont pas toujours plus « humains » ;
- et ce qui vaut hors de l'anglais, puisque presque toutes les données sont en anglais.

**[clic]** Prédire n'est pas expliquer. Pour passer de la corrélation au mécanisme, il faut ouvrir la boîte.

---

## Partie 3 — Ouvrir la boîte : langage, pensée, mémoire

C'est ce qu'on va faire maintenant : ouvrir la boîte. Le langage a plusieurs niveaux, des sons jusqu'au récit ; je vais me concentrer sur un seul : la structure de la phrase.

---

## Slide 16 — Un cas d'étude : l'accord sujet-verbe

Notre cas d'étude, c'est l'accord entre le sujet et le verbe. Reprenons la phrase de tout à l'heure, en un peu plus long : « Les clés que l'homme près de l'armoire tient sont… ».

**[clic]** Le verbe « sont » s'accorde avec « clés », au pluriel. Pas avec le mot le plus proche.

**[clic]** Et il y a un piège : « l'armoire », au singulier, juste avant le verbe. On appelle ça un attracteur. Si on suivait l'ordre des mots, on écrirait « est ». L'accord suit la structure de la phrase, pas l'ordre des mots.

**[clic]** Pourquoi ce phénomène ? Parce que la bonne réponse est connue, et qu'on peut poser exactement la même question à un humain et à un modèle.

**[clic]** La question devient : un réseau de neurones qui n'a vu que des phrases, sans aucune règle de grammaire, apprend-il cette structure ? Et si oui, comment ? L'avantage du modèle, c'est qu'on peut regarder chaque neurone.

**[clic]** C'est un petit phénomène, bien choisi, pour tester une grande question.

---

## Slide 17 — Dans le modèle : des « neurones du nombre »

C'est ce qu'ont fait Yair Lakretz et ses collègues, notamment Stanislas Dehaene, en 2019. Dans un réseau de 1 300 unités, un LSTM, un type de réseau plus ancien et plus simple que ChatGPT, ils ont trouvé deux unités qui gardent en mémoire le nombre du sujet : une pour le pluriel, une pour le singulier. Regardez la courbe : l'unité « pluriel » s'active sur « clés » et reste active jusqu'au verbe.

**[clic]** Un petit circuit, qu'on peut appeler syntaxique, décide à quel moment mettre ces unités à jour.

**[clic]** Et la preuve qu'elles servent : si on les supprime, le modèle fait des erreurs d'accord.

**[clic]** On a donc trouvé un mécanisme précis, testable et manipulable. C'est quelque chose qu'on ne peut pas faire dans un cerveau humain.

Ce mécanisme concerne la structure de la phrase. Mais le langage suffit-il pour penser ? C'est notre volet suivant.

---

## Slide 18 — Pensée : le langage n'est pas la pensée

Deuxième volet : la pensée. On a souvent l'impression que penser, c'est se parler dans sa tête. Mais le cerveau suggère autre chose.

En rouge, le réseau du langage : comprendre et produire des phrases.

**[clic]** En bleu, un autre réseau, qu'on appelle « multi-demande » : il s'active pour le calcul, la logique, la résolution de problèmes.

**[clic]** Et certains patients aphasiques, qui ont perdu une grande partie du langage, peuvent encore calculer et raisonner.

**[clic]** Chez l'humain, langage et pensée s'appuient donc sur des réseaux en grande partie distincts. Pour les IA comme ChatGPT, qui parlent très bien, la question de savoir si elles « pensent » reste ouverte.

Revenons aux neurones du nombre : ils gardent une information en mémoire, du sujet jusqu'au verbe. Ça nous amène au dernier volet, la mémoire.

---

## Slide 19 — Mémoire : garder le sujet en tête jusqu'au verbe

Notre mémoire de travail est limitée. Plus le verbe est loin de son sujet, plus la lecture ralentit. Sur le schéma : en haut, sept mots entre le sujet et le verbe, c'est coûteux ; en bas, ils sont côte à côte, c'est facile.

**[clic]** Si on donne à un modèle une mémoire imparfaite du contexte, comme la nôtre, il reproduit mieux ces difficultés humaines.

**[clic]** Le raisonnement est simple : si un modèle à la mémoire limitée bute sur les mêmes phrases que nous, c'est que notre difficulté vient de la mémoire. Cette idée, donner à un modèle une limite « humaine », c'est exactement ce que j'ai poussé plus loin dans mon travail.

---

## Partie 4 — Mon travail : des modèles plus humains ?

Je vais maintenant vous présenter mon propre travail.

---

## Slide 20 — La question

Vous vous souvenez de ce qu'on ne savait pas : pourquoi les plus grands modèles ne sont pas toujours plus « humains ». C'est de là que part ma question : si l'on donne à un modèle des limites humaines, devient-il plus proche de l'humain ?

**[clic]** Première limite : la mémoire. Le modèle oublie progressivement le contexte, comme notre mémoire de travail.

**[clic]** Deuxième limite : les données. Au lieu de milliers de milliards de mots, on entraîne le modèle avec 10 à 100 millions de mots, à peu près ce qu'entend un enfant. C'est le défi BabyLM.

**[clic]** Pour tester ça, nous avons comparé 118 modèles sur 18 jeux de données : 7 jeux comportementaux, comme les temps de lecture et l'oculométrie, et 11 jeux cérébraux, en IRMf, MEG, EEG et électrodes intracrâniennes.

---

## Slide 21 — Résultat : lecture et cerveau ne vont pas ensemble

Voici le résultat. Chaque point est un modèle. Plus il est à droite, plus il est proche du cerveau. Plus il est en haut, plus il est proche de la lecture humaine.

**[clic]** En haut à gauche, les petits modèles contraints, avec peu de données ou une mémoire limitée. Ils sont plus proches de la lecture humaine, mais plus loin du cerveau.

**[clic]** En bas à droite, les grands modèles montrent l'inverse : proches du cerveau, mais loin de la lecture.

**[clic]** Et parmi nos modèles, aucun n'est en tête sur les deux scores à la fois.

**[clic]** Ce que ça nous dit : « ressembler à l'humain » n'est pas une seule propriété. Il faut toujours préciser à quel niveau : le comportement, ou l'activité du cerveau.

Ce sont des résultats préliminaires, le travail est en cours.

---

## Partie 5 — Application : décoder le langage dans le cerveau

Pour finir, une application concrète, qui montre que tout cela n'est pas seulement théorique.

---

## Slide 22 — Encoder, décoder : deux directions

Jusqu'ici, on a comparé le modèle au cerveau, en partant du langage et du modèle pour prédire l'activité du cerveau : c'est ce qu'on appelle l'encodage. Le but était de comprendre le cerveau.

**[clic]** On peut aussi faire l'inverse : décoder, c'est-à-dire partir de l'activité du cerveau pour retrouver les mots. Là, le but est d'aider des personnes.

Je vais vous montrer deux exemples :
**[clic]** avec des électrodes implantées dans le cerveau, les travaux de Willett et collègues ;
**[clic]** et sans chirurgie, avec l'IRMf, les travaux de Tang et collègues.

**[clic]** Le point commun : ce sont les mêmes outils, réseaux de neurones et modèles de langage, qui servent dans les deux sens.

---

## Slide 23 — Redonner la parole : électrodes implantées

Premier exemple, publié dans *Nature* en 2023. Une patiente atteinte de SLA, une maladie qui paralyse progressivement les muscles, ne peut plus parler de façon intelligible. Des micro-électrodes ont été implantées dans les zones de son cerveau qui contrôlent la parole. Elle tente de prononcer des phrases.

**[clic]** Un réseau de neurones apprend à reconnaître, dans son activité cérébrale, les sons qu'elle essaie de produire.

**[clic]** Puis un modèle de langage, le même type de modèle que dans la première partie, corrige et complète, en choisissant les phrases les plus probables.

**[clic]** Et la phrase s'affiche à l'écran.

**[clic]** Les résultats : 9 % d'erreurs sur les mots avec un vocabulaire de 50 mots, et 24 % avec un vocabulaire de 125 000 mots.

**[clic]** Et la vitesse : 62 mots par minute. C'est beaucoup plus rapide que les méthodes précédentes, mais encore loin des 160 mots par minute d'une conversation normale.

---

## Slide 24 — Retrouver le sens d'une histoire avec l'IRMf

Deuxième exemple, sans chirurgie cette fois : avec l'IRMf. Trois participants ont écouté 16 heures d'histoires dans l'IRM.

Le décodeur fonctionne comme une boucle. Un modèle de langage propose des suites de phrases possibles.

**[clic]** Pour chacune, un modèle d'encodage prédit quelle activité IRMf elle devrait produire. C'est exactement le modèle d'encodage de la partie 2, utilisé à l'envers.

**[clic]** On compare ces prédictions au vrai signal mesuré.

**[clic]** Et on garde les meilleures suites, puis on recommence.

**[clic]** Le résultat : le décodeur retrouve l'idée générale de l'histoire, pas les mots exacts.

**[clic]** Il marche même quand la personne imagine une histoire, ou regarde un film muet.

**[clic]** Mais le décodeur est propre à chaque personne : celui entraîné sur quelqu'un ne marche pas sur une autre. Et si la personne résiste, par exemple en pensant à autre chose, il échoue.

**[clic]** Et il faut un IRM : impossible à utiliser au quotidien.

---

## Slide 25 — Limites et questions éthiques

Ces résultats sont impressionnants, mais il faut être lucide.

La précision : on est encore loin d'une conversation fluide, surtout sans chirurgie.

**[clic]** La vie privée mentale : qui a le droit d'accéder à ces données, et pour en faire quoi ?

**[clic]** Le consentement : le décodage exige que la personne participe volontairement. Il ne doit jamais être imposé.

**[clic]** L'accès équitable : ces technologies ne doivent pas être réservées à quelques pays.

**[clic]** Ce sont des résultats réels, et déjà utiles aux patients. Mais on est encore loin de « lire dans les pensées ».

---

## Conclusion

---

## Slide 26 — Trois messages à retenir

Si vous ne retenez que trois choses de cet exposé.

Premièrement : l'IA, ce n'est pas que ChatGPT. C'est aussi un instrument scientifique, pour étudier le langage dans le cerveau, et pour aider des patients.

**[clic]** Deuxièmement : un modèle est une hypothèse. Il prédit une partie de l'activité cérébrale et de la lecture, et on peut l'ouvrir pour y trouver des mécanismes, comme les neurones du nombre.

**[clic]** Troisièmement : prédire n'est pas expliquer. Un bon score ne suffit pas. Il faut tester les mécanismes, et préciser à quel niveau un modèle ressemble à l'humain.

---

## Slide 27 — Et pour la Guinée ?

Et pour nous, en Guinée ? Je pense qu'il y a de vraies opportunités.

Nos langues, d'abord. Vous vous souvenez : on ne sait pas ce qui vaut hors de l'anglais, parce que presque toutes les données sont en anglais. Le pular, le maninka, le soussou… sont absents. C'est une vraie place à prendre.

**[clic]** Ensuite, ce type de recherche ne demande pas forcément beaucoup de matériel. L'EEG est portable et peu coûteux, et les temps de lecture se mesurent avec un simple ordinateur.

**[clic]** Et les outils sont ouverts. Les modèles et les données sont en libre accès, sur Hugging Face, MNE-Python ou Brain-Score, et il existe des formations gratuites comme Neuromatch Academy.

**[clic]** Comprendre comment un cerveau guinéen traite sa propre langue, c'est une question scientifique ouverte. Et elle peut être traitée ici.

---

## Merci !

Merci beaucoup pour votre attention. Je serai ravi de répondre à vos questions.

Vous pouvez scanner le QR code pour télécharger les slides, et me contacter à l'adresse affichée : boubacar.sow@ens.psl.eu.
