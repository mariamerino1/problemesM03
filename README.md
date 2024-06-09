# PARSER de docs gencat d'1 cicle a col·leccions mongodb.

## PAS 1. de fitxer txt a fitxers .json

Executar `curr_a_json.py`

Transforma fitxers de text que contenen el llistat de mòduls publicat per gencat en maig de 2024, en fitxers .json que contenen documents 
Per veure detalls:
```
import curr_a_json
help(curr_a_json)
```
Per executar: cal tenie en el mateix directori:

  Aquest .py (curr_a_json.py)
  
  Els fitxers de text pla a processar (fitxers font)
  
    Exemple SMX_curr.txt, ASIX_curr.txt, DAW_curr.txt
    
Aquest .py conté un main() amb els exemples, 
  si es canvia els curriculums a parsejar, canviar el main()
  
**Cal preparar fitxers font (els .txt)**: 
  - Traure capçaleres i peus i guardar en format text (per exemple amb Writer)
  - Comprovar manualment que totes les línies comencen com toca: 
    - moduls, RAs, CAs i continguts en un número seguit d'un punt.
  - A tenir en compte:  Esborrarà totes les línies que tinguin menys de 5 caràcters.

## PAS 2. inserir els docs .json en col·leccions mongodb
Executar `mongo_inserts.py`

Es connecta a la base de dades en server mongodb i crea les col·leccions a partir dels .json que es trobin al directori escollit. (Al exemple d'aquest main "./")

Els .json han de ser tal com s'han obtingut de `cur_a_json.py`. Fa la connexió a partir de **SRV_URI** que **ha d'estar** guardada en un fitxer **.env** al mateix directori que aquest .py

Per veure detalls:
```
import mongo_inserts
help(mongo_inserts)
```
