# test-conflict

Normalement, dans le développement réel d'une application, des conflits se produiront spontanément. Cependant, pour notre formation, nous allons intentionnellement forcer un conflit dans git.

Dans la plupart des cas, git est capable de mélanger les modifications que différents utilisateurs apportent à différents fichiers, mais si deux utilisateurs apportent des modifications au même fichier localement (surtout si la modification se trouve sur la même ligne), git ne pourra pas savoir quelle modification est la bonne. Produisons un tel conflit :

<<<<<<< HEAD
- Voici une ligne du README.md avec deux (deux) fautes de frappe (fautes de frappe) à corriger
=======
- Voici une ligne du README.md avec deux (deux) fautes de frappe (fautes de frappe) à corriger
>>>>>>> 66d210e6354cc56d5c850bf5362c125bcb6cf6d9

- **Athos** corrigera la première faute de frappe (deux) et **Porthos** la seconde (fautes de frappe) 

- Chacun va faire un clone du repositoire et corriger sa faute de frappe localement, puis essayer de faire un `push` du changement. 
