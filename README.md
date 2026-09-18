# Kunskapskontroll 2 – Interaktiv datavisualisering med Plotly

Individuell fördjupningsuppgift i Python inom Data Science.

Projektet undersöker hur Plotly kan användas för att skapa interaktiva datavisualiseringar och vad interaktiviteten tillför jämfört med ett statiskt diagram. Pandas används för grundläggande förberedelse av data och Matplotlib används endast för en kort jämförelse.

## Projektfil

`Plotly_Gapminder_Jupyter.ipynb` är projektets körbara Jupyter Notebook. Den innehåller både förklaringar, kod och visualiseringar.

## Data

Projektet använder Gapminder-datasetet som finns inbyggt i Plotly Express:

```python
import plotly.express as px

df = px.data.gapminder()
```

Ingen extern datafil eller API-nyckel behövs. Datasetet innehåller bland annat:

- land (`country`)
- kontinent (`continent`)
- år (`year`)
- förväntad livslängd (`lifeExp`)
- befolkning (`pop`)
- BNP per capita (`gdpPercap`)

## Visualiseringar

Notebooken innehåller:

1. en dataöversikt
2. ett interaktivt linjediagram
3. ett interaktivt stapeldiagram
4. ett interaktivt bubbeldiagram
5. ett animerat bubbeldiagram över tid
6. ett diagram med filtrering via dropdown
7. en jämförelse mellan ett statiskt Matplotlib-diagram och ett interaktivt Plotly-diagram

Plotly-diagrammen demonstrerar bland annat hover-information, zoomning, panorering, filtrering, val via legend och animation.

## Bibliotek

- **Pandas** – filtrering och gruppering av data
- **Plotly Express** – interaktiva diagram och animation
- **Matplotlib** – statisk jämförelse

## Starta projektet

1. Öppna `Plotly_Gapminder_Jupyter.ipynb` i Jupyter Notebook, JupyterLab eller Visual Studio Code med Jupyter-tillägget.
2. Välj en Python-kernel.
3. Kör cellerna uppifrån och ned med **Shift + Enter** eller välj **Run All**.
4. Kör installationscellen en gång om biblioteken inte redan är installerade.

Installationscellen använder:

```python
%pip install pandas plotly matplotlib
```

Efter installationen kan Python-kerneln behöva startas om innan notebooken körs från början.

## Källor

- [Plotly Express – officiell dokumentation](https://plotly.com/python/plotly-express/)
- [Plotly – animationer](https://plotly.com/python/animations/)
- [Plotly – inbyggda dataset](https://plotly.com/python-api-reference/generated/plotly.data.html)
- [Pandas – GroupBy](https://pandas.pydata.org/docs/user_guide/groupby.html)
- [Gapminder – data](https://www.gapminder.org/data/)

## Avgränsning

Projektet fokuserar på Plotly och interaktiv datavisualisering. Det innehåller inte avancerad statistik, maskininlärning, externa API:er eller en webbapplikation.
