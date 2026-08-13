# ⌚📡 Indy Open T-Impulse Wristband

## Tu beacon APRS en la muñeca.

![Indy Open T-Impulse Wristband](./docs/images/t-impulse-wristband.png)

**Indy Open T-Impulse Wristband** es un proyecto abierto de la familia
**Indy Open**, orientado a convertir la **LILYGO T-Impulse** en un
beacon APRS portátil, ligero y configurable.

El proyecto aprovecha el **STM32L073RZ**, el posicionamiento GNSS y la
radio **LoRa** para transmitir balizas APRS y mostrar en la muñeca
información útil como hora, satélites, batería y estado de transmisión.

> ## 🚧 EL PROYECTO ESTA EN CONTINUO DESARROLLO 🚧
>
> Si quieres seguir la evolución del proyecto, utiliza ⭐ **Star** y 👀
> **Watch** en GitHub para recibir las próximas actualizaciones.
>
> La interfaz y controles descritos corresponden al firmware `v0.1.4` o posterior.

# WEBFLASHER - Indy Open T-Impulse Wristband
# https://xe3jac.github.io/Indy-Open-T-Impulse-Wristband/webflasher

## Manual - Indy Open T-Impulse Wristband
## https://xe3jac.github.io/Indy-Open-T-Impulse-Wristband/

### ZADIG - USB Driver
### https://zadig.akeo.ie/

Toda la configuración es desde el Web Flasher donde puedes seleccionar el perfil de radio, configurar
tus datos APRS y preparar el firmware para instalarlo en la T-Impulse.

------------------------------------------------------------------------

## 🚀 ¿Qué queremos hacer?

Indy Open T-Impulse Wristband busca ofrecer un tracker APRS pequeño y
cómodo para llevar directamente en la muñeca.

Entre las funciones del proyecto se encuentran:

-   📍 Posicionamiento mediante GNSS
-   📡 Envío periódico de balizas APRS
-   🛰️ Número de satélites
-   🔋 Estado de batería
-   🕐 Hora obtenida mediante GNSS
-   ➤ Hora de la última transmisión
-   🚶 Intervalos de baliza según actividad
-   ⚙️ Configuración mediante Web Flasher
-   📻 Comunicación mediante LoRa

------------------------------------------------------------------------

## 📡 APRS

El dispositivo puede configurarse con los siguientes parámetros:

-   Indicativo APRS
-   Comentario de baliza
-   Intervalo estacionario
-   Intervalo caminando
-   Intervalo conduciendo
-   Potencia de transmisión
-   Activación o desactivación de TX

Los parámetros se personalizan desde el Web Flasher antes de instalar el
firmware.

------------------------------------------------------------------------

## 📻 Perfiles de radio

Actualmente se contemplan los siguientes perfiles:

  Módulo   Radio       Frecuencia
  -------- -------- -------------
  S78G     SX1278     433.775 MHz
  S76G     SX1276     868.200 MHz
  S76G     SX1276     915.000 MHz

> La frecuencia y potencia utilizadas deben cumplir con la normativa
> aplicable en cada país o región y con los privilegios de la licencia
> del operador.

------------------------------------------------------------------------

## 🔧 Hardware objetivo

El desarrollo está pensado para:

### LILYGO T-Impulse

Características principales utilizadas por el proyecto:

-   STM32L073RZ
-   GNSS
-   LoRa
-   Pantalla integrada
-   Funcionamiento portátil con batería
-   Conexión USB para configuración e instalación

------------------------------------------------------------------------

## ⌚ Información en pantalla

La interfaz está diseñada para mostrar únicamente la información más útil en el OLED de 64×32 píxeles.

El recorrido de pantallas es circular:

```text
Reloj → GPS → APRS → Batería → Modo → Reloj
```

### 1. Reloj

Muestra la hora local y el indicativo APRS.

```text
09:55 PM
XE3JAC-9
```

### 2. GPS

Muestra el estado del posicionamiento GNSS y el número de satélites.

```text
GPS = FIJADO
8 SATELITES
```

### 3. APRS

Muestra si APRS está habilitado, el total de transmisiones confirmadas desde el encendido y el tiempo estimado para la próxima baliza.

```text
APRS = ON
TX = 15
PROX = 00:15
```

### 4. Batería

Muestra voltaje y porcentaje aproximado calculado mediante ADC.

```text
BATERIA
3.19V 82%
```

> La conversión de voltaje y porcentaje continúa en proceso de calibración con mediciones reales de batería cargada y descargada.

### 5. Modo

Muestra el modo de consumo actual:

```text
MODO
AHORRO
```

Puede mostrar `ACTIVO` o `AHORRO`.

### Controles

- **Toque breve:** cambia a la siguiente pantalla.
- **Doble toque:** alterna entre modo **ACTIVO** y **AHORRO**.
- **Toque largo de 2 segundos:** apaga la pulsera entrando en suspensión profunda.
- Con la pantalla apagada, el primer toque la despierta conservando la pantalla anterior.

### Modos de consumo

| Modo | Pantalla | GNSS |
|---|---|---|
| Activo | Se apaga a los 10 s | Permanece encendido |
| Ahorro | Se apaga a los 5 s | Se suspende para ahorrar energía y despierta periódicamente |


------------------------------------------------------------------------

## 🥾 Ideal para

-   🏔️ POTA / SOTA
-   🥾 Senderismo
-   🚴 Ciclismo
-   👥 Eventos
-   🚗 Operación móvil
-   📻 Radioaficionados

------------------------------------------------------------------------

## ⭐ Sigue el proyecto

Si te interesa Indy Open T-Impulse Wristband:

-   ⭐ Dale una **Star** al repositorio
-   👀 Usa **Watch** para recibir actualizaciones
-   🍴 Haz **Fork** si quieres experimentar
-   💡 Comparte ideas y sugerencias
-   🐛 Reporta errores
-   🤝 Contribuye al desarrollo

Cada colaboración ayuda a que el proyecto siga creciendo.

------------------------------------------------------------------------

## ☕ Apoya el proyecto

Indy Open es un proyecto comunitario desarrollado por interés en la
radioafición, la experimentación y el desarrollo de nuevas herramientas.

Si quieres ayudar a continuar desarrollando, probando hardware y creando
nuevas funciones, puedes apoyar voluntariamente el proyecto.

❤️ **Las donaciones son completamente opcionales.**

[![Donar con
PayPal](https://www.paypalobjects.com/es_XC/MX/i/btn/btn_donateCC_LG.gif)](https://www.paypal.com/donate?hosted_button_id=2RX7AT3HP4RNG)

**¡Gracias por apoyar Indy Open APRS! 73 de XE3JAC**
