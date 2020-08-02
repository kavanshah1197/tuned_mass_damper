# Background and Motivation
Throughout history, humans have built impressive structures and cities only for them to encounter the forces of nature. Earthquakes are one of the Earth’s most destructive forces — the seismic waves throughout the ground can destroy buildings, take lives, and costs tremendous amounts of money for loss and repair.
According to the National Earthquake Information Center, there is an average of 20,000 earthquakes each year —16 of them being major disasters. As with the case with most earthquakes, the damage was not caused by the quake itself but by the collapse of buildings with people inside them, making earthquake-proof buildings a must.

![Earthquake](https://s3-us-west-1.amazonaws.com/acropolis-wp-content-uploads/2019/02/impact-of-earthquakes-v2.gif)
[^fn]
[^fn]: Image/gif taken from https://www.bigrentz.com/blog/earthquake-proof-buildings
---
# Designing earthquake resistant buildings
Over the past few decades, engineers have introduced new designs and building materials to better equip buildings to withstand earthquakes, a few of which are outlined below:
- Base isolation - One way to resist ground forces is to “lift” the building’s foundation above the earth. Base isolation involves constructing a building on top of flexible pads made of steel, rubber, and lead. When the base moves during the earthquake, the isolators vibrate while the structure itself remains steady. This effectively helps to absorb seismic waves and prevent them from traveling through a building.

![Base isolation](https://s3-us-west-1.amazonaws.com/acropolis-wp-content-uploads/2019/02/flexible-foundation-1.gif)
[^fn]
- Tuned mass damper – Engineers suspend a large mass with steel cables with a system of hydraulics at the top of the building. When the building begins the sway, the mass moves in the opposite direction to stabilize the direction. Like damping, these features are tuned to match and counteract the building’s frequency in the event of an earthquake.

![Tuned mass damper](https://s3-us-west-1.amazonaws.com/acropolis-wp-content-uploads/2019/02/pendulum.gif)
[^fn]
- Shock absorbers - Like their use in cars, shock absorbers reduce the magnitude of shockwaves and help buildings slow down. This involves placing dampers at each level of a building between a column and beam. Each damper consists of piston heads inside a cylinder filled with silicone oil. When an earthquake occurs, the building transfers the vibration energy into the pistons, pushes against the oil. The energy is transformed into heat, dissipating the force of the vibrations.

![Shock absorbers](https://s3-us-west-1.amazonaws.com/acropolis-wp-content-uploads/2019/02/vibration-control-v3.gif)
[^fn]
---
# Problem setup and simplifying assumptions
- A 20-story building is modeled in 2 dimensions, assuming the case where the displacement in the out-of-page direction is negligible compared to the displacement in the in-plane directions. 
- Second, only the mass of the floor/ceiling slabs (denoted by m1, m2, …, mn) and the mass of the TMD are considered significant in the model. The floor slabs are modeled as rigid beams, while the supporting columns are modelled as columns having elastic modulus E and area moment of inertia I. The beams are assumed to be fixed at both ends. 
- The wind load is assumed to vary linearly as the height from the ground increases. Wind load is calculated by assuming 20m/s wind at the top floor and by using the assumed façade area. This load is then linearly interpolated to all floors
- The earthquake is assumed to only displace the ground along the X-axis. The frequency and amplitude of the earthquake can and have been changed in this investigation.

![Simplified problem setup](https://github.com/kavanshah1197/tuned_mass_damper/blob/master/Simplified_rep_building.jpg?raw=true)

##### Modal analysis results - 20 mode shapes and corresponding natural frequencies

![Modal analysis results](https://github.com/kavanshah1197/tuned_mass_damper/blob/master/Mode%20shapes%201%20to%2020%20with%20frequency.jpg?raw=true)


##### Selected result - change in the displacement time series due to addition of TMD
![Short time response of top floor for TMD only](https://github.com/kavanshah1197/tuned_mass_damper/blob/master/Short%20time%20resp%20with%20tmd.jpg?raw=true)
