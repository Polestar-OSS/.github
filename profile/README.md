# Polestar OSS

[![Website](https://img.shields.io/badge/Website-polestar--oss.github.io-ff7500)](https://polestar-oss.github.io/)
[![License: AGPL-3.0](https://img.shields.io/badge/License-AGPL--3.0-blue.svg)](https://github.com/Polestar-OSS/polestar-journey-log-explorer/blob/main/LICENSE)

**Community-built, open-source tools for Polestar owners. Your car, your data, your browser.**

Everything here runs as a static site in the browser. Nothing is uploaded, there is no
account and no server. The only optional third party is a visit counter that stays off
until you accept it.

🌐 **https://polestar-oss.github.io/**

## Tools

### Journey Log Explorer

Drop the monthly exports from Polestar's Journey Log app and read your year: overview,
charts, insights, a map with replay, and what the same driving would have cost in petrol.

- **Open it**: https://polestar-oss.github.io/polestar-journey-log-explorer/
- **Source**: [polestar-journey-log-explorer](https://github.com/Polestar-OSS/polestar-journey-log-explorer)
- **Docs**: [docs/](https://github.com/Polestar-OSS/polestar-journey-log-explorer/tree/main/docs), including every formula and an ADR per decision

What it does:

- Three experience levels: Simple, Detailed, Expert, with a built-in help guide.
- Every chart has a table twin, one y-axis and at most three colours.
- Insights with evidence: seasonality only when your data covers the seasons, hemisphere-aware.
- Map with trips, heat and day-linked routes; replay a trip or a range of days from 0.2× to 10×; opt-in road snapping.
- Electricity tariffs: flat, time-of-use, tiered or seasonal. Presets for Hydro Ottawa, Toronto Hydro, every Canadian province, every US state, the UK, Sweden and the EU, each citing its source. Any currency.
- Against petrol and hybrid: Volvo S60, V60, XC60, S90, V90 and XC90, petrol or plug-in hybrid, from EPA fuel-economy data, with CO₂ and trees.
- Merge several exports and remove duplicates.
- Journeys persist in your browser (IndexedDB); export them back as a CSV in the Journey Log format, export or import settings, wipe everything with one confirmed click.
- Metric or imperial, dark or light, reduced motion respected, built for phones.

## Principles

- **Privacy by design.** Static sites, no backend. Journey data never leaves the browser. Real exports and screenshots of them never enter a repository.
- **Real data only.** No placeholder numbers. Tariffs cite their regulator or utility, fuel prices cite StatCan, the EIA or DESNZ, comparison cars come from EPA data, and the method is written down.
- **AGPL-3.0.** Copyleft, including over a network. Fork it, host it, improve it, and share the source of what you ship.
- **One repository per tool.** Each owns its code, tests, pipeline, infrastructure and docs, driven by a Makefile that CI calls.

## Contributing

Issues and pull requests are welcome in each tool's repository. Read its `CONTRIBUTING.md`
and `docs/ARCHITECTURE.md` first; `make check` runs what CI runs. Have an idea for another
tool? [Open an issue](https://github.com/Polestar-OSS/polestar-journey-log-explorer/issues).

- [Explorer issues](https://github.com/Polestar-OSS/polestar-journey-log-explorer/issues)
- [Website issues](https://github.com/Polestar-OSS/polestar-oss.github.io/issues)

## Disclaimer

Polestar is a trademark of Polestar Holding AB. This organisation is an independent
community project and is not affiliated with, endorsed by or connected to Polestar or any
of its subsidiaries.
