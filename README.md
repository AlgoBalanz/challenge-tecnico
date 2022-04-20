# Challenge Técnico

## :sparkles: Objetivo

El challenge técnico consiste en desarrollar una pantalla como la siguiente:

![Pantalla a desarrollar](https://via.placeholder.com/468x300?text=Pantalla+a+desarrollar)

## :page_facing_up: Datos

Para obtener la información se utilizará el MarketData que brinda la API y WebSocket de Binance.

API
```
https://binance-docs.github.io/apidocs/spot/en/#market-data-endpoints
```

WebSocket
```
https://binance-docs.github.io/apidocs/spot/en/#websocket-market-streams
```

---

Los pares que se deberán utilizar son los siguientes:


|         |           |          |          |          |
|---------|-----------|----------|----------|----------|
| BTCBUSD | ETHBUSD   | BNBBUSD  | LUNABUSD | SOLBUSD  |
| LTCBUSD | MATICBUSD | AVAXBUSD | XRPBUSD  | BUSDUSDT |


>El CCL que se deberá usar es 200 (constante)

## :hammer_and_wrench: Cálculos

En pantalla se deberá mostar la cotización en `ARS` de cada una de las criptomonedas. 

Tomando como ejemplo `BTCBUSD`, se deberá mostrar la cotización de `BTC` en `ARS` usando la siguiente formula:

```
BTC/ARS = 1° PRECIO en ASK de BTC/BUSD * CCL
```

---

Para el caso especial de `BUSDUSDT`, se deberá mostrar la cotizacion de `USDT` en `ARS` usando la siguiente formula:

```
USDT/ARS = (1 / 1° PRECIO en BID de BUSD/USDT ) * CCL
```

---

Las cotizaciones se deberán mostrar REDONDEADAS a 4 decimales.