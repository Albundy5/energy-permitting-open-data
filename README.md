# Energy permitting open data: Greece and Italy

Machine-readable copies of the reference tables published in the permitting guides at [ariadnelabs.eu](https://ariadnelabs.eu/). Each table states public law (deadlines, guarantee amounts, grid connection priority rules, the regional implementation of Italy's aree idonee) with the provision it comes from. Every file names the guide page it was taken from; that page is the edition of record and carries the sources, the date the provisions were checked and the full explanation.

## Datasets

| File | What it holds | Language | Rows | Source page |
|---|---|---|---|---|
| `greece/renewables-permitting-calendar-greece` | Producer Certificate filing cycles, supplementary-information deadlines, and the validity of the Final Connection Offer, the environmental terms decision (ΑΕΠΟ) and the Installation Licence | English | 8 | [Renewables permitting calendar, Greece](https://ariadnelabs.eu/guides/renewables-permitting-calendar-greece.html) |
| `greece/imerologio-adeiodotisis-ape` | The same calendar, Greek original | Greek | 8 | [Ημερολόγιο αδειοδότησης ΑΠΕ](https://ariadnelabs.eu/el/odigoi/imerologio-adeiodotisis-ape.html) |
| `greece/grid-connection-priority-groups-greece` | How ΑΔΜΗΕ and ΔΕΔΔΗΕ rank connection requests: the decision in force, the groups, the order within a group, the storage tracks | English | 8 | [Grid connection priority groups, Greece](https://ariadnelabs.eu/guides/grid-connection-priority-groups-greece.html) |
| `greece/omades-proteraiotitas-syndesis` | The same rules, Greek original | Greek | 8 | [Ομάδες προτεραιότητας σύνδεσης](https://ariadnelabs.eu/el/odigoi/omades-proteraiotitas-syndesis.html) |
| `greece/letters-of-guarantee-renewables-greece` | Each letter of guarantee on a renewable or storage project's route: amount, return or forfeiture, provision | English | 7 | [Letters of guarantee, Greece](https://ariadnelabs.eu/guides/letters-of-guarantee-renewables-greece.html) |
| `greece/engyitikes-epistoles-ape` | The same table, Greek original | Greek | 7 | [Εγγυητικές επιστολές ΑΠΕ](https://ariadnelabs.eu/el/odigoi/engyitikes-epistoles-ape.html) |
| `italy/aree-idonee-by-region-italy` | Region by region: the state of aree idonee legislation, the act with its publication and entry into force, and a link to the official text | English | 21 | [Aree idonee by region](https://ariadnelabs.eu/guides/aree-idonee-by-region-italy.html) |
| `italy/aree-idonee-regioni` | The same matrix, Italian original | Italian | 21 | [Aree idonee, regione per regione](https://ariadnelabs.eu/it/guide/aree-idonee-regioni.html) |

Each dataset comes as CSV (UTF-8 with BOM, so Excel opens Greek and accented text correctly) and as JSON. The JSON carries the name, description, language, source page, `dateModified` and licence, then one object per row keyed by the column headings. Where a table cites official texts, a final column lists their links.

## How current it is

The files are regenerated from the guide pages whenever a guide changes, and this repository is synced from them weekly. `dateModified` in each JSON file is the date of the guide's last substantive change. Laws change: before relying on a row, open the source page and the official text it cites. Only the official publication is authoritative.

## Licence and attribution

[CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) (full text in `LICENSE`). Reuse, including commercial reuse, is free with attribution, for example:

> Source: Ariadne Labs, ariadnelabs.eu, "Letters of guarantee in Greek renewables and storage permitting", CC BY 4.0.

The tables summarise provisions for information and are not legal or technical advice on a specific project.

## About

Maintained by [Ariadne Labs](https://ariadnelabs.eu/about.html), which builds MitOS, permitting and project-controls software for energy infrastructure. Corrections are welcome as issues on this repository.
