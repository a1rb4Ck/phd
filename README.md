# Pierre Nagorny's PhD thesis

## Template

From SYMME lab PhD Jean Collomb, David Leh, Florian Huet

### Fonctionnement

* Le fichier "manuscrit.tex" (dossier manuscrit) est le document maître.
* Il suffit de rédiger des les fichiers .tex de chacun des dossiers, puis d'excécuter le fichier maître.
* Il est possible d'ajouter ou de supprimer des dossiers/fichiers (par exemple des chapitres). Il suffit d'ajouter/désactiver les lignes correspondantes dans le fichier "manuscrit.tex".

### Modifications autres

* Logo de l'université (Grenoble Alpes) peut être modifié dans le fichier "meta-donnees.sty".
* Spécialité du doctorat peut être modifiée dans le fichier "meta-donnees.sty".
* Laboratoire peut être modifié dans le fichier "meta-donnees.sty".
* Ecole doctorale peut être modifiée dans le fichier "meta-donnees.sty".
* Des packages peuvent être ajoutés dans le fichier "packages.tex".
* Les couleurs (Tableaux, références, liens ...) peuvent être modifiés dans le fichier "packages.tex" via le package "hyperref".

### Technical hints

#### macOS

Use Basic MacTex, TexStudio and install new packages with _tlmgr_.  

```bash
brew cask install texstudio
brew cask install basictex  
```

To install new package:  

```bash
tlmgr install package  
```

#### Found your missing packages!

```bash
tlmgr info package.sty

> Packages containing files matching `package.sty':  
>     package-with-a-strange-name:  
>         texmf-dist/tex/latex/package-with-a-strange-name/package.sty  
```

```bash
tlmgr install package-with-a-stange-name  
```

#### List all your installed latex packages

```bash
tlmgr list --only-installed > installed_texlive_packages.txt
```
