# Laadregelaar

## Info component
Regelt het laden van de batterijen vanuit de panelen en beschermt ze tegen overladen.

## Relevante parameters

| Parameter | Betekenis |
|---|---|
| Stroom (A) | Maximale laadstroom |
| Max. ingangsspanning (V) | Moet hoger zijn dan de Voc van de panelenreeks |
| Type | MPPT of PWM |

## Welke types + vergelijking

| Type | Voordelen | Nadelen |
|---|---|---|
| MPPT | Haalt meer energie uit de panelen | Duurder |
| PWM | Goedkoop, eenvoudig | Minder efficiënt, panelenspanning moet passen bij batterij |

## Hoe dimensioneren

1. Stroom ≥ panelenvermogen ÷ batterijspanning × 1,25
2. Controleer de maximale ingangsspanning bij koude ochtenden

**Leveranciers:** zie de [centrale supplier list op Drive](https://drive.google.com/), filter op *PV (zonne-energie)* en het component.
