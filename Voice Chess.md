**Problem Statement:** To design a voice commanded chess game with automatic movements according to voice commands.

**Constraints:**
* Easy voice interaction with the microcontroller.
* Smooth movement of pieces without any collisions/interactions with other pieces.
* Motors to be compatible with microcontroller.
* Power requirements and cost-effectiveness

**Ideating Solution:**

Steps needed: Voice => conversion to text => Arduino => motors => moving pieces => repeat

Process | Solutions available | Advantages | Disadvantages
--------|---------------------|------------|--------------
Voice to text conversion| 1. Android apps (using google voice) <br/> 2. Offline speech to text devices <br/> 3. Deivising our own sample device using deep learning | 1. Simple and direct application including many languages and related features <br/> 2. Same as (1) along with elimination of internet usage <br/> 3. Low chances of error due to limited combination of words and very cost-effective | 1. Uses internet and high chances of error <br/> 2. Costly, high error chances, difficult to work with arduino <br/> 3. Lengthy process of data inclusion with ML <br/>
Transmission to arduino| 1. Using android app and transfer via bluetooth <br/> 2. Communication along I2C synchronous serial protocol | 1. Wireless, high speed and low power communication <br/> 2. Simple, wired and easily compatible communication| 1. Connection issues <br/> 2. Low speed and high energy module
Reaching out to pieces to be moved | 1. Relay activating electromagnets and attracting iron base of that chess-piece <br/> 2. Motors unlocking that chess-piece from its place <br/> 3. Individual sensors/receivers for each piece and activation via a sensor module.| 1. Allows high attraction, smooth and easy movement <br/> 2. Cheap method, easy to implement, low energy and eliminates chances of unlocking other pieces like in (1). <br/> 3. allows high automation, quality and easy method of arduino and piece interactions | 1. Chances of attracting other pieces along with it, high current requirement <br/> 2. System may corrode/break with time <br/> 3. Very costly and difficult to setup, needs good practical sensor knowledge.
Moving pieces using motors | 1. Move along with magnetic interactions as in (1) above <br/> 2. Moving along deep hole lines between houses <br/> 3. Wheeled movement or directly 'flying' to final position. | 1. Easy and smooth movement <br/> 2. Faster movement without any chance of interacting/collision with other pieces <br/> 3. Good quality, less collision chances and attractive/interesting movements | 1. Slower movement and chances of interactions with other pieces. <br/> 2. May degrade/break with time <br/> High current requirement and need good knowledge about sensors.

**Final Ideation:-**

So, after seeing the advantages and disadvantages of the proposed solutions, we can choose the following:
* **Speech to Text conversion:** Using deep learning to make our own device which converts speech to text for only the required ones like A1, A2....A8, B1, B2,....H7, H8. This eliminates chances of errors and allows smooth and fast functioning. A good review on this can be found [here.](http://ijarcet.org/wp-content/uploads/IJARCET-VOL-4-ISSUE-7-3067-3072.pdf)
* **Data transmission to Arduino:** Using any type of communication methods like bluetooth or I2C seems feasible and easy to use/implement depending on the availablity and costing.
* **Piece Identification:** We can have a mechanical method of locking peices to their houses and enable their movement when the motors reach out (from below the chessboard) and unlock it from its house. This shall be controlled mainly by the Arduino.
* **Moving pieces:** Paths to be made in between houses for the movement of pieces with help of stepper motors. This will help faster and smoother movement without interactions/clashing with other pieces.

The initial approach (as per an instructable) is summarised here: [Voice Chess](https://github.com/prateekagrawalgithub/Electronics-club-Mini-Task-1/blob/master/Entertainment/Voice%20Chess.md)

*As some electronic components are eliminated and easy to use devices are introduced along with mechanical components/mechnisms, the cost involved, accuracy, power requirements have considerably reduced along with the implementation being easier and smoother!*
