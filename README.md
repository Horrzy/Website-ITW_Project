# Black Books – ITW Projekt

Jednostránková webová prezentace fiktivního londýnského knihkupectví **Black Books**, inspirovaná stejnojmenným britským sitcomem. Projekt vznikl v rámci předmětu **ITW (Tvorba webových stránek)** na **FIT VUT v Brně** (2025).

## O projektu

Hlavním cílem projektu bylo vytvořit kompletní vizuální styl a rozvržení stránky v čistém CSS ([`css/style.css`](css/style.css)) nad předem připravenou HTML kostrou ([`index.html`](index.html)) a pomocnými JavaScriptovými skripty. Stránka je stylována do retro/knižního vzhledu s využitím písem *IM Fell DW Pica* a *Spectral*, sépiových filtrů a plynulých CSS přechodů.

### Hlavní prvky a sekce

- **Výsuvné postranní menu** – fixní navigační panel na levém okraji okna s ikonami Font Awesome, který se po najetí myší plynule vysune.
- **Úvodní hlavička (Header)** – tmavé záhlaví s pozadím, vinětou a hover efektem.
- **Home** – představení knihkupectví doplněné o vlastní HTML5 video přehrávač s upravenými ovládacími prvky (přehrát/pozastavit, časová osa s náhledem času, ztlumení, režim celé obrazovky).
- **Products** – přehled produktů v responzivní mřížce (CSS Grid) s animovaným zobrazením popisků při najetí myší.
- **Services** – nabídka služeb (*Tax Consulting*, *Reading Lessons*, *Recommendation of Books*) se střídavým rozložením obrázků, cenami a odkazy na ukázky.
- **Events** – časová osa (timeline) akcí rozdělená svislou linkou na levou a pravou stranu s interaktivním zobrazením detailů.
- **Clients** – automaticky se střídající citace zákazníků (slider řízený přes CSS proměnnou `--slider-time` a `js/slider.js`).
- **Contact** – sekce s dalším videem a rezervačním formulářem na vybrané události, po jehož odeslání se zobrazí notifikace.
- **Patička & návrat nahoru** – tlačítko pro návrat na začátek stránky aktivované při odscrollování (`js/scroll.js`).

## Použité technologie

- **HTML5**
- **CSS3** (CSS Grid, Flexbox, přechody a animace, filtry, masky, vlastní proměnné)
- **JavaScript** (pomocné skripty pro přehrávač videa, slider, detekci scrollování a toast notifikaci)
- **Google Fonts** (`Spectral`, `IM Fell DW Pica`)
- **Font Awesome 6**

## Struktura projektu

```text
.
├── index.html          # Hlavní HTML dokument
├── css/
│   └── style.css       # Kompletní stylování stránky
├── js/
│   ├── scroll.js       # Detekce scrollování stránky
│   ├── slider.js       # Automatické přepínání citací v sekci Clients
│   ├── toast.js        # Zobrazení notifikace po odeslání formuláře
│   └── video.js        # Logika vlastního video přehrávače
├── img/                # Obrázky, ilustrace a SVG ornament
└── video/              # Vložená videa (heaven.mp4, shoes.mp4)
```

## Spuštění

Projekt je čistě statický a nevyžaduje žádný build krok ani instalaci závislostí. Stačí otevřít soubor `index.html` přímo v webovém prohlížeči, případně spustit lokální HTTP server:

```bash
python3 -m http.server 8000
```

Následně otevřete adresu `http://localhost:8000`.

## Autor a kredity

- **Řešení stylů (`css/style.css`)**: `xraskaj00` (FIT VUT v Brně)
- **Zadání, HTML šablona a pomocné JS skripty**: Jiří Hynek / Dexter@FIT (2025), pouze pro vzdělávací účely.
