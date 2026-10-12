# SOLEN — conversion vers InDesign

Conversion des documents SOLEN (Microsoft Publisher / PDF) au format Adobe InDesign.

## Organisation

```
sources/
  publisher/   fichiers .pub d'origine
  pdf/         PDF à convertir (exportés depuis Publisher ou convertis via LibreOffice)
indesign/
  indd/        fichiers InDesign (.indd) + dossier Links/ des images
  idml/        exports IDML (ouvrables dans toutes les versions d'InDesign)
```

## Processus

1. Déposer le fichier source dans `sources/publisher/` ou `sources/pdf/`.
2. Un `.pub` est d'abord exporté en PDF (de préférence depuis Publisher, sinon
   `soffice --headless --convert-to pdf`).
3. Le PDF est converti en InDesign via le service Adobe « PDF → InDesign ».
4. Le résultat est rangé dans `indesign/` sous le même nom que la source.

## Conventions de nommage

`SOLEN_-_DOC_<numéro>_-_<TITRE>` — identique entre la source et le résultat.

## Suivi

| Doc | Source | Pages | Format | InDesign |
|-----|--------|-------|--------|----------|
| 27 — RPM BERGMANN VIII | `sources/pdf/SOLEN_-_DOC_27_-_RPM_BERGMANN_VIII.pdf` (Publisher LTSC) | 4 (A4) | PDF | à faire |
