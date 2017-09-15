
# Comment (à peu près) bien utiliser github à plusieurs
## Comment fonctionnent les branches? (silence ça pousse)

**Créez une nouvelle branche par feature** sur laquelle vous travaillez, vous ne devriez pas travailler sur plusieurs
trucs séparés en même temps sur la meme branche, sinon en cas de création de bug sur l'une des features, il sera
necessaire de perdre des avancées sur l'autre feature qui fonctionne en revenant en arrière.

**Utilisez VCS > git > branches** pour creer et/ou switcher sur une branche désirée.

**Utilisez VCS > git > pull** sur la branche souhaitée pour repartir sur des bases propres si vous changez de branches
en cours de modifications.

**Utilisez VCS > git > rebase > experimental** après validation et test de votre modification par tout le monde pour
ajouter votre travail au projet en phase de debug

**Utilisez VCS > git > rebase > master** Quand une version stable, testée et a peu près complète est prête pour faire
 des demonstrations.


## Comment faire des commits propres? (Réponse: En les lavant)

**Ne modifiez qu'un seul fichier par commit**, avec une description brève de ce qui y a été ajouté/réglé/amélioré.
Cela permet d'avoir un historique clair sur les versions des fichiers et d'eviter de perdre des changements si il y a
 besoin de revenir en arrière.

## L'importance des code review ( Par ce qu'on aime ça le voyeurisme )

Il serait important de se faire mutuellement **des revisions de code honnêtes à chaque fois demande de fusion de
branches** au projet. Cela inclut:

- Se dire bonjour et des conneries :D
- Faire remarquer si la coding-style du projet est parfois non-respectée
- Dire si des morceaux de codes sont trop peu explicites ou documentés (compréhensibles)

Il serait bon de ne pas fusionner tant qu'au moins l'un de nous (au mieux tout le monde) ne donne pas le feu vert et
tant qu'il reste des petits defauts à corriger. Ca permettra d'avoir un prototype **propre, lisible et comprehensible
pour plus tard**.
