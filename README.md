# Tandy1000-DMA-Upgrade
 DMA and Memory Upgrade for the Tandy 1000/A/HD models.  This is a clone of the T512CLK-A1 Upgrade by ATD Inc.  It uses no special or programmable logic chips, everything is off-the-shelf 74 series logic and a standard 8237A DMA Controller.
 
 This board also upgrades these machines to 640k in just one slot, instead of requiring two of the original Tandy boards.  This particular project is a direct 1:1 clone of the original PCB, done in Sprint.   I will be working on creating a version in KiCAD with proper schematics as well.
 
 ## Bill of Materials
|Quan |Ref(s)        |Mouser Part Number  |Description                                                     
|-----|--------------|--------------------|----------------------------------------------------------------
| 16  |U1-U16        |n/a                 |DRAM 1x256  (41256 or equivalent)
| 1   |U17           |595-SN74LS139AN     |74LS139 Dual 4 bit Decoder
| 1   |U18           |595-SN74LS08N       |74LS08 Quad AND Gates
| 1   |U19           |595-SN74LS32N       |74LS32 Quad OR Gates
| 2   |U20,U21       |595-SN74LS258BN     |74LS258 Quad 2 to 1 Multiplexer
| 1   |U22           |n/a                 |Custom RTC Module, do not populate
| 1   |U23           |595-SN74LS138N      |74LS138 3 to 8 Demultiplexer
| 1   |U24           |595-SN74LS373N      |74LS373 Octal Latches
| 1   |U25           |n/a                 |8237A DMA Controller
| 1   |U26, U29      |595-SN74LS245N      |74LS245 Octal Bus Transciever
| 1   |U27, U32      |595-SN74LS74AN      |74LS74 Dual Flip-flop
| 1   |U28           |595-SN74LS04N       |74LS04 Hex Inverter
| 1   |U30           |595-SN74LS670N      |74LS670 4x4 Register
| 1   |U31           |595-SN74LS00N       |74LS00 Quad NAND Gates
| 1   |R1            |299-330-RC          |330 Ohm 1/8w Resistor
| 2   |RP1,RP2       |652-4610X-2LF-33    |33 ohm Resistor Pack SIP10 (Isolated)
| 1   |RP3           |652-4608X-1LF-4.7K  |4.7k ohm Resistor Pack SIP8 (Bussed)
| 1   |JP1           |798-A14PA254DSA71   |2x2 Header 2.54mm (or a piece of wire)
| 20  |C1-C20        |581-SA105E104Z      |0.1uF MLCC
| 1   |C21           |647-UMT1H100MDD     |10uF Electrolitic
| 1   |C22           |581-SA102A101JAR    |100pF MLCC

Note:	All 74LSxx series logic ICs can be substituted with any family with "LS" or "T" in the name, such as ALS, ACT, AHCT, or HCT among others.


## Built With

* [Sprint Layout 6](https://www.electronic-software-shop.com/lng/en/electronic-software/sprint-layout-60.html?language=en)

## Authors

* **Rob Krenicki** - [rkrenicki](https://github.com/rkrenicki)

## License

This project is licensed under the GPL 3.0 License