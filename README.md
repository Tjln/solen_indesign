# SOLEN — conversion vers InDesign

Conversion des documents SOLEN (Microsoft Publisher / PDF) au format Adobe InDesign.

## Organisation

```
sources/pdf/                PDF d'origine (exportés depuis Publisher)
indesign/<nom du doc>/      fichier .idml + toutes ses images (même dossier)
```

## Ouvrir un document dans InDesign

1. Télécharger le dossier `indesign/<nom du doc>/` en entier (le .idml et les images).
2. Ouvrir le `.idml` dans InDesign. Si des liens apparaissent manquants :
   panneau **Liens** → **Rééditer le lien** → pointer vers ce dossier (tout se relie d'un coup).
3. Enregistrer sous en `.indd`.

Polices nécessaires sur le poste : Arial, Arial Rounded MT Bold, Calibri (fournies avec Office).

## Processus

1. Exporter le document en PDF depuis Publisher, le déposer dans `sources/pdf/`.
2. Conversion PDF → InDesign via le service Adobe.
3. Corrections automatiques des défauts connus de la conversion (voir ci-dessous).
4. Les petits décalages restants se règlent à la main dans InDesign.

### Défauts connus de la conversion Adobe (corrigés automatiquement)

- Police Arial Rounded MT Bold enregistrée sous un nom erroné (`ArialRoundedMTBold`) → renommée.
- Fonds de couleur derrière certains titres perdus → recréés.

## Suivi

| Doc | Pages | État | Reste à faire à la main |
|-----|-------|------|-------------------------|
| 27 — RPM BERGMANN VIII | 4 (A4) | converti + corrigé | vérifier titres, intertitres et textes des encadrés « Économie d'élimination » (p. 2), bloc adresse (p. 4) |
