# Saw Cut Window

**Demo only.** Prepared by Soheil Heydari.

A browser-based demo for planning control-joint saw cutting on rigid concrete pavements. Enter the slab size, a registered TfNSW R83 mix, the site and the pour date and time. The page fetches the hourly weather forecast and shows:

- the saw-cutting window (when sawing can start without ravelling, and when it should finish before uncontrolled cracking)
- a chart of tensile strength gain against hypothetical early-age stresses for 72 hours after placement
- an hourly table of air temperature, humidity, wind, rain, solar radiation and plastic-shrinkage evaporation rate for 96 hours

**Live page:** https://soheilheydari25.github.io/saw-cut-window/

## Method

- Weather: [Open-Meteo](https://open-meteo.com) forecast and archive APIs (free for non-commercial use, CC BY 4.0), including the Bureau of Meteorology ACCESS models.
- Evaporation rate: Uno (1998) form of the ACI 305 nomograph.
- Strength gain: Arrhenius maturity (equivalent age at 20 °C) with the CEB-FIP strength curve for S35 pavement concrete; tensile strength 0.3 fc^(2/3).
- Stresses: hypothetical thermal-gradient stresses scaled to illustrate the critical cracking time. These are placeholders for a calibrated model.

Not for construction decisions.
