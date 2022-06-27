# New concept of analog processor based on operational amplifiers for computing neuro net algorithms based on operational amplifiers

Look at an example of the simplest neuro net configuration: perceptron
![neuron](https://user-images.githubusercontent.com/24607459/175899744-58625eb9-125d-4838-bc16-4fb3de2b9922.png)
Every single neurone takes an array of real numbers as input, multiplies it by corresponding weights, adds all numbers together and performs activation function.
To calculate it we use special type of processor: TPU (Tensor Processing Unit), contains a large number of separate ALUs, each of them contains a large number of transistors.
![Anatomy+of+a+Neural+Network+Accelerator+Example_+Google+Tensor+Processing+Unit+(TPU)](https://user-images.githubusercontent.com/24607459/175903597-b780c617-7511-4a89-94c9-f60ccea9a562.jpg)
But this isn't the only solution.
We can use analog scheme to perform such calculations. Recall that operational amplifier was developed especially for calculating math operations on analog values (adding, substracting, multiplying on a constant, etc.). We can use a simple scheme below for emulate behaviour of one simple neurone:

![Снимок](https://user-images.githubusercontent.com/24607459/175906990-4a569ba4-1c7e-4afe-b2b0-603e3509c9c7.PNG)
It multiplies input values to corresponding coefficients (depending on related resistance), adds all together and performs activation.
Cascade of two zener’s diodes and one resistor gives a function similar to arctangent
![image](https://user-images.githubusercontent.com/24607459/175908364-d461f308-dc19-476d-b1a1-8a472c716ccf.png)
5 neurons connected in parallel:

![one layer](https://user-images.githubusercontent.com/24607459/175916698-22d7265f-b4e7-4cd3-8eff-a7a2b5086106.PNG)
Instead of resistors it's better to use MOSFETs to be able to reprogram weights and store it (similar to flash memory)

Complete scheme of simple analog TPU for perceptron config with 3 layers (5 neurons each)
![CompleteNet](https://user-images.githubusercontent.com/24607459/175919641-68faebd8-0027-4564-9956-23626d70db12.PNG)
