# Optimising Pipeline

## [Project 1: Water Level Indicator](https://github.com/GayatriRR/MiniTask1#proj-17-water-level-controller-using-8051-microcontroller)

**Problem Statement:** In our daily lives, we need to regularly measure the level of water in the tank to know when to switch the motor on and off. For this, we need a water level indicator which can estimate the level of water in the tank. 

**Ideation:** The current project uses microcontroller 8051 with probes at different levels to sense the level using transistors and relays to automatically switch on and off the motor according to feedback from the probes. We realize that a major deciding factor of this project is the sensor; thus we need to choose a sensor appropriately. 

Sensor >> Transistor >> Microcontroller >> Relay >> Pump

| Sensor choice | Feasibilty | Advantages | Disadvantages |
|------------|---------------|---------------|----------------|
| [Probes](https://www.electronicshub.org/water-level-controller-using-8051-microcontroller/) | Easy to implement. Water level measurement in steps. | Water level for tank of any depth can be measured. | Measurement of water is limited to the number of probes. Moreover, more probes result in more area occupied. | 
| [Ultrasonic](http://www.circuitstoday.com/ultrasonic-water-level-controller-using-8051) | Easy to implement. Sensor can give exact water level. | The exact depth of water is given (precision of 1cm). | The tank needs to be within a depth of 2m|

The selection of the sensor depends on the application. For common household tanks, it is better to use probes in the project because an ultrasonic sensor limits the depth of the tank. Here, we only need to check if the tank is full to switch the motor off and if it is empty to switch the motor on. On the other hand, if we need an accurate measure of the depth of the water level, we might need to use an ultrasonic sensor.

Moreover, the project involves an LCD Display displaying the amount of water in the tank. For a common househohold tank, this can be avoided. By avoiding bringing in the LCD Dispaly, we do not even need the microcontroller in the project. Thus I would suggest removing the microcontroller and the LCD Display in the water level controller used for tanks at home. 
This would involve a Probes >> Transistor >> Relay >> Pump circuit. 

An LCD Display for a circuit containing an ultrasonic sensor would make more sense.


## [Project 2: Wireless Electronic Notice Board](https://github.com/GayatriRR/MiniTask1#proj-21-wireless-electronic-notice-board)

**Problem Statement:** Notice boards are of utmost importance in our lives, and we are moving well into the digital world, increasing the need for wireless control of an electronic notice board. The notice board displays the information that is sent to it wirelessly. 

**Ideation:** The project mentioned uses GSM technology for wireless information transfer. An SMS is sent from a mobile through GSM technology using a GSM module to the microcontroller which helps the LCD display the message appropriately. We realize that the wireless technology chosen for the project needs to be thought out well. 

The general working principle of the notice board: Message >> Transmission through a wireless technology >> Corresponding wireless module >> Microcontroller >> LCD Display

| Wireless technology | Feasibilty | Advantages | Disadvantages |
|------------|---------------|---------------|----------------|
| [GSM](https://www.electronicshub.org/wireless-electronic-notice-board-using-gsm/) | Need to understand how to work with the technology | Long range wireless communication | Low data transfer.|
| [Bluetooth](https://www.ijert.org/research/wireless-e-notice-board-using-bluetooth-technology-IJERTCONV6IS07092.pdf) | Not hard to implement when you know how to work with it | Decent transfer of data. Less power consumption. | Short range data transfer. Peer to peer transfer. |
| [WiFi](http://ijiset.com/vol3/v3s3/IJISET_V3_I3_24.pdf) | Not hard to implement, most comfortable infact | Fast transfer, good operating range | Needs to be close to a WiFi access point. Power consumption. |

[Selection of the wireless communication](https://predictabledesigns.com/wireless_technologies_bluetooth_wifi_zigbee_gsm_lte_lora_nb-iot_lte-m/) is based on the applications. For secure long range applications, and ones that might involve the devices not close to a WiFi access point, we would use a GSM technology. For short range applications, depending on data that needs to be transferred, we could choose between bluetooth and WiFi. 



