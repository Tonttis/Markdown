# Git ja GitHub - Perusteet

## Git-versionhallinnan tärkeimmät asiat
Git on hajautettu versionhallintajärjestelmä, jonka avulla voidaan seurata muutoksia ohjelmistokehitysprojekteissa. Se mahdollistaa yhteistyön, muutosten hallinnan ja version palauttamisen tarvittaessa.

---

## Git peruskomennot

**1. git add**

```bash
git add tiedosto.txt
```
Lisää tiedoston seurantaan staged-tilaan.

**2. git commit**

```bash
git commit -m "Viesti muutoksista"
```
Tallentaa staged-tilassa olevat muutokset paikalliseen repositorioon.

**3. git status**

```bash
git status
```
Näyttää tilatietoa muutoksista.

**4. git push**

```bash
git push origin main
```
Lähettää paikalliset muutokset GitHubiin.

**5. git branch**

```bash
git branch uusi-haara
```
Luo uuden haaran (branch) kehitykselle.

---

## Muutosten peruuttaminen

**1. git checkout**

```bash
git checkout -- tiedosto.txt
```
Peruu työtilassa olevat muutokset tietylle tiedostolle.

**2. git revert**

```bash
git revert HEAD
```
Luo uuden commitin, joka kumoaa edellisen muutoksen.

**3. git reset**

```bash
git reset --hard HEAD~1
```
Palauttaa projektin edelliseen commit-tilaan poistamalla muutokset.

---

## GitHubin käyttö

### Paikallisen hakemiston kytkeminen GitHubiin

1. Luo uusi repositorio GitHubissa.
2. Alusta paikallinen hakemisto:

```bash
git init
git remote add origin https://github.com/kayttaja/repo.git
git branch -M main
git push -u origin main
```

---

### Tiedon lähettäminen ja hakeminen

**Tietojen lähetys GitHubiin:**

```bash
git push origin main
```

**Tietojen hakeminen GitHubista:**

```bash
git pull origin main
```

---

## Forkkaaminen ja upstream

**Forkkaaminen GitHubissa:**

1. Siirry haluttuun GitHub-repositorioon.
2. Klikkaa *Fork* ja kopioi uusi repositorio omaan tiliisi.

**Forkin kloonaaminen paikallisesti:**

```bash
git clone https://github.com/oma-kayttaja/forkattu-repo.git
```

**Upstream lisääminen forkkiin:**

```bash
git remote add upstream https://github.com/alkuperainen-kayttaja/alkuperainen-repo.git
git fetch upstream
git merge upstream/main
```

---

## Markdown-muotoilut esimerkkeinä

**Lihavointi ja kursivointi**

*kursivoitu teksti*  
**lihavoitu teksti**  

**Kuvat**
Paikallinen kuva
![Paikallinen kuva](git-logo.png)

Verkkolinkitetty kuva
![Verkkolinkitetty kuva](https://git-scm.com/images/logo@2x.png)

**Koodilohko**

```python
print("Hei Git!")
```

**Hyperlinkki**

[Git dokumentaatio](https://git-scm.com/doc)

**Vaakaviiva**

---

**Lohkolainaus**

> Versionhallinta on avain onnistuneeseen ohjelmistokehitykseen.

**Luettelo**

- Git-versiohallinta
- GitHub-repositoriot
- Komennot ja työkalut

