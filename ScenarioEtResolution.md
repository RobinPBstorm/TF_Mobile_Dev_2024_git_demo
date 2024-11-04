 # Git
 
<details>
  <summary>Table des matières</summary>
  <ol>
    <li>
     <a href="#avant-de-demarrer">Avant de demarrer</a>
    </li>
    <li>
     <a href="#exporter-un-projet">Exporter un Projet</a>
    </li>
    <li>
      <a href="#importer-un-projet">Importer un projet</a>
    </li>
    <li>
      <a href="#travail-a-plusieurs-sur-git">Travail a plusieurs sur git</a>
    </li>
  </ol>
</details>

 ## 1. Avant de demarrer

### Télécharger Git

[Lien pour télécharger](https://git-scm.com/downloads)

Pour vérifier s'il est installé:

```
git --version
```

En cas de trou de mémoire:

```
git --help
```

 ## 2. Exporter un Projet

**Première fois avec git sur cette machine ?**

Ajoutons notre nom et l'email dans la configuration globale
```
git config --global user.name "John Doe"
git config --global user.email johndoe@example.com
```

### Préparer le projet pour git

Bien le faire dans le dossier du projet

```
git init
```

### Vérifions l'état des fichiers
Pour afficher l'état de mes fichiers du projet:

```
git status
```

Pour renommer la brance **master** en **main**

```
git branch -M main
```
### Ajout des fichiers à envoyer

Indiquer quel(s) fichier(s) on enverra sur le dépôt distant

Soit un par un:
```
git add nom_fichier
```

ou tout ceux modifié:
```
git add .
```

### Plaçons un message pour décrire l'ensemble de modification qu'on envoit 

Préparons les modifications à l'envoi et en indiquant un message:
```
git commit -m "message pour le commit"
```

**Pas encore de dépôt distant d'enregistré ?**
```
git remote add origin https://github.com/RobinPBstorm/TF_Mobile_Dev_2024_git_demo.git
```

### Envoit des commits

Enfin, nous envoyons nos changement avec:

-la première fois:
```
git push -u origin main
```
-les fois suivante:
```
git push
```

 ## 3. Importer un projet

On clone le projet (l'adresse est trouvable sur la github du projet)
```
git clone https://adresse_projet
```

 ## 4. Travail a plusieurs sur git

un truc
