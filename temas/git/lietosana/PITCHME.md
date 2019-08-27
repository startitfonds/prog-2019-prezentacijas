## Kā to lieto?

+++

### Termini

@ul

- Repozitorijs (repository), repo - koda organizācijas vienība, mape
- Versija (version) - saglabāti un pieejami datņu satura varianti
- Kommits (commit) - izmaiņu versijas saglabāšana (process), pati versija
- Zars (branch) - paralēla izmaiņu versija repozitorijā

@ulend

+++

### GitHub

git repozitoriju tiešsaistes krātuve

+++

Esoša repozitorija pievienošana (fork) savam GitHub kontam

@img[](assets/img/github-fork.png)

+++

Repozitorija klonēšana ar GitHub Desktop

@img[](assets/img/gh-desktop-clone.png)

+++

Repo mapes atvēršana VSCode

@img[](assets/img/gh-desktop-open-vsc.png)

---

### Ja VSCode rāda git error

@img[](assets/img/vscode-git-error.png)

+++

- iekš VSCode - atver Command Palette (Ctrl+Shift+P)
- atrod un atver "settings.json" datni
- izveido ierakstu, kur iestatīt "git.exe" atrašanās vietu

Ierakstam jāizskatās tā:

```
{
    "git.path": "C:/ "
}
```

+++

- atrod un atver mapi, kur tika ieinstalēts "Git for Windows" vai GitHubDesktop
- atrod "git.exe" atrašanās vietu
- saglabā "settings.json" datni

+++

### Aizver un atkal atver VSCode

Tagad viss ir kārtībā!

@img[](assets/img/vscode-git-view-light.png)

Ja nav, sauciet mentoru!

---

### VSCode integrācija

@img[](assets/img/vscode-side-icons.png)

+++


### Lejupielādē (klonē) repozitoriju lokāli

 @img[](assets/img/github-repo-menu.png)
 
 @img[](assets/img/gh-desktop-clone.png)
 
 ```
 git clone https://github.com/vards/repo-nosaukums.git
 ```

+++

### Izveido jaunu zaru

Darbojas kā virtuāla kopija visai repozitorijas struktūrai un datiem.

@img[](assets/img/gh-desktop-branching.png)

```
git checkout -b gd--b123-labojums
```

+++

### Reģistrē mainītu datni saglabāšanai

- Izmaiņu pievienošana repo nenotiek automātiski.
- Mainīta datne būs iezīmēta (**M**).
- Izmainīto datni vai datnes jāpievieno "staging" sarakstam.
- Kad pievienotas visas datnes, veic "commit".

+++

### Saglabā reģistrētās datnes jaunā versijā

@img[](assets/img/vscode-git-commit.png)

```
git add .
git commit -m "Izmaiņas aprakstošs komentārs"
```

+++

### Publicē visas versijas (kommitus) tiešsaistes repo

@img[](assets/img/gh-desktop-push.png)

```
git push
```

+++

### Lejupielādē visas izmaiņas no tiešsaistes repo

@img[](assets/img/gh-desktop-pull-changes.png)

```
git pull
```

+++

### Darba plūsma

@img[](assets/img/git-workflow-simple.png)

---

## Vēl par git un GitHub

+++

### Jauna repozitorija izveidošana

- var to darīt lokāli ar "git init"
- vienkāršāk ir to darīt caur GitHub un td veikt "clone"

+++

### Citu lietotāju repozitorija dublēšana

- "fork" - izveido savu repozitoriju, kas ir kopija
- ir visas tiesības savu repo un saturu mainīt

+++

### Lietotāju pievienošana un tiesības

- Lietotāja pievienošana
- Lietotāja tiesības

+++

### Izmaiņu pievienošanas pieprasījums

- Issuing a pull request
- Accepting a pull request

+++

### Merging
