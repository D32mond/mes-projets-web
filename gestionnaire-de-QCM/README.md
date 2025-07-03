LIFAP5 - projet 2019-2020 : gestionnaire de QCM en JavaScript
=============================================================

* URL de votre dépôt <https://forge.univ-lyon1.fr>
* DOMINGUES kévin 11607884 #1
* monôme #2
* UCBL QCM

Fonctionnalités obligatoires
----------------------------

_*_Vous devez réaliser _toutes ces fonctionnalités_ pour avoir la note maximale_*_. Cocher celles réalisées :

* [X] **Modifier l'utilisateur connecté** : il faut pour cela remplir la champ `xApiKey` de l'objet `state` déclaré dans `js/modeles.js`. Comprendre le fonctionnement permettant le mise à jour de l'état (dans `js/modeles.js`) et la modification du comportement du bouton "utilisateur" (dans `js/vues.js`). Ensuite, il faut permettre de choisir l'utilisateur avec lequel on se connecte et se délogguer le cas échéant.

* [X] **Afficher les questions et les propositions d'un quiz** : lorsque l'on clique sur un quiz, la fonction `clickQuiz` (définie dans `js/vues.js`) est appelée. Elle appelle `renderCurrentQuizz` qui va changer l'affichage du div HTML `id-all-quizzes-main`. Modifier ces fonctions de façon à afficher les questions (et leurs propositions de réponses) du quiz au lieu de "Ici les détails pour le quiz xxyyzz".

* [X] **Répondre à un quiz**: modifier l'affichage précédent de façon à pouvoir répondre au quiz, c'est-à-dire pouvoir cocher la réponse choisie à chaque question, puis cliquer sur un bouton "Répondre" qui enverra les réponses au serveur.

* [X] **Afficher les quiz de l'utilisateur connecté et des réponses déjà données** : reprendre la fonctionnalité d'affichage de tous les quiz et l'adapter pour afficher les quiz de l'utilisateur connecté dans l'onglet "MES QUIZ". Similairement, remplir l'onglet "MES REPONSES" pour afficher les quiz auxquels l'utilisateur connecté a répondu.

* [X] **Créer un quiz pour l'utilisateur connecté** : ajouter un formulaire permettant de saisir les informations d'un nouveau quiz dans l'onglet "MES QUIZ". Ajouter un bouton "Créer" qui déclenchera l'ajout du quiz sur le serveur et le rafraîchissement de la liste des quiz. Permettre d'ajouter aux quiz de l'utilisateur connecté un formulaire d'ajout de question. Ce formulaire permettra de saisir les propositions possibles pour la question. Sa validation déclenchera l'ajout de la question sur le serveur_.

Fonctionnalités optionnelles (au choix)
---------------------------------------


*Vous devez réaliser _au moins trois catégories de fonctionnalités_ pour avoir la note maximale*. Cocher celles réalisées :

* [X] Catégorie **modifications de quiz et de leurs questions**
  - Mettre à jour un quiz : changer la description et le titre d'un quiz.   Ajouter un bouton "Modifier" qui va faire apparaître un formulaire de modification. Gérer ce formulaire pour mettre à jour les données sur le serveur.
  - Mettre à jour l'énoncé une question: changer la phrase (`sentence`) d'énoncé et permettre ~~d'ajouter/supprimer une proposition à une question~~ de modifier une proposition: ajouter par exemple un bouton de suppression à côté de chaque question ~~et un formulaire d'ajout de proposition~~ (NB, le serveur ne propose pas de route permettant de manipuler les propositions, tout passe par l'API des questions)  

* [X] Catégorie **formulaire de recherche**
  - Le formulaire de recherche en haut de la page permet de recherche en texte plein sur tous les champ de texte des quiz, des questions et des propositions. Changer le comportement de l'onglet "TOUS LES QUIZ" pour mettre en surbrillance les éléments retournés par le résultat de la recherche.  

Remarques additionnelles
------------------------

 J'ai rajouter un bouton relier à une fonction pour supprimer un QCM.  
 J'ai modifier la Catégorie **formulaire de recherche** pour afficher que les réponses de la recherche et un boutton pour supprimer le filtre.  
