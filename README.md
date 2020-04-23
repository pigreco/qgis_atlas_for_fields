# QGIS Atlante per campi -- in lavorazione

Generare un atlante per campi / Generate an atlas for fields

<!-- TOC -->

- [QGIS Atlante per campi -- in lavorazione](#qgis-atlante-per-campi----in-lavorazione)
  - [Perché questo repository](#perch%c3%a9-questo-repository)
  - [layer nella TOC](#layer-nella-toc)
  - [espressione copyright progetto QGIS](#espressione-copyright-progetto-qgis)
  - [progetti QGIS](#progetti-qgis)
  - [Riferimenti](#riferimenti)
  - [Licenza](#licenza)

<!-- /TOC -->

## Perché questo repository

Per documentare un esempio poco noto di Atlas per campi. L'atlante di **QGIS** si basa sulla definizione del `layer di copertura` e crea tante pagine quante sono le feature del layer. **QGIS** permette di utilizzare, come Coverage layer, anche semplici tabelle senza geometria come il caso in esame.


![](./imgs/img_01.png)



## layer nella TOC

nome file | layer rinominato nella TOC | usato per
----------|----------------------------|----------
`covid19-andamento_nazione.vrt` | `andamento_nazionale`| alimentare il grafico nell'Atlas
`incidenza1k_totale_casi_prov_pivot_dw.csv` | `incidenza1k`| mettere in JOIN con `province`
`totale_casi_prov_pivot_dw`|`totale_casi`| mettere in JOIN con `province`
`province_ita` | `province`| visualizzare i vettore tematizzati
`regioni_ita_mod` | `regioni`| visualizzare i confini regionali
`atlas_pagename`|-|alimentare il `Layer di Copertura`

## espressione copyright progetto QGIS

```
by Totò FIANDACA
QGIS - [%@qgis_version%]
© Fonte dati: PCM-DPC - Confini ISTAT
```

## progetti QGIS

- `progetto_base.qgs` - progetto con solo i layer caricati - EPSG progetto 3857;
- `progetto_atlas.qgs` - progetto con atlas per campi - EPSG progetto 3857.

## Riferimenti

- [QGIS](https://qgis.org/it/site/)
- [data.word](https://data.world/)
- [Notepad++](https://notepad-plus-plus.org/downloads/)
- [Visual Studio Code](https://code.visualstudio.com/)

## Licenza

**CC BY-SA 4.0** [visualizza licenza](https://creativecommons.org/licenses/by-sa/4.0/deed.it)