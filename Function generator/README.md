# Functional generator based on operational amplifiers
https://everycircuit.com/circuit/6253211932164096
![final scheme](https://user-images.githubusercontent.com/24607459/175829432-e2b665b3-46ee-44b6-8238-fa08ad03942b.PNG)
press button (or shake your mobile device) to initialize occilations. Amplitude will obtain 5 volts.
=====================================================================================================================


There is a useful derivator scheme based on op-amp:
![derivator](https://user-images.githubusercontent.com/24607459/175816549-78b8fca8-be4c-4b4c-8324-94cc070f9977.PNG)
Given input signal x(t), it returns <img src="https://latex.codecogs.com/svg.image?-R\cdot&space;C&space;\cdot&space;\frac{\partial&space;x}{\partial&space;t}"/>

It can be used to solve differential equations like this:
![functional scheme](https://user-images.githubusercontent.com/24607459/175817329-34faa98f-81ed-48e2-b974-ab746783db84.PNG)
As we can see on picture above:

<img src="https://latex.codecogs.com/svg.image?x(t)&space;=&space;-\ddot{x}(t)&space;,so:x(t)&space;=&space;A\cdot&space;sin(\omega&space;t&plus;\varphi&space;)"/>

![simple scheme](https://user-images.githubusercontent.com/24607459/175818473-ced9c0c4-9e79-4bcd-b1a6-084100e4bd52.PNG)

There is a problem: amplitude and phase are not fixed, so amplitude could change randomly. We need to add another feedback loop to regulate amplitude. One of possible solutions:
![full functional scheme](https://user-images.githubusercontent.com/24607459/175820813-78457d37-1f09-43cf-bfeb-000df90c3e36.PNG)

https://everycircuit.com/circuit/6253211932164096
![final scheme](https://user-images.githubusercontent.com/24607459/175829432-e2b665b3-46ee-44b6-8238-fa08ad03942b.PNG)
