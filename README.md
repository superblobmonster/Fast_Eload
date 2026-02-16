# Fast_Eload
Designed in KiCad 9.0.7 and FreeCAD 1.0.2
## Design Specs
+ 10A/us slew rate
+ 15A RMS, 50A peak, 20A fuse
+ 100W (To be verified) average, peak power limited by FET SOA.
+ 100V input, 150V TVS protection, 250V+ rated parts.
+ 10V external power supply

## Design notes
+ Produce with 2oz copper
+ Fill and cap vias, or plate solid
+ Thinner PCB the better for thermal performance
+ Turn-off slew rates > 15A/us causes instability, root cause unknown

## Parts
+ CCA BOM: https://www.digikey.com/en/mylists/list/430F3M7L10

Additional parts/accessories:
+ Copper shim-stock: https://www.mcmaster.com/products/metals/copper-2~/shape~sheet/thickness~0-032/thickness~0-040/thickness~0-04/
+ TIM
+ Ring terminals
+ M3x4 screws
+ Amphenol MMCX to BNC: 095-850-207-006
+ Tektronix probe tip adaptor to BNC: 13036700
+ Ribbon cable assembly: 71600-308LF

## TODO and Notes
+ Validate thermal performance
+ Measure control bandwidth
+ Create control board with:
  + 10MS/s DAC
  + Slew rate limiting
  + SOA protections
  + V/I Monitoring: ADS7253?, Unregulation detection
  + Isolated input signal, 10MS/s ADC
  + Paralleling features, enable controls
+ Add temperature monitoring
+ Heatsink and interface design for equipment rack enclosure
+ Design a fully electrically isolated THT version with a SOT-227 FET
