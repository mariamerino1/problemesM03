# problemesM03
# DRAFT model de dades

## Convenis
Una col·lecció per guardar el calendari.
`calendari`
conté les dates dels dies no lectius


Hi ha diverses col·leccions per a cada cicle.

- `prefix_moduls`
- `prefix_ras`
- `prefix_continguts`
- `prefix_programacio`
- `prefix`

El prefix de totes les col·leccions d'un cicle, es crea amb:
`gX_sigles_del_cicle`
`X` és M per a cicles de grau mig i `s` per a cicles de grau superior. 
Per exemple: gs_daw...


## Configuració Tailwindcss
Seguir les instruccion de la [Documentació](https://tailwindcss.tw/docs/guides/vite)
```bash
npm install -D tailwindcss postcss autoprefixer
npx tailwindcss init -p

`

## Afegir Vue Tailwind Datepicker
[Documentació](https://dev.to/elreco/add-a-tailwind-datepicker-to-your-vue-3-application-57j2)

https://vue-tailwind-datepicker.com/
