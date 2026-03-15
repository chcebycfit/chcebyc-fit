# Wdrożenie chceByc.fit na GitHub Pages
## Instrukcja krok po kroku

---

## Metoda A — Przez przeglądarkę (bez Git, najszybsza)

### Krok 1 — Rozpakuj ZIP
Pobierz `chcebyc-fit.zip` i rozpakuj na pulpicie.
Powinieneś zobaczyć 13 plików: `index.html`, `chcebyc-*.html` i `chcebyc-logo.svg`.

### Krok 2 — Wejdź na GitHub
Otwórz: **https://github.com/chcebycfit/chcebyc-fit**

Jeśli repo nie istnieje — utwórz je:
1. Kliknij **+** (prawy górny róg) → **New repository**
2. Nazwa: `chcebyc-fit`
3. Zaznacz: **Public**
4. Zaznacz: **Add a README file**
5. Kliknij **Create repository**

### Krok 3 — Wgraj pliki
1. W repozytorium kliknij **Add file** → **Upload files**
2. Przeciągnij wszystkie 13 plików z rozpakowanego ZIP
3. Scroll w dół → **Commit changes** → kliknij zielony przycisk

### Krok 4 — Włącz GitHub Pages
1. Kliknij **Settings** (górne menu repo)
2. W lewym panelu kliknij **Pages**
3. Pod "Branch" wybierz: **main** i folder **/ (root)**
4. Kliknij **Save**

### Krok 5 — Czekaj 2 minuty
GitHub zbuduje stronę. Po chwili zobaczysz:

> ✅ Your site is live at **https://chcebycfit.github.io/chcebyc-fit/**

Gotowe!

---

## Metoda B — Przez Git (dla programistów)

```bash
# Sklonuj repo (jeśli jeszcze nie masz lokalnie)
git clone https://github.com/chcebycfit/chcebyc-fit.git
cd chcebyc-fit

# Skopiuj wszystkie pliki z ZIP do folderu repo
# (zastąp SCIEZKA_DO_ZIP właściwą ścieżką)
cp /SCIEZKA_DO_ZIP/*.html .
cp /SCIEZKA_DO_ZIP/*.svg .

# Wypchnij na GitHub
git add .
git commit -m "chceByc.fit v0.2.0 — 11 modułów prototypu"
git push origin main
```

Potem włącz Pages jak w Kroku 4 powyżej.

---

## Struktura URL po wdrożeniu

| Strona | URL |
|--------|-----|
| Hub nawigacyjny | https://chcebycfit.github.io/chcebyc-fit/ |
| Landing Page | https://chcebycfit.github.io/chcebyc-fit/chcebyc-landing.html |
| Rejestracja | https://chcebycfit.github.io/chcebyc-fit/chcebyc-auth.html |
| Dashboard | https://chcebycfit.github.io/chcebyc-fit/chcebyc-dashboard.html |
| Panel Trenera | https://chcebycfit.github.io/chcebyc-fit/chcebyc-coach.html |
| Panel Admina | https://chcebycfit.github.io/chcebyc-fit/chcebyc-admin.html |
| Pomiary | https://chcebycfit.github.io/chcebyc-fit/chcebyc-measurements.html |
| Kalendarz | https://chcebycfit.github.io/chcebyc-fit/chcebyc-calendar.html |
| Marketplace | https://chcebycfit.github.io/chcebyc-fit/chcebyc-marketplace.html |
| Profil | https://chcebycfit.github.io/chcebyc-fit/chcebyc-profile.html |
| Aplikacja mobilna | https://chcebycfit.github.io/chcebyc-fit/chcebyc-mobile.html |

---

## Uwagi

**Czcionki** — wczytują się z Google Fonts (wymaga internetu). Na offline nie zadziałają.

**Claude API** — działa w przeglądarce bez zmian. Onboarding, Panel Trenera
i Panel Admina mają prawdziwe wywołania AI.

**HTTPS** — GitHub Pages automatycznie daje certyfikat SSL. Claude API
wymaga HTTPS — działa poprawnie.

**Aktualizacja plików** — gdy coś poprawisz, wróć do repo → Upload files
→ przeciągnij zaktualizowane pliki → Commit. GitHub Pages zaktualizuje
się automatycznie w ciągu ~1 minuty.

---

*chceByc.fit · Prototyp v0.2.0 · Marzec 2026*
