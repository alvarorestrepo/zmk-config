# Blank Slate Keyboard

Un teclado ortolineal de 4x12 (similar al Planck) con conectividad inalámbrica Bluetooth usando el microcontrolador NRF52840.

## Características

- Matriz de 4 filas x 12 columnas
- Soporte para Bluetooth 5.0
- Monitoreo y reporte de batería
- Modo de ahorro de energía (deep sleep)
- Múltiples perfiles Bluetooth (hasta 5 dispositivos)
- Compatibilidad USB-C
- Macros personalizables
- Capas múltiples para diferentes funciones
- Homerow mods para mayor eficiencia de escritura
- Tap-dance para funcionalidades duales en misma tecla

## Hardware

Este teclado utiliza un microcontrolador NRF52840 con las siguientes características:
- Bluetooth 5.0
- Bajo consumo de energía
- Sensor de batería incluido
- 48 teclas en total (matriz 4x12)

## Mapeo de Teclas

El teclado incluye:
- Capa base QWERTY (DEFAULT)
- Capa de números y navegación (LOWER)
- Capa de símbolos y funciones Bluetooth (RAISE)
- Capa de ajustes para configuración del sistema (ADJUST)

## Comandos Útiles

Para compilar el firmware:
```
west build -p -b nice_nano_v2 -- -DSHIELD=blank-slate
```

Para generar el archivo UF2:
```
west build -p -b nice_nano_v2 -- -DSHIELD=blank-slate -DZMK_CONFIG="$(pwd)/config"
```

## Características Adicionales

- Homerow Mods: Permite que las teclas de la fila base actúen como modificadores cuando se mantienen presionadas
- Macros programadas para texto frecuente
- Combos para acceder a funciones especiales
- Soporte para reinicio/bootloader 