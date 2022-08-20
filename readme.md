# DroneAssistant Buttplug
## An Home Assistant Powered Butt Plug

### Parts and Materials

You will need

#### **Software**
- A Home Assitant Instance
- ESPHome Installed in Home Assistant
- a Loose Knowledge of how to use ESPHome

#### **Hardware with Links**
-  ESP D1 Mini, I used these you can use any kind of ESP that works with ESP Home, It needs to have PWM outputs which most do. Warning, the ESP D1 Minis will require you to solder the legs on, you can get pre-soldered boards such as the ESP8266 Dev kit
    - https://www.amazon.co.uk/Development-NodeMcu-ESP8266-Internet-Compatible/dp/B08QZ2887K/ref=sr_1_6?crid=3MIWN7WQOOAXW&keywords=ESP+D1&qid=1660992149&sprefix=esp+d1%2Caps%2C74&sr=8-6
- PWM to Voltage Convertor Board - I used these DC Motor Controllers You need something that takes the PWM Speed control from the ESP and turns it into more or less voltage, these work very well are small and cheap. - these will require you solder the wires in place or solder on header cables 
    -https://www.amazon.co.uk/gp/product/B07ZHC5M7H/ref=ppx_yo_dt_b_asin_title_o00_s00?ie=UTF8&psc=1

- Some Jumper Wires.
    -https://www.amazon.co.uk/240pcs-Solderless-Breadboard-Arduino-Project/dp/B08PJSTS3C/ref=sr_1_7?crid=376EIZ26JGYYE&keywords=breadboard+jumper+wires&qid=1660992325&s=industrial&sprefix=breadboard%2Cindustrial%2C60&sr=1-7

Some way of making conecting wires together, I recomend wago style cage clamp connectors, prefferably made by wago, 

#### **Container**
For the container I used the a Wiska box 206 and an M20 gland, this 
should mean it's splashproof which makes cleaning after play easier, 
    
- https://ww.amazon.co.uk/WISKA-Weatherproof-Outdoor-External-Junction/dp/B08D6MBFZG/ref=sr_1_2?crid=189E8EJDCG5FF&keywords=wiska+206&qid=1660992783&sprefix=wiska+206%2Caps%2C66&sr=8-2


**Wiring**
- D1 to PWM side of PWM Board
- GND from PWM to GND wago
- GND from Board to GND wago 
- GND from Vin out to GND wago
- 5v from VIN IN to 5v pin


**Software**
 - Create a config in ESPhome and copy code from repo into it, 
    - tweak as needed

I've added a modified flicker automation, which will work with a toggle helper you'd need to setup in home assistant which would vary the amount of power every 6 seconds 