System Elements 
+++++++++++++++

#. Antennas
#. IMU
    #. Based on a system design where all components are mechanically connected to each other the IMU can be placed onto the digital board directly. This saves space and reduces cables.
#. Data Logger 
    #. Three simultaneously sampling  Analog Devices `AD4030-24 <https://www.analog.com/en/products/ad4030-24.html>`_ ADC running at :math:`2^{17}` Sps.
    #. GPS timing control.
    #. Data storage onto SD card.

#. Power supply


External Ports 
++++++++++++++

#. Battery connection
#. GPS antenna connection
#. Data read port. Details to be decided, options are USB, Ethermet ,??
#. Mechanical option to remove SD card.
#. Antenna for Bluetooth or WiFi communication (optional).
#. LoRa antenna or similar for position and status beacon (optional).