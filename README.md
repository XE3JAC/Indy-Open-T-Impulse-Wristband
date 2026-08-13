# Indy Open T-Impulse Wristband

```{=html}
<p align="center">
```
`<img src="docs/images/t-impulse-wristband.png" alt="Indy Open T-Impulse Wristband" width="100%">`{=html}
```{=html}
</p>
```
```{=html}
<p align="center">
```
`<strong>`{=html}Tu beacon APRS en la muñeca.`</strong>`{=html}
```{=html}
</p>
```
**Indy Open T-Impulse Wristband** convierte la **LILYGO T-Impulse** en
un beacon APRS portátil, ligero y configurable.

Obtén tu posición mediante GNSS, transmite balizas APRS y consulta la
información más importante directamente desde tu muñeca.

> ⚠️ **Proyecto en desarrollo**\
> Las características, funciones y especificaciones pueden cambiar
> durante el desarrollo y las pruebas.

------------------------------------------------------------------------

## 📡 ¿Qué hace?

Indy Open T-Impulse Wristband está diseñado para transmitir
periódicamente la posición del usuario mediante **APRS sobre LoRa**.

El dispositivo puede mostrar información relevante como:

-   📍 Estado de posición GNSS
-   🛰️ Número de satélites
-   🔋 Nivel de batería
-   📡 Estado de transmisión
-   🕐 Hora obtenida mediante GNSS
-   ➤ Última transmisión realizada

------------------------------------------------------------------------

## ✨ Características

-   Beacon APRS portátil
-   GNSS integrado
-   Comunicación LoRa
-   Configuración personalizada de APRS
-   Intervalos de transmisión según actividad
-   Potencia de transmisión configurable
-   Activación y desactivación de TX
-   Información de batería
-   Hora mediante GNSS
-   Web Flasher para configuración e instalación
-   Diseño portátil y de bajo consumo

------------------------------------------------------------------------

## 🛰️ APRS

La configuración puede incluir:

-   Indicativo APRS
-   Comentario de baliza
-   Intervalo estacionario
-   Intervalo caminando
-   Intervalo conduciendo
-   Potencia de transmisión
-   Activación o desactivación de TX

------------------------------------------------------------------------

## 📻 Perfiles de radio

  Módulo   Radio       Frecuencia
  -------- -------- -------------
  S78G     SX1278     433.775 MHz
  S76G     SX1276     868.200 MHz
  S76G     SX1276     915.000 MHz

> La disponibilidad y utilización de determinadas frecuencias y
> potencias depende de la región y de la normativa aplicable.

------------------------------------------------------------------------

## ⌚ Pantalla

Entre los datos que puede mostrar se encuentran:

-   Hora
-   Indicativo APRS
-   Estado GNSS
-   Satélites
-   Batería
-   Estado TX
-   Última baliza transmitida

El objetivo es ofrecer una interfaz sencilla, clara y adecuada para una
pantalla de muñeca.

------------------------------------------------------------------------

## 🌐 Web Flasher

El proyecto incluye un **Web Flasher** que permite configurar e instalar
el firmware desde un navegador compatible.

El usuario puede seleccionar el perfil de radio, introducir su
configuración APRS y preparar una copia personalizada del firmware antes
de instalarla en el dispositivo.

------------------------------------------------------------------------

## 🔧 Hardware

**Plataforma objetivo:** LILYGO T-Impulse\
**Microcontrolador:** STM32L073RZ

Perfiles contemplados:

-   **S78G / SX1278**
-   **S76G / SX1276**

------------------------------------------------------------------------

## 🥾 Ideal para

-   🏔️ POTA / SOTA
-   🥾 Senderismo
-   🚴 Ciclismo
-   👥 Eventos
-   🚗 Operación móvil
-   📻 Radioaficionados

------------------------------------------------------------------------

## 🚧 Estado del proyecto

**Indy Open T-Impulse Wristband se encuentra actualmente en
desarrollo.**

El hardware, firmware, interfaz y comportamiento pueden cambiar conforme
avanzan las pruebas.

------------------------------------------------------------------------

## 🛠️ Instalación

El método recomendado de instalación es mediante el **Web Flasher**
incluido en este repositorio.

Los archivos del instalador web se encuentran en:

`/webflasher/`

Las versiones publicadas del firmware pueden encontrarse en la sección
**Releases** del repositorio.

------------------------------------------------------------------------

## 🤝 Contribuciones

Este es un proyecto abierto y comunitario. Son bienvenidos los reportes
de errores, pruebas con hardware, mejoras del firmware y Web Flasher,
documentación y pull requests.

------------------------------------------------------------------------

## 🌎 Familia Indy Open

T-Impulse Wristband forma parte del ecosistema **Indy Open**:

-   📡 Indy Open APRS
-   🟧 Indy Open TNC
-   🟢 Indy Open LoRa
-   🟣 Indy Open HamWatch

------------------------------------------------------------------------

## ⚠️ Uso de radiofrecuencia

La transmisión de radiofrecuencia está sujeta a las regulaciones
aplicables en cada país o región.

El usuario es responsable de utilizar frecuencias, niveles de potencia,
indicativos y demás parámetros permitidos por la legislación aplicable y
por su licencia de radioaficionado.

------------------------------------------------------------------------

## 📜 Open Source

**Abierto · Colaborativo · Comunitario**

Indy Open busca desarrollar hardware y software abierto para la
comunidad radioaficionada.

Consulta los archivos de licencia incluidos en este repositorio para
conocer las condiciones aplicables.

------------------------------------------------------------------------

```{=html}
<p align="center">
```
`<strong>`{=html}INDY OPEN`</strong>`{=html}
```{=html}
</p>
```
```{=html}
<p align="center">
```
Tu radio. Tu red. Tu pasión.
```{=html}
</p>
```
