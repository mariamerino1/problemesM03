# problemesM03
# DRAFT model de dades

## Convenis
Una col·lecció per guardar el calendari.
`calendari`
conté les dates dels dies no lectius


Hi ha diverses col·leccions per a cada cicle.
```
- gX_yyy_moduls
- gX_yyy_ras
- gX_yyy_continguts
- gX_yyy_programacio
- gX_yyy_rel_prog_ras
```
`X` és:

  `m` per a cicles de grau mig
  `s` per a cicles de grau superior.

`yyy` són les sigles d'un títol.

Per exemple: `gs_daw_moduls`  

## Exemples de documents.
### gs_daw_moduls
```json
[
    {
        "_id": "0373",
        "modul": "Llenguatges de marques i sistemes de gestió d’informació",
        "durada": 99,
        "hores_centre": 66,
        "hores_empresa": 33,
        "ects": 7
    }
]
```
### gs_daw_ras
```json
[
    {
        "_id": "0373ra1",
        "desc": "1. Reconeix les característiques de llenguatges de marques analitzant i interpretant fragments de codi.",
        "cas": [
            "1.1 Identifica les característiques generals dels llenguatges de marques.",
            "1.x ... criteris d'avaluació",
            "1.9 Identifica els avantatges que aporten els espais de noms."
        ]
    }
]
```
### gs_daw_continguts
```json
[
    {
        "_id": "0373con1",
        "desc": "1. Reconeixement de les característiques de llenguatges de marques:",
        "continguts": [
            "1.1 Classificació.",
            "1.2 Característiques i àmbits d'aplicació.",
            "1.3 Estructura i sintaxi.",
            "1.4 Eines d'edició.",
            "1.5 Elaboració de documents ben formats.",
            "1.6 Utilització d'espais de noms."
        ]
    }
]
```

### gX
