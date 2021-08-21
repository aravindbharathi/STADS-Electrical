# Multilayer PCB Design Documentation

[Original Google Doc](https://docs.google.com/document/d/11V8R4Qwv2B22nqZ2oEq-6VUJGhk6oecQe_GyAkEhjhQ/edit)

> 13-07-2021 (Discussion with Aravind and Rateesh)
1. Avoid having traces in top layer below the Microprocessor
2. Try to have traces originating from the centre of the microprocessor pins and going straight away from the pins.
3. You can mount components on the lower layer for many applications as it gives more freedom.
4. Try to have uniform distance between traces.
5. Try to keep a minimum number of turns in a trace.
6. Avoid vias below microprocessors.
7. Avoid 90degree turns.
8. Keep fine tuning placement and orientation while routing 

## Multilayer PCBs

- Benefits: Higher component density, smaller size, higher flexibility, EMI shielding
- EMI Shielding in electronic devices and equipment is the use of manufacturing techniques and materials to protect signals from being disrupted by external electromagnetic signals as well as preventing generated signals from interfering with surrounding components

- Configure multilayer PCB In Eagle: Go to DRC---> Layers, change number of layers to desired. 
- Now add new via types:
  - Top to bottom(Through)
  - Top to inner(Blind)
  - Inner to inner(Buried)

To rename a layer go to layers in top left of Eagle and rename.
Our PCB will be mostly manufactured by PCBPower, keep checking their blogs and have a detailed idea about their manufacturing constraints before designing the PCBs.


- Netclass: Can make different netclasses in eagle which specify minimum trace width clearance and other properties. Now we can assign the different connections to one of these net classes and the DRC or autorouter will keep those rules in mind.

- Skew: Two different components receiving clock signals at different time due to difference in trace lengths from the microcontroller
[How to Prevent Clock Skew in PCB Design](https://resources.pcb.cadence.com/blog/2019-how-to-prevent-clock-skew-in-pcb-design)

Some good routing practices: [https://www.protoexpress.com/blog/best-high-speed-pcb-routing-practices/](https://www.protoexpress.com/blog/best-high-speed-pcb-routing-practices)

- Impedance matching : Attempt to have source and load impedance to be complex conjugate of each other in order to achieve maximum power transfer [Why is Impedance Matching Important? Impedance Matching Fundamentals | Advanced PCB Design | Cadence](https://resources.pcb.cadence.com/blog/2019-why-is-impedance-matching-important-impedance-matching-fundamentals)

Fan out:
- [How to fanout a BGA - Altium Designer (AD20)](https://www.youtube.com/watch?v=1A9XDI18pLA)
- [BGA Fanout Routing - Autodesk EAGLE](https://www.youtube.com/watch?v=XgJomyAvxrA)

Differential signalling: [Learn how to use Differential Pair for PCB Design in Autodesk EAGLE](https://www.youtube.com/watch?v=GAu8aP3qAwE)

High Speed circuits: [High Speed PCB Design Guidelines 2019 - Autodesk EAGLE](https://youtu.be/HDMW2GFEyTs)

Signal Integrity: [Introduction to Signal Integrity for PCB Design](https://youtu.be/TExobD7vDUY)
