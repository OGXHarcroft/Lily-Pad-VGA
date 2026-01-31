# Lily Pad VGA

This is a low cost, reasonably easy to assemble VGA, analog audio, and S/PDIF digital audio breakout box for original Xbox. A 1.0-1.4 Xbox console with a VGA patched BIOS is required. VGA mode is not currently supported on 1.6 Xbox consoles. VGA mode is experimental and some displays will not work with a a VGA signal from a Xbox. The embedded video sync separator is intended for SD and ED resolutions. While it may work with 720p and 1080i video modes, they are not recommended of supported.

Multiple BOM files are included and many links for components can be found at the bottom of this page.

![Product Image](img/product.png?raw=true "Product Image")


### PCB Ordering Details

[Latest Gerbers](https://github.com/OGXHarcroft/Lily Pad VGA/releases/latest)
The included gerber files should work with most PCB board houses, but Eagle board files are included if you need to generate new gerbers for your specific board house.

When ordering from JLC PCB the default options are ideal. Board thickness should be 1.6mm.
JLC PCB assembly files are included for all surface mount components. There is a BOM file for the remaining through hole components aside from the S/PDIF fiber transmitter.

![Product Image](img/LilyPad.png?raw=true "Lily Pad Image")

### Part Ordering Information

Additional Materials Required Depending on Your BOM:
- 4x U.FL (aka I-PEX MHF) 2mm diamter terminated coaxial cables at least 15cm long (included in Digikey BOM)
- 4x M3 16mm machine screws (included in Digikey BOM)
- 4x M3xL4xOD4.5mm brass inserts (not included in any BOM)
- 1x Xbox AVIP connector (not included in any BOM)

Optional But Recommended Components:
- GQ-1504 S/PDIF fiber optic transmitter
- the 3D printed case, retention clip, case screws and brass inserts
- XD-08 cable gland for strain relief
- 20-30cm of 4-6mm braided cable sleeving
- Zip tie for strain relief
- heat shrink to make the braided cable sleeving easier to deal with
- Additional wire for strain relief


### Basic Assembly Instructions and Advice

1) Assemble the AVIP connector wire harness with the 4 U.FL terminated coaxial cables and the 5 pin 1.25mm picoblade cable using the image below. The shielding on the cables can be directly soldered to the ground pin for each signal line. An extra piece of wire should be added as extra strain relief to protect the picoblade wires and coaxial cables, and will offer some extra grounding for static discharges. The added piece of wire can be soldered directly to the shielding of the AVIP connector and to the extra plated through hole on the board to the right of J2, and then through the same sleeving and cable glands as the rest of the wire harness. Ensure this cable is the shortest wire in the harness for proper strain relief. Coloring the U.FL connectors with marker to denote signal they carry may be helpful. Make sure you put the AVIP connector boot and cable glad onto the wire harness before soldering the wires to the pins on the connector. Adding a small piece of heat shrink on each end of the sleeving will help the sleeving stay in place. Adding a zip tie on the adapter side of the cable gland will help with strain relief.

![AVIP Image](img/AVIP_connector_pinout.png?raw=true "AVIP Image")

2) Assemble the PCB with components from the various BOM files and links below. The S/PDIF transmitter (J4) is difficult to find outside of ebay, aliexpress, alibaba etc. Aside from the 3D prints, every component can be purchased from Aliexpress. BOM and CPL files for PCB assembly at JLC PCB for all surface mount components are included in this repo. Trimming the longest legs off the audio and S/PDIF connectors will aid in the best fit for the case. Several BOM files are included in this repo; please read the title of each one carefully for the components you require.

3) Connect the 5 pin cable to J2, connect the Red, Green, Blue and SPDIF U.FL cables to their correspdonding connectors on the mainboard. Insert the retention clip in the holes on either side of the connectors with the slim side pointing up. Then melt the pegs that protrude through the back of the PCB to permanently affix the retention clip to the board at 180-200C. Alternatively a twist tie passed through the back of the board can help retain the signal wires.

4) For case assembly, place the smooth end of one of the brass standoffs into each of the 4 holes on the inside of the top half of the case, then melt them into place at a safe temperature for the plastic your case was printed with. Generally 180-200C should be sufficient). After placing the adapter board into the bottom half of the case, make sure to slot the cable glad into the provided slot.


### Links For Components

- Xbox AVIP connector:
https://console5.com/store/microsoft-xbox-av-multi-out-plug-for-custom-rgb-cables-repair-og-original.html
or https://www.aliexpress.com/item/1005005195913174.html
- GQ-1504 S/PDIF transmitter (transmitting): https://www.aliexpress.com/item/1005004654447952.html
- J2 audio connector alternate: https://www.aliexpress.com/item/1005001528210520.html
- M3 16mm screws alternate (6mm): https://www.aliexpress.com/item/1005007188294590.html
- M3xL4xiD4.5mm brass threaded inserts: https://www.aliexpress.com/item/1005006071488810.htm (could not find on digikey)
- DSub15 alternate: https://www.aliexpress.com/item/1005003798059447.html
- DSub15 jackscrew: (outside thread 5mm) https://www.aliexpress.com/item/4000371838126.html
- U.FL terminated coaxial cables: https://www.aliexpress.com/item/1005009463616815.html
- 5 pin 1.25mm picoblade cable: https://www.aliexpress.com/item/1005007277110532.html
- Cable gland (choose XD-08-Black): https://www.aliexpress.com/item/1005005691860036.html 
- braided cable sleeving: https://www.aliexpress.com/item/1005007486025295.html


### Thanks and Credit

- Kekule for helpful ideas.
- DiscoStarSlayer for helpful advice.
- HoneySoakedSeagull for the frog art.
- Derf for another great project name.
- Team Cerbios for adding VGA support into their BIOS.