3-Channel ADC 
-------------

Based on Analog Devices `AD4030-24 <https://www.analog.com/media/en/technical-documentation/data-sheets/ad4030-24-4032-24.pdf>`_ .

The current version of the `3-channel data logger schematic <../_static/3-channel_ADC.pdf>`_ is meant for discussion. It is not intended to be a finalized design.

Design decisions for the ADC board:

    #.  Input filter:

        #. Do we need an input filter in front of the ADC?
        #. Currently the schematic contains elements for passive filter elements in common mode and differential mode. The resistors are 0 Ohm types and all capacitors are DNP. This allows to add a passive filter if we want to.
        
    #.  Shielded connector:

        #. Do we want to add a shield to the 10-pin connector between the analog board and the digital board?
    
    #.  Buffer amplifier for the reference:

        #. On page 27 of the `AD4030-24 data sheet <https://www.analog.com/media/en/technical-documentation/data-sheets/ad4030-24-4032-24.pdf>`_ the options for the reference input of the ADC are discussed. I'm currently undecided if it is better to use the REF or the REFIN ports of the ADC. The data sheet mentions that the best possible gain error is achieved with an external buffer and the REF pin. However, figure 28 shows an increased error in case of a burst in combination with an externally driven reference. This should never happen in our application.

        #. What is the better option to fight noise. A driver close to the reference source should keep the reference signal low impedance and lower the overall noise.

        #. We need a reference buffer anyhow as the reference voltage is needed on the analog board. What is the reference voltage actually needed for?
