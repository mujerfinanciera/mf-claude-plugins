# Mapeo categorías Nora → grupos MF

Nora usa el catálogo global de categorías (códigos tipo Plaid). Esta tabla agrupa cada categoría primaria en los grupos del método MF. Las subcategorías (`*_DETAILED`) heredan el grupo de su primaria salvo las excepciones listadas.

| Código Nora (primaria) | Grupo 50/30/20 | Grupo 80/20 | Nota |
|---|---|---|---|
| `RENT_AND_UTILITIES` | Necesidades | Vivir | |
| `FOOD_AND_DRINK` | Necesidades | Vivir | **Excepción:** `FOOD_AND_DRINK_RESTAURANT`, `FOOD_AND_DRINK_FAST_FOOD`, `FOOD_AND_DRINK_COFFEE`, `FOOD_AND_DRINK_BEER_WINE_AND_LIQUOR` → Deseos |
| `TRANSPORTATION` | Necesidades | Vivir | `TRANSPORTATION_TAXIS_AND_RIDE_SHARES` → Deseos si hay transporte público disponible; preguntar |
| `MEDICAL` | Necesidades | Vivir | |
| `GENERAL_SERVICES` | Necesidades | Vivir | **Excepción:** `GENERAL_SERVICES_EDUCATION` y `GENERAL_SERVICES_CHILDCARE` → Necesidades; `GENERAL_SERVICES_STORAGE`, `GENERAL_SERVICES_POSTAGE_AND_SHIPPING` → Deseos |
| `GOVERNMENT_AND_NON_PROFIT` | Necesidades | Vivir | impuestos y trámites; donaciones → Deseos |
| `LOAN_PAYMENTS` | Necesidades (cuota mínima) / Ahorro y deudas (pago extra) | Vivir / Ahorro y deudas | Si no se distingue, va a Necesidades |
| `BANK_FEES` | Necesidades | Vivir | marcar siempre como "gasto a revisar" |
| `ENTERTAINMENT` | Deseos | Vivir | |
| `GENERAL_MERCHANDISE` | Deseos | Vivir | ropa, electrónica, online; `GENERAL_MERCHANDISE_SUPERSTORES` → preguntar (puede ser supermercado) |
| `PERSONAL_CARE` | Deseos | Vivir | `PERSONAL_CARE_HAIR_AND_BEAUTY`, `PERSONAL_CARE_GYMS_AND_FITNESS_CENTERS` → Deseos; farmacia → Necesidades |
| `HOME_IMPROVEMENT` | Deseos | Vivir | reparaciones urgentes → Necesidades; preguntar |
| `TRAVEL` | Deseos | Vivir | |
| `TRANSFER_OUT` | Ahorro y deudas | Ahorro y deudas | solo si el destino es cuenta de ahorro/inversión propia; si no, ignorar (es movimiento, no gasto) |
| `TRANSFER_IN` | — | — | no es ingreso ni gasto; ignorar |
| `INCOME` | Ingresos | Ingresos | |
| `OTHER` | preguntar | preguntar | |

## Reglas

- Ante la duda, **preguntá**, no asumas. La usuaria conoce su vida.
- Mostrá el agrupamiento antes de calcular porcentajes, para que lo corrija.
- Lo que Nora marca como `needsConfirmation` o sin categoría va a "a revisar" y se pregunta.
- Nunca sumes montos en monedas distintas. Si hay más de una moneda, trabajá en la principal y listá el resto aparte.
