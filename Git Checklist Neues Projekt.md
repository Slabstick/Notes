#Git #GitHub #IntelliJ

1. Repo erstellen in GitHub/BitBucket
2. Lokalen Arbeitsordner anlegen
3. init commit
	1. `git init`
4. Projekt in IntelliJ anlegen
	1. Advanced Settings -> Content root auf lokalen Ordner setzen
5. gitIgnore commit
	1. .idea Ordner -> .gitignore (Wenn schon angelegt. Sonst später)
	2. .gitignore auf www.gitignore.io erstellen
	3. `git add .`
	4. `git commit -m "first commit"`
	5. `git branch -M main`
6. Mit Remote verknüpfen:
	- Github: `git remote add origin git@github.com:UserName/Repo.git`
	- Bitbucket: `git remote add origin https://jklimczok@intern.quinscape.de/bitbucket/scm/~jklimczok/Repo.git`
7. `git push -u origin main`
8. `git checkout -b firstCode`
9. `git push --set-upstream origin firstCode`
10. Jetzt erst anfangen zu coden

## Merge to Main

1. `git checkout main`
2. `git merge firstCode`
3. `git push origin main`

## Fehlerbehebung

### Github/BitBucket remote URL falsch eingegeben:
- `git remote set-url origin git@github.com:UserName/Repo.git`
oder
- `git remote set-url origin https://jklimczok@intern.quinscape.de/bitbucket/scm/~jklimczok/Repo.git`
- `git push -u origin --all`

### Delete Branch
- `git branch -d local_branch_name`

### User aktualisieren
- `git config user.name "Jakob Klimczok"`
- `git config user.email "Jakob.Klimczok@quinscape.de"`
