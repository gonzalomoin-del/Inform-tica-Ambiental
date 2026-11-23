# 💻 Contaminación Ambiental e Informática Ecológica (Green IT)
> **Asignatura:** Fundamentos de Hardware — 1.º de ASIR
> **Integrantes:** Gonzalo Morales y Rafael Moreno

---

## 📑 Índice
1. [Impacto indirecto: Consumo energético y huella hídrica](#1-impacto-indirecto-consumo-energético-y-huella-hídrica)
2. [Marco legal y tratamiento de RAEE en España y la UE](#2-marco-legal-y-tratamiento-de-raee-en-españa-y-la-ue)
3. [Obsolescencia programada desde el diseño de hardware y software](#3-obsolescencia-programada-desde-el-diseño-de-hardware-y-software)
4. [Alargar la vida útil de equipos mediante GNU/Linux y hardware modular](#4-alargar-la-vida-útil-de-equipos-mediante-gnulinux-y-hardware-modular)

---

## 1. Impacto indirecto: Consumo energético y huella hídrica
El sector TIC genera cerca del **3,5 % de las emisiones globales**, ya que los equipos domésticos, las redes de telecomunicaciones y los Centros de Procesamiento de Datos (CPD) consumen electricidad y agua de forma ininterrumpida. 

Los CPD evaporan millones de litros de agua dulce al día en sus torres de refrigeración para evitar que los servidores se sobrecalienten; a esto se suma que las centrales eléctricas que generan esa energía también consumen agua y emiten $\text{CO}_2$.

* **Problema 1 — Auge de la nube y la IA:** El crecimiento masivo de estos servicios dispara el consumo eléctrico y agota los recursos hídricos locales destinados a enfriar los servidores.
  * **Solución:** Aprovechar la refrigeración natural (*free cooling*) usando aire frío y ubicar los CPD en países con climas fríos.
* **Problema 2 — Origen de la energía y consumo fantasma:** Gran parte de la electricidad que alimenta la red y el consumo en espera (*standby*) en los hogares sigue proviniendo de centrales térmicas contaminantes.
  * **Solución:** Consolidar servidores mediante virtualización para reducir el número de máquinas físicas activas y alimentar las infraestructuras con energías 100 % renovables.

---

## 2. Marco legal y tratamiento de RAEE en España y la UE
En las plantas de tratamiento autorizadas, la gestión de los Residuos de Aparatos Eléctricos y Electrónicos (RAEE) sigue un proceso estrictamente regulado por fases:

1. **Clasificación y reutilización:** Se evalúa inicialmente si algún equipo puede ser reacondicionado para darle una segunda vida.
2. **Descontaminación manual:** Se extraen componentes peligrosos y contaminantes como baterías de litio, condensadores tóxicos, tóner y mercurio.
3. **Trituración y separación mecánica:** El resto del hardware pasa por procesos de triturado y separación mediante electroimanes, corrientes de Foucault y lectores ópticos que aíslan hierro, cobre, aluminio y distintos tipos de plásticos.
4. **Refinado de metales preciosos:** Las placas base trituradas se envían a refinerías especializadas donde, mediante procesos químicos y térmicos, se recuperan materiales como oro, plata o paladio para reincorporarlos a la fabricación de nueva electrónica.

---

## 3. Obsolescencia programada desde el diseño de hardware y software
¿Qué tanto derecho tienen las empresas a fabricar aparatos que dentro de un tiempo predeterminado dejarán de funcionar? Desde el punto de vista técnico e informático, los fabricantes no suelen programar una «fecha de caducidad» literal en el código, pero sí utilizan el **diseño de ingeniería y las decisiones de arquitectura** para controlar el ciclo de vida útil del hardware. En la práctica, ejercen ese control mediante dos vías principales:

* **Arquitectura cerrada e integración extrema:** Al soldar la memoria RAM, el almacenamiento SSD o incluso el chip de red directamente a la placa base, el fabricante elimina la modularidad del estándar PC e impide reparaciones o ampliaciones sencillas.
* **Control de firmwares y drivers:** Las empresas dominan el software de bajo nivel. Pueden dejar de optimizar controladores para tarjetas gráficas o placas base antiguas, o bloquear mediante firmware el uso de baterías y pantallas de repuesto no oficiales.

---

## 4. Alargar la vida útil de equipos mediante GNU/Linux y hardware modular
Desde la administración de sistemas, la forma más efectiva de combatir la basura electrónica y la obsolescencia programada es extender al máximo la vida útil del equipamiento antes de desecharlo. Esto se logra aplicando dos medidas técnicas fundamentales:

* **Reutilización mediante distribuciones GNU/Linux ligeras:** Cuando un ordenador antiguo deja de recibir soporte oficial o rinde mal con sistemas operativos modernos pesados, su hardware sigue siendo funcional. Instalar distribuciones como **Lubuntu** (con entorno LXQt), **Xubuntu** (con XFCE) o **Debian** sin entorno gráfico reduce drásticamente el consumo de memoria RAM y ciclos de CPU.
* **Compra responsable y hardware modular:** Al renovar equipos, en lugar de adquirir dispositivos cerrados, se debe priorizar hardware modular que permita sustituir o ampliar fácilmente la memoria RAM, el almacenamiento y la batería, eligiendo además componentes con certificaciones ecológicas y de eficiencia energética.
