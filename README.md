# Astro + Netlify starter

En minimal företagshemsida med kontaktformulär för Netlify Forms.

## 1. Installera

```bash
npm install
```

## 2. Starta lokalt

```bash
npm run dev
```

Öppna sedan den lokala adressen som Astro visar i terminalen.

## 3. Byt innehåll

- `src/pages/index.astro` = startsidan
- `src/pages/tack.astro` = tacksidan efter formuläret
- `src/layouts/BaseLayout.astro` = global layout och all styling

## 4. Lägg på GitHub

```bash
git init
git add .
git commit -m "Initial Astro site"
```

Skapa ett tomt repo på GitHub och koppla det:

```bash
git remote add origin <DIN_GITHUB_REPO_URL>
git branch -M main
git push -u origin main
```

## 5. Deploy på Netlify

1. Logga in på Netlify
2. Välj **Add new project**
3. Importera från GitHub
4. Välj ditt repo
5. Netlify brukar känna av Astro automatiskt
6. Build command: `npm run build`
7. Publish directory: `dist`
8. Deploy

## 6. Kontaktformulär

Formuläret är redan markerat med:

- `data-netlify="true"`
- hidden field för `form-name`

När sajten ligger live på Netlify kan formulärsvar dyka upp under forms/submissions i Netlify.

## 7. Eget domännamn

Det lägger du till i Netlify efter deploy.

## 8. Vanliga ändringar

- byt företagsnamn i `BaseLayout.astro`
- byt texter i `index.astro`
- ändra färger i `:root`
- lägg till fler sektioner direkt i `index.astro`
