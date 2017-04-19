# hifive1_tutorials
Tutoriales y cosas interesantes que hacer con una HiFive1 de SiFive

## ¿Qué y porqué?
La placa HiFive1 de la empresa SiFive es una placa de demostración de los chips open-source de tipo RiscV. La placa tiene un formato similar al de un Arduino UNO, y también puede ser programada utilizando el Arduino UNO.

Me parece importante el apoyar a chips abiertos, dado que tiene un potencial para innovación e integración mucho más grande que los chips actuales los cuales están absolutamente plagados de acuerdos como NDAs, y montos a pagar por la supuesta PI (propiedad intelectual) que hoy en día debería estar más que obsoleta.

Por eso en esta guía explicamos como comenzar a utilizar la tarjeta con el IDE de Arduino y algunos ejemplos interesantes de código.

## Instalación

Para mayor facilidad, esta guía incluye los pasos desde la línea de comando, para instalar los módulos necesarios para el IDE de Arduino, así como también una receta de Ansible la cual puede usarse para instalar los módulos necesarios de forma automática en varios equipos, con muy poca interacción.

### Instalación manual (recomendada)

Necesitas tener ya instalado el IDE de Arduino, y luego debes ejecutar estos comandos:
```bash
arduino --pref boardsmanager.additional.urls=http://static.dev.sifive.com/bsp/arduino/package_sifive_index.json --save-prefs
arduino --install-boards sifive:riscv
```
