# Graphite, Materials Data Series #9

An interactive data dashboard and LinkedIn carousel on the most underrated material in the energy transition. People know graphite as pencil lead. Its real job is the anode in every lithium-ion battery, the largest mineral by mass in an EV pack, and one country makes almost all of the battery-ready grade.

Part of my Materials Data Series, where I take one material at a time and tell it as a materials engineer who works in data. Steel, aluminium, copper, rare earths, lithium, nickel, cobalt and titanium came first. Silicon is next.

**Live dashboard:** _(deploy `index.html` to Netlify/GitHub Pages)_

---

## What's inside

| File | What it is |
|------|-----------|
| `index.html` | Interactive Chart.js dashboard, 5 tabs: Production & Geography (with a highlighted world map), What 3 Mt Looks Like, Pencils to Power, The China Factor, Why It Matters |
| `fetch_data.py` | Reproducible Python pipeline that compiles the cited figures into `data/*.csv` |
| `data/*.csv` | Tidy datasets (mine production, reserves, the China chain, natural vs synthetic, end uses, battery minerals, price, scale) |
| `carousel/index.html` | 9-slide LinkedIn carousel (1080x1080) |
| `Graphite_Materials_Carousel.pdf` | Exported carousel, ready to upload |
| `linkedin-post.txt` | Post caption, with the LinkedIn document title and GitHub slug at the top |

## Reproduce the data

```bash
python fetch_data.py      # writes data/*.csv
```

The dashboard embeds the same numbers in JS so it runs from `file://` with no server.

## What the data shows

- The world mines about **1.63 Mt of natural graphite** a year and bakes a similar amount of **synthetic graphite** from petroleum coke. Counting all uses, roughly **two-thirds is synthetic**, made rather than mined.
- Graphite is the **anode in every lithium-ion battery**, and the **largest mineral by mass in an EV pack** at around **100 kg**, more than the nickel, cobalt, manganese and lithium combined (about 59 kg). That is roughly **250,000 pencils' worth** of graphite per car.
- **Batteries are now the largest single use** at about **28%** of demand, up from almost nothing a decade ago and projected near **62% by 2036**. Refractories and steelmaking are the traditional anchor.
- **China dominates the chain, and the grip tightens downstream:** about **78% of mining**, **90% of processing**, **93% of anode material** and **99% of spherical (battery-ready) graphite**. It holds only about **30% of reserves**, so the advantage is industrial, not geological.
- The bottleneck is **processing, not scarcity**. Turning flake into 99.95% pure spherical graphite is the hard step. In **December 2023** China placed graphite under **export licensing**, and flake exports fell about a quarter the next year.

## Sources

USGS Mineral Commodity Summaries 2025, the Graphite (Natural) chapter (mine production, reserves, prices, end uses). Supply-chain shares for processing, anode material and spherical graphite from Benchmark Mineral Intelligence, IDTechEx and the IEA.

Mine output in kt and Mt; reserves in Mt. End-use and natural-versus-synthetic shares are approximate 2024 estimates. Battery-mineral masses are typical EV-pack values and vary by chemistry. Spherical-graphite prices are indicative market levels. Figures rounded and attributed.

---

*Built by Ibtisam Ahmed Khan · June 2026 · [linkedin.com/in/ibtisam-ahmed-khan](https://linkedin.com/in/ibtisam-ahmed-khan)*
