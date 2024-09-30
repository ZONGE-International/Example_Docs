Requirements 
------------

#. Three input channels for search coil magnetometer
#. Analog Devices `AD4030-24 <https://www.analog.com/en/products/ad4030-24.html>`_ ADC. One ADC/channel.
#. Reference voltage is 4.096 V.
#. Input voltage range -Vref to +Vref 

    #. Differential input with 2.5 V common mode.
    #. Input range IN+ to GND: 452 mV to 4.55 V
    #. Input range IN- to GND: 452 mV to 4.55 V
#. Sampling rate 2^17 Hz. The underlying sampling rate of the datalogger is 2^20 Hz. The reduction to 2^17 Hz is done by a block filter inside of the ADC.
#. Analog frequency range to be controlled by amtenna section.
#. Power delivery to analog board: 
    
    #. +- 9 V with a minimum on 30 mA on each rail.
    #. Ripple: TBD
    #. Noise:  Wide bandwidth noise must be filtered out.