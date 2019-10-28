# RADIAL
Radio Identification and Location project in collaboration with General Dynamics UK for Engineering Education Scheme Wales 2017 

I lead, wrote the software and designed the hardware set up for this project. The aim was to be able to find people who were missing out of mobile signal. Simply put the system works by flying a drone in a search pattern and mapping the radio intensity of signals in the GMS range. These are presumed to be from mobile phone pings searching for a tower when out of signal range. 

The executive summary from the report is below.

>Every day, hundreds of people around the world find themselves in difficulty, in isolated locations and unable to call for assistance. These people are sometimes victims of accidents or natural disasters but often they are partly responsible for their predicament through lack of preparedness and excessive risk-taking. Many people who find themselves in trouble are carrying with them electronic communications devices that they cannot use to call for help because they are out of range of the necessary communications infrastructure.
>
>The Radio Identification and Location (RADIAL) project being executed by Monmouth Comprehensive School and General Dynamics United Kingdom Limited (GDUK) has evaluated options for a rapidly deployable system to detect and locate the radio signals transmitted by modern personal electronic devices e.g. mobile phones, tablets. A prototype of the preferred option has been designed and implemented, taking into account the legislation for the use of such a system, in particular safety and radio transmissions. The prototype shall be trialled on location with GDUK in March 2017.
>
>Before settling on the final scope of the RADIAL project the school team explored a wide range of ideas that might meet the needs of different types of Emergency Services users. A number of these ideas were discussed when the school team visited GDUK for a site tour. GDUK then decided whether they could adapt any of them to meet their customers’ needs. Some ideas were considered too impractical at the current time e.g. a system that could automatically call the emergency services if a swimmer strayed into a dangerous position in the sea. After reviewing these alternatives it was decided that a system that could detect and precisely locate people in areas of coastline or countryside where they may be at risk would be a useful capability for GDUK to offer to customers.
>
>The school team then worked to further understand the project scope and did a lot of research. It was decided to develop a radio detection system with airborne sensors to minimise the blocking of radio signals by the environment. It was then decided that an Unmanned Aerial Vehicle (UAV or ‘drone’) operated from a Rescue Support Vehicle (RSV) on the ground would provide the best way to increase coverage and improve detection of radio signals. The team then produced a list of questions that it needed GDUK’s advice on. With GDUK’s assistance the team selected a Software Defined Radio (HackRF One SDR) that could detect the range of radio frequencies used by mobile phones and similar devices. A small lightweight processor that could be packaged with the SDR was required to run the SDR software (called GNU radio). The Raspberry Pi 3 (RPi3) was selected from a number of alternative processors. A Global Positioning System (GPS) hardware module was connected to the RPi3 to allow the location of the UAV to be reported back to the RSV.
>
>A considerable effort was made to learn how to get the SDR software to detect the required radio frequencies and power levels. The software was written using the Python language. The software loaded on the RPi3 can process frequencies and power levels and associate these with GPS coordinates. This data is then transmitted to a base computer located in the RSV. A visual display was developed for the base computer to enable users to locate a source of radio signals and direct the UAV. A device that transmits at 27MHz (an unlicensed frequency band used with remote control toys) was acquired to test the system in places where there were already Wi Fi and mobile phone signals.
>
>At the workshop in Cardiff Metropolitan University it was agreed exactly which parts of the overall system would be designed and built by the school team and which parts would be provided by GDUK. It was decided that the team would design and make a case suitable to protect the RPi3 and fix it to the UAV, using sacrificial connectors and cabling between the case and the RPi3. This would then be fitted to the UAV by GDUK alongside the HackRF One SDR which would be in a special screened case. The team sent the specifications for the case and the cabling to GDUK for them to design the rest of the system to be used in the trial.

I would like to note that I wrote all of this code several years ago and acknowledge that some of it is messily and inefficently written and that the whole system is not particularly reliable and could be significantly re designed to improve it. If I was todo the same project again I would design the system in a significantly different way

Written in 2017
