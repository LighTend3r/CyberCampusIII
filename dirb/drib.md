# dirb

**/!\ En construction**

## Description :

Dirb est un commande intégré dans KaliLinux, elle permet de faire un recherche de tout les dossier/fichier qui peuvent potentiellment exister sur un site Web.

## Commande :
```
dirb <url> [wordlist_file] [options]
```

---

### Utilisation classique :

Une utilisation classique de dirb qui consiste juste en une recherche de dossier sur le site web mis en argument
```
dirb http:siteweb/fichier/out/content/ /usr/share/wordlist/dirb/commun.txt
```

Une autre utilisation assez commune qui permet de rechercher des fichiers sur un site web, l'option `-t` permet de ne pas rajouter le `\` à la fin de l'url, **car ce n'est pas un dosier qu'on chercher**
```
dirb http:siteweb/fichier/out/content/index.html?page= /usr/share/wordlist/dirb/commun.txt -t
```

### Option :

* **-t**

Comme vue plus haut, l'option `-t`, empêche l'antislash de ce mettre a la fin de l'url rechercher, ça permet de **rechercher des fichiers** et non des dossiersd


