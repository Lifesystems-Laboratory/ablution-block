# Water Solutions

## Water analysis

### Purpose of testing 
Apart from obvious reason to test water to be sure it's safe to drink there are many benefits to testing it multiple places in the system for a multitute of paramaters such as temperature, flowrate in pipes, total dissoleved solids, pH etc. This data can show the effectiveness of water heating and filtrations systems, inform and automate system maintainance. 

### Methods of testing 
We will try to get as much as possible data from ESP8266 and ESP32 nodes and sensors that can provide data about water from multitudes of perspectives.  

### live data and AI
Live data will be gathered and logged by HomeAssistant (more on that in Brains sections). Multiple actions can be scripted and automated to optimise energy usage for water sourcing, purification and heating. HomeAssistant has AI / machine learning integrations (e.g. Tasmota) that can act as an agent and adjust multiple parameters based on the model of the environment and predicted usage. 


## Drinking water / Technical water
In some locations where there is unverified water source or no water source, it would be great if Ablution block could have some kind of water collection and filtration system. 
Water filtration system can make sure that there is a source of drinking / technical water that is safe to use.

### Rain water collection and filtration 
We are building modular rain water harvesting and filtration system. Rainwater showed on TDS (Total dissolved solids) meter as close to distilled 40 mg/L (PPM). The size of the system will be defined by the usage and rainfall prediction models. The tricky part is storing harvested water in subzero temperatures, as the water reservuars inside insulated space are limited capacity. 
In the warm period of the year outdoor modular water tanks, gutter system and filers can be scaled up easily depending on the usage. 

### Atmospheric water generation
Humidity measured so far was typically 30-60%. We have already installed heat pump (air-to-air) that can work as dehumidifier and collect water from the air. We plan to experiment with other type of dehumidifyers or DIY solutions. 

### Ground water source
Currentl location of ablution block v.0.1 has access to a well, but water there is not super clean, TDS shows 320 PPM, so we are testing varios filters such as activated charcoal and cationic resin filters with moderate success (reduced to 240 PPM). Ground waters while have some level of filtration can be still polluted and need constant monitoring.   


## Waste Water
There is a lof of water used by human life actyvities (washing, cooking) that needs to be reused, preserved or safely disposed. 
We want to experiment with grey and black water filtration systems. 
Filtering water to the level that it can be used again as technical water could reduce total water consumption. 

### Grey water
Seperating grey water can make it much easier to clean and reuse water. Using available filters in conjunction with biological ways to clean water (ponds, plant etc.)

### Black water
We would like to work on low cost and effcicient alternative to septic tanks for black water. One of the alternatives available on the market is Bio-Septics of different types. 

