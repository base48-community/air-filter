# Air Filter

Air Filter implementation in the Hackerspace

## Terminology

* Ultra-Fine Particles ("UFP"): Airborne particles smaller than 0.1 microns (\(<100\text{\ nm}\)) in diameter. They are a major component of air pollution, stemming from traffic and industrial combustion, and are considered highly dangerous to health because they can enter the bloodstream.
* Volatile Organic Compounds ("VOC"): Large group of carbon-based chemicals that easily evaporate at room temperature, turning into gases. They are emitted by thousands of everyday products—such as paints, varnishes, cleaning supplies, new furniture, and carpets—and often accumulate in indoor air, where levels can be 2 to 10 times higher than outdoors. 
* Particulate Matter ("PM"): Indication of the particles per size infused in the air


## Motivation

Improve the currently very poor air quality in the hackerspace with these known air pollutants:
    * FDM 3D Printers: UFP, VOC
    * SLA 3D printers: VOC
    * Wood Workshop: UFP, fine and large particles
    * Metallurgy: UFP, VOC
    * Smoking: Obvious..
    * Chemical Laboratory: "All kinds"

Based on data from home assistant which only tracks particulate matter the in-door air is unhealthy, likely carcinogenic and poses health risk to members who are more sensitive to air quality due to various medical conditions.

## How to Filter the Air?

Ultra-Fine Particles can be filtered via HEPA Filter.

Volatile Organic Compounds can be absorbed into activated carbon, that importantly(!) wasn't treated with acid.

## Acid-Impregnated Activated Carbon

it is designed to target specific inorganic gases, not the diverse, low-level Volatile Organic Compounds (VOCs) and odors that typical air purifiers are designed to remove, thus not good option for our implementation.

## Projected Implementation

### Corsi-Rosenthal Box

![](./img/CR-Box.png)

https://en.wikipedia.org/wiki/Corsi–Rosenthal_Box

Is a popular DIY design, that requires minimal amount of engineering to implement, but depends on big box fan which is often expensive, but we could use 3x3 grid of avilable high flow low noise (if ran on low RPM) fans to mitigate this cost.

Requires MERV 13 furnace filters made for AC, it's important to pick one that has low air restriction for the most effectiveness.

HELP_WANTED: It's unknown which MERV 13 Furnace filter to use that would be sufficiently economical and had the expected effective use that's ideally washable as the one-time-use can get very expensive in comparison..
