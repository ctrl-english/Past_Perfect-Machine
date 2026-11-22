# 🕰️ The Past Perfect Machine

Jeu pédagogique en ligne pour travailler la différence entre **past perfect simple** et **past perfect be + ing** (le past perfect en anglais). L'application se limite volontairement à ce contraste : le prétérit n'y apparaît que comme repère du récit. En un seul fichier, sans installation ni dépendance : elle fonctionne entièrement dans le navigateur de l'élève.

## 🎮 Les 5 mini-jeux

| Jeu | Objectif |
| --- | --- |
| 🗃️ Le tri des étapes | Ranger 8 phrases dans la bonne boîte à étapes (avant le récit, explication d'un résultat, durée écoulée, arrière-plan du récit) |
| 🔀 Mélange des mots | Reconstituer 5 phrases en remettant les mots dans le bon ordre |
| ✍️ La machine à écrire | Choisir la bonne forme du past perfect entre deux propositions, sur 8 phrases |
| ⚡ Quiz éclair | 10 questions en 20 secondes chacune |
| 🧠 Mémo du past perfect | Retrouver les 8 paires de phrases le plus vite possible |

Le tout est complété par un **Mémo des règles** (past perfect simple vs past perfect be + ing, avec le tableau des marqueurs) consultable avant de jouer, un système d'étoiles (jusqu'à 15 ★) et un rapport de résultats envoyé au professeur. Les phrases s'appuient sur des situations de commerce et de marketing, adaptées aux BTS tertiaires.

## 📤 Rapport des résultats

Après avoir joué à toutes les épreuves, l'élève peut envoyer son rapport (scores, étoiles, prénom, classe) à son professeur par e-mail via le service gratuit FormSubmit. L'adresse du destinataire se règle dans `REPORT_CONFIG.teacherEmail` (voir ci-dessous).

## ▶️ Utilisation

Ouvrir simplement `index.html` depuis n'importe quel hébergement statique (GitHub Pages, etc.) ou l'adresse donnée par le professeur. Les scores et le prénom du joueur sont gardés dans le stockage local du navigateur : rien n'est envoyé tant que l'élève ne clique pas sur « Envoyer mon rapport ».

## ✏️ Personnaliser l'exercice

Tout le contenu pédagogique se trouve dans les blocs de données au début de `index.html`, modifiables librement :

- `QUIZ_DATA` : les 10 questions du quiz, avec les options et l'explication (`why`) affichée après la réponse
- `SORT_ROLES` et `SORT_DATA` : les boîtes (les emplois du past perfect) et les phrases du jeu de tri
- `MEMORY_DATA` : les 8 paires du mémoire
- `SCRAMBLE_DATA` : les 5 phrases à reconstituer
- `FILL_DATA` : les 8 phrases de la machine à écrire
- `REPORT_CONFIG.teacherEmail` : l'adresse e-mail qui reçoit les rapports

Au tout premier envoi d'un rapport, FormSubmit envoie un e-mail d'activation à cette adresse : cliquer sur le lien qu'il contient pour activer la réception.

## 🔧 Technique

- Un seul fichier HTML (structure, styles et moteur de jeu inclus), aucun framework ni dépendance externe
- Stockage local du navigateur pour les records et le joueur
- Envoi du rapport via FormSubmit (gratuit, sans inscription)

## 📄 Licence

Distribué sous licence [MIT](LICENSE).
