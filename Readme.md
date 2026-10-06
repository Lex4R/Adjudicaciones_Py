# Proyecto-Data Science sobre Adjudicaciones del Paraguay

## Datos (no incluidos en git por su peso)
Descargar de https://www.contrataciones.gov.py/datos/data y colocar en `datos_completos/`:

- `awards.csv` (adjudicaciones, base del análisis)
- `con_amendments.csv` (enmiendas, de acá sale el target)
- `contracts.csv` (solo puente award→contrato)
- `awa_suppliers.csv` (RUC proveedor)
- `ten_lots.csv` (agregado de lotes por proceso)
- `records.csv` (variables del llamado: método, categoría, montos, plazos, fechas)

El resto de los CSV del portal no se usa. Cada año pesa ~250MB; agregar más años es copiar los mismos 6 archivos del corte correspondiente.

## Reproducción
1. Colocar los 6 CSV en `datos_completos/`.
2. Ejecutar `Fase1_Etapa2_Etapa3.ipynb` de principio a fin genera `output/dataset_final.csv`.
3. En las fases siguientes usaremos solo `output/dataset_final.csv`, sin necesidad de los datos crudos.
