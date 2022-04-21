# TO DO:

## HARDWARE: Joint effort --> Kate, McKenna, Ashlee

  -Identify and procure antenna
  
  -Build/Order cables (Including adapters if necessary)
  
     -CDH to Xcvr
     
     -Xcvr to LNA
     
     -LNA to Antenna (If antenna doesnt come with one that works)
     
     -Power to LNA
    
    
    
## LINK BUDGET: McKenna, Dan
  
  -Copy oresat diagram as starting point
  
  https://github.com/oresat/oresat-c3-rf/blob/master/link-models/OreSat1_link_model_v2.5.5a_eng_primary.pdf
  
  -Determine if current parts provide correct power levels
  
  -Estimate achievable data rate
  
  -Verify architecture will comply with FCC
 
 
 
## ENCODING/MODULATION: Kate, Ashlee 
  
  -Establish CDH (Rpi)/ Xcvr link
  
  -Determine data encoding protocol
  
  -Determine modulation scheme
  
  
## MISC: Dan

  -Talk to EOSS about freq usage and see if they have antenna recommendation


# Parts:
HTC
https://www.seeedstudio.com/433Mhz-Wireless-Serial-Transceiver-Module-1-Kilometer-p-1733.html

LNA
https://www.digikey.com/en/products/detail/signal-processing-group-inc./LNA%2520-00120/13980502?utm_adgroup=Signal%20Processing%20Group%20Inc&utm_source=google&utm_medium=cpc&utm_campaign=Shopping_DK%2BSupplier_Other&utm_term=&utm_content=Signal%20Processing%20Group%20Inc&gclid=CjwKCAiA1JGRBhBSEiwAxXblwbAXTGDeDRQM1EYvt4CfAOFc4UvDOuQEqoSz-NYzY6nFP2amaY8hThoCWnwQAvD_BwE

# Regulation Notes: ***NOT COMPREHENSIVE***

Wavelength band | Frequencies | Emission types authorized | Standards see § 97.307(f), paragraph:

70 cm | Entire band | MCW, phone, image, RTTY, data, SS, test | (6), (8). 

(6) A RTTY, data or multiplexed emission using a specified digital code listed in § 97.309(a) of this part may be transmitted. The symbol rate must not exceed 56 kilobauds. A RTTY, data or multiplexed emission using an unspecified digital code under the limitations listed in § 97.309(b) of this part also may be transmitted. The authorized bandwidth is 100 kHz. 

(8) A RTTY or data emission having designators with A, B, C, D, E, F, G, H, J or R as the first symbol; 1, 2, 7, 9 or X as the second symbol; and D or W as the third symbol is also authorized.

No station may transmit with a transmitter power exceeding 50 W PEP on the UHF 70 cm band from an area specified in paragraph (a) of footnote US270 in § 2.106, unless expressly authorized by the FCC after mutual agreement, on a case-by-case basis, between the Regional Director of the applicable field facility and the military area frequency coordinator at the applicable military base. An Earth station or telecommand station, however, may transmit on the 435-438 MHz segment with a maximum of 611 W effective radiated power (1 kW equivalent isotropically radiated power) without the authorization otherwise required. The transmitting antenna elevation angle between the lower half-power (−3 dB relative to the peak or antenna bore sight) point and the horizon must always be greater than 10°.



# Links:

Regulations:

https://www.ecfr.gov/current/title-47/chapter-I/subchapter-D/part-97

https://www.arrl.org/part-97-amateur-radio

Frequency band notes:

https://www.arrl.org/band-plan

https://www.arrl.org/files/file/8803051.pdf

Interference notes:

https://www.arrl.org/radio-frequency-interference-rfi

Swapping UART ports for rpi compute module 4

https://docs.turta.io/how-tos/raspberry-pi/raspbian/swapping-the-serial-ports


# Notes from 3/25

Trying to get response from Rpi to HC-12 via AT command mode

-are we configuring rpi uart correctly?

-is our terminal setting/using the right baud (9600), default for pi is 115200

-are we setting the HC-12 correctly to get into AT command mode?

-maybe we skip and go straight for module to module comms? (means no way to verify hc-12 settings)
