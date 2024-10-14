System Power 
++++++++++++

The following elements need to be powered:

    #.  Antennas
        #. Voltage: +9 V and -9 V 
        #.  Power:  13 mA average, 20 mA peak per antenna. Clarify with John if this is 20 mA for each power rail or total.
    #. Digital board
        #. ADC:
            #. +5 V 
            #. + 1.8 V for the analog section.
            #. + 1.8 V for the digital section.
        #. FPGA:
            #. 3.3 V is used by the FPGA and the flash memory that carries the FPGA code.
            #. 1.8 V for IO connection to ADC
            #. 1.2 V locally generated from 1.8 on iCEBreaker board. Maybe DCDC?



