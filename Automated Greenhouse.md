**Problem statement:** To design an automatic greenhouse model according to the requirements (like water, light, temperature) of the plantation.

**Constraints:**
* Physical requirements(like ambient temperature, lighting) to be met with required environment to make plant grow properly.
* Timer setup for each required task.
* Water and electronic instruments shouldn't interact.
* Allowing external control and management along with data extraction of each task.
* Power requirements along with being cost-effective.

**Ideation:**

Physical measurements => sensors => microcontroller => actuators and data storage(optional) <= exteral control by us

Process | Solutions available | Advantages | Disadvantages
--------|---------------------|------------|--------------
Physical measurements + Sensors| 1. Monitoring all the available factors <br/> 2. Monitoring limited essential factors | 1. Prevention from loose ends and minimised risks <br/>2. Easy to implement/monitor and low power input| 1. High cost, difficult to monitor <br/>2. Compromise on risk management.
Microcontrollers| 1. Arduino + Raspberry Pi 3 ([Quick guide](https://www.instructables.com/id/Connect-Your-Raspberry-Pi-and-Arduino-Uno/))<br/>2. Arduino + NodeMCU esp8266 ([Quick guide](https://www.instructables.com/id/Quick-Start-to-Nodemcu-ESP8266-on-Arduino-IDE/)) <br/> 3. Separate greenhouse computer technology ([Example](http://www.climatecontrol.com/climate-manager/))| 1. Connection to internet, micro 'computer', extreme processing capability <br/> 2. Suitable for specific IoT appliction, cheaper (Rs.750)<br/> 3. Readily available, vast flexible features  | 1. Very costly(Rs. 2000) <br/> 2. Power constraints and limited functions <br/> 3. Too costly
External control, monitor and/or management | 1. Blynk app in android <br/> 2. Website and database | 1. Very simple and less time taking setup, allows all IoT applications <br/> 2. Allows more features and flexibility | 1. cannot implement complex projects <br/> 2. More time and knowledge required to develop.

Final Ideation:-

Analysing the table for the available solutions and features:
* **Physical factors:** Keeping in mind, the complexity of plant growth requirements, instead of limiting to just water, temperature &light, we should extend it to  wind blow, humidifier, nutrient supply, space adjustments and other chemical/physical factors with the required actuators.
* **Microcontrollers:** Arduino+Raspberry Pi 3 seems compatible as more physical factors undertaken which is difficult for NodeMCU.  Costs may go up a bit (actuators + raspberry pi), but will help plant to grow healthier.
* **External control:** Designing a website seems good as flexibility required for more features and complex arrangement. Will take some more time, but will be helpful.

The initial approach (as per an instructable) is summarised here: [Automated Greenhouse](https://github.com/prateekagrawalgithub/Electronics-club-Mini-Task-1/blob/master/Automation/Automated%20Greenhouse.md)

*As we have broader approach for plant care and growth, a bit more cost involved looks effective than the initial approach. So, it's cost-effective, more flexible to introducing more features, accurate and a high-quality greenhouse devised*
