# IOL-Friction-Testing
Project Scope: Create a friction testing system that can quanitatively measure the durability and lubricity of a hydrophilic polymer coating. Due to the complex geometry of the IOL (Intraocular Lens) cartridge, a precise testing setup is essential. Client informed a strong need for exceptional coating performance - including measuring lubricity, durability, and perfroming a qualitative post-injection inspection under a 1000x 3D surface video microscope. 

IOL & Cataract Info: An IOL is used by an ophthalmologist (eye surgeon) to treat cataracts. A cataract is when an eye's natural lens becomes "cloudy" causing degenerative vision loss. To address this disease, engineers and doctors have created the IOL to act as a new artifical lens. Typically, an ophthalmologist will remove the natural, cloudy lens, and replace it with an IOL. To understand and visually understand the IOL, the IOL cartridge and it's proper setep, please view the video below.

▶️ [Three-Piece IOL Lens Loading Tutorial in Two Minutes by: Matt Hirabayashi MD (@EyeFlyMD)](https://www.youtube.com/watch?v=hnIIPaW2O_Y)


Machine Design: From a conceptual standpoint, the main design was to hold the syringe with the loaded IOL cartridge and allow, the "plunger" to press on the IOL at a consistent speed. Furthermore, the layout of the machine would have to only allow for horizontal movement to mimic the ophthalmologist procedure. From a mechanical standpoint, the design used a stepper motor directly coupled to a lead screw assembly, converting rotary motion into precise and uniform horizontal linear motion of the carriage.

Together with the EGR team, the original CAD was as follows: 

[CAD model Picture 1](https://github.com/Franzvd14/IOL-Friction-Testing/blob/main/IMG_1741%20(1).jpg)
This is a Top View of the Friction Tester (CAD by EGR team; I contributed to the mechanical design concept).

[CAD model Picture 2](https://github.com/Franzvd14/IOL-Friction-Testing/blob/main/IMG_1740%20(1).jpg)
This is a Side View of the Friction Tester.

Machine Design Cont.: To measure the friction testing data, a calibrated force gauge (up to 200N) was integrated to measure the precise injection force. Using a software system such as Logger Lite, the force sensor can take the data and enable "run/ stop" cycles which can produce a force graph (N vs. s). Additionally, to take the data from the force gauge and translate the data to the computer, a "Go!Link" USB interface was used. The raw data could then be exported to Excel or MATLAB for further processing, allowing for clearer visualization and analysis of the results.

An example is seen below:

[IOL Excel Friction Graph](https://github.com/Franzvd14/IOL-Friction-Testing/blob/main/IMG_1987%20(1).jpg)
This graph shows the AVG. force of the uncoated sample (Close to 113N) and the coated sample (Close to 4.5 N). From here a simple calculation (AVG uncoated / AVG coated) is made to show how many more times the coated surface is more lubricious compared to the uncoated surface. It's important to note the objective is to find the lens injection force. This means that there had to be additional testing where data was collected from just the plunger and the viscious saline being injected without the lens to find the correct true lens force. Upon finding this data, the data without the lens was subtracted from the data with the lens granting the true lens injection force.

Machine Build: 

The machine while being built is pictured below.

[Friction Testing Machine](https://github.com/Franzvd14/IOL-Friction-Testing/blob/main/Friction.jpg)
This picture shows each component and the early assembly of the friction tester.

