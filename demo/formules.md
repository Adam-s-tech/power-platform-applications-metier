# Formules Power Fx · démo minimale

> Démo générique. Source : liste SharePoint `PiecesAeronautiques`.

## Total des pièces

```powerfx
CountRows(PiecesAeronautiques)
```

## Pièces bloquées

```powerfx
CountRows(Filter(PiecesAeronautiques, statut = "Bloqué"))
```

## Pièces en cours

```powerfx
CountRows(Filter(PiecesAeronautiques, statut = "En cours"))
```

## Filtre par site

```powerfx
Filter(PiecesAeronautiques, site = ListeSites.Selected.Value)
```

Ces quatre formules suffisent pour un tableau de bord de démonstration.
Elles n'utilisent ni Dataverse, ni AI Builder, ni connecteur premium.
