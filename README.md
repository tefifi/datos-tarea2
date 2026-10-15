# Datos Tarea 2 - Ingeniería de Software

Copia de los valores de UF y dólar observado del año 2026, obtenidos desde mindicador.cl el 14 de octubre de 2026, para quienes no puedan consultar la API.

## Archivos

| Archivo | Contenido |
|---|---|
| `uf-2026.json` | Unidad de fomento (UF), un valor por día, del 2026-01-01 al 2026-11-09 |
| `dolar-2026.json` | Dólar observado, un valor por día hábil, del 2026-01-02 al 2026-10-14 |

## Formato

Es el mismo formato que entrega mindicador.cl para una consulta por año:

```json
{
  "version": "1.7.0",
  "autor": "mindicador.cl",
  "codigo": "uf",
  "nombre": "Unidad de fomento (UF)",
  "unidad_medida": "Pesos",
  "serie": [
    { "fecha": "2026-09-01T04:00:00.000Z", "valor": 40875.09 }
  ]
}
```

## Notas

- El dólar observado no tiene valor en fines de semana ni feriados, por lo que esas fechas no aparecen en `dolar-2026.json`.
- La UF tiene valor todos los días.
