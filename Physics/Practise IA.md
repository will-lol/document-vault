# How does the radius of a balloon affect its terminal velocity?
## Introduction
## Research Question
I want to explore the relationship between the volume of gas (exhaled air) in a ballon and its terminal velocity. Measuring the volume of air in a balloon is mathematically challenging, so the radius may be a more fitting measurement. Terminal velocity is possible to measure using a camera because the balloon reaches 95%+ terminal velocity very quickly. My question therefore is:

**How does the radius of a balloon affect its terminal velocity?**
## Theory and Hypothesis 
The following is a force diagram of a balloon falling through air:
![[balloonforce.svg|300]]
There are 3 forces acting on the balloon: weight, drag and buoyancy. The balloon reaches a terminal velocity, meaning that the net force acting on the balloon is 0. Buoyancy and drag are not necessarily the same. 
### Weight
To find the weight of these balloons we must know the mass. The mass of the balloons depends on the volume of exhaled air in the balloons. According to BBC bitesize and Engineering toolbox, the composition of exhaled air is as follows: 

|         Gas         | Percent in exhaled air (BBC Bitesize) | Density at NTP/STP (Engineering toolbox) |
|:-------------------:|:-------------------------------------:| ---------------------------------------- |
|    Nitrogen, N2     |                  79%                  | 1.165 kgm<sup>-3</sup>                   |
|     Oxygen, O2      |                  16%                  | 1.331 kgm<sup>-3</sup>                   |
| Carbon dioxide, CO2 |                  4%                   | 1.842 kgm<sup>-3</sup>                   |
|        Other        |                  1%                   |                                          |

Assuming that the balloons are spherical and at normal temperature and pressure (293K, 100 kPa), we can generate a formula for relating the radius of the balloon to its weight. The mass of an empty ballon is 0.004kg. 
$W=mg$,  $V=\frac{4}{3}\pi r^2$, $m=V\cdot\rho$, $g=9.81$
$$ m=0.004 + 1.165((\frac{4}{3}\pi r^2) \cdot 0.79) + 1.331((\frac{4}{3}\pi r^2 \cdot 0.16) + 1.842((\frac{4}{3}\pi r^2 \cdot 0.04) $$
$$ W = 9.81(0.004 + 1.165((\frac{4}{3}\pi r^2) \cdot 0.79) + 1.331((\frac{4}{3}\pi r^2 \cdot 0.16) + 1.842((\frac{4}{3}\pi r^2 \cdot 0.04))$$
### Drag & Buoyancy
Buoyancy is a constant force that does not vary as the balloon falls. The buoyant force is a force upward that is a result of gravity. When an object is in a fluid it displaces some of that fluid. The weight force of that displaced fluid is the buoyant force. Since the volume of air displaced is approximately the volume of the balloon, we can predict the buoyant force quite easily knowing the density of air at normal temperature and pressure.
$$W_a=\rho\cdot g \cdot V$$
$$ W_a=1.2041\cdot9.81\cdot V $$
We can replace V with the formula for the volume of a sphere.
$$W_a=1.2041 \cdot 9.81 \cdot \frac{4}{3}\pi r^2$$
$$\therefore W_a \propto r^2$$
The relationship between buoyancy and weight is constant. As we increase the radius, the ratio between the two is the same. This is due to the fact that both values are proportional to $r^2$. Calculating the ratio between them results in a value around 1.002, meaning the balloon will always accelerate slightly downward.

Drag is not a constant force, it varies with the velocity of an object. This variation is the foundation of the concept of terminal velocity — the acceleration of the object decreases as its velocity increases and so the velocity will approach a point that we call terminal velocity. This explains why we can never measure terminal velocity with a great deal of accuracy. However, there are a number of constants that affect drag. The drag equation:
$$D=C_d \cdot \frac{\rho V^2}{2} \cdot A$$
$C_d$, the drag coefficient is a value comprised of many factors specific to an object.
$A$ is the projected area
$D$ is the drag force
We can replace the $A$ with the formula for area of a circle.
$$D=C_d \cdot \frac{\rho V^2}{2} \cdot \pi r^2$$
$$\therefore D \propto r^2$$
### Predicting a trend
All 3 forces acting upon the balloon in this situation are proportional to the radius squared of the balloon which makes it difficult to predict a trend. However, the fact that the drag coefficient varies with velocity means that despite changes in the buoyant and weight forces means that a change in radius will result in a smaller terminal velocity. I expect that a plot of radius versus terminal velocity will result in a power graph with two asymptotes. Therefore, a plot of the square root of radius should result in a negative linear trend.
## Experiment
### Variables
**Independent variable:** Radius of balloon
- Circumference will be measured and converted into radius using circumference formula, $r = \frac{C}{2\pi}$
**Dependent variable:** Terminal velocity
- Will be measured using a smartphone camera
- Video will be processed in DaVinci Resolve
- The 'Tracker' tool in the 'Fusion' page of DaVinci Resolve will be used to plot displacement against time
- The resulting data will be processed in Excel. The beginnings and ends of the balloon's displacement time graph will be trimmed off according to how long they took to reach a terminal velocity
- The trend line tool in Excel will be used to find a value of terminal velocity

| Control variable                  | Action/Explanation                                           |
| --------------------------------- | ------------------------------------------------------------ |
| Air pressure                      | Do not change rooms, record trials in a short period         |
| Temperature                       | Do not change rooms, record trials in a short period         |
| Height dropped from               | Mark a consistent height on the wall                         |
| Camera frame rate                 | Ensure camera is not in auto frame-rate mode                 |
| Composition of gas in balloon     | Use the same person to blow up balloons                      |
| Outside forces other than gravity | Record inside, ensure fans or air-con is off                 |
| Position of camera                | Keep camera in a secure position, record trials in one video |
| Initial velocity                  | Drop balloon in a consistent manner                                                             |

### Diagram
![[diagram.svg | 300]]
### Apparatus
- Balloon (4x)
- 1m ruler (2x)
- Small box (1x)
- Video camera (1x)
- Tape 
- Digital video editing software with tracking and tracking data export function (1x)
### Method
1. Two one-meter rulers were taped to the wall, end-to-end and vertically. The polystyrene box was taped above them so that the the lower face was in-line with the highest point of the rulers.
2. The circumference to be tested was measured on the tape measure and formed into a loop, being pinched in place so as not to move.
3. The balloon (colour corresponding) was held so that it fell into the middle of the loop created. As it was inflated, the tape was adjusted continually such that it stayed around the widest point perpendicular to the symmetrical axis of the balloon. Once the balloon was large enough for the tape to be taught, air was slowly released until there was no deformity in the surface of the balloon, but the tape was still pulled smooth against it. The balloon was removed from the tape and the neck was tied. The balloon was labeled with a permanent marker to note its circumference.
4. The camera was set up in a consistent position that allowed it to see clearly both the top of the polystyrene box and the floor in front of the rulers.
5. The balloon was then placed on top of the polystyrene box such that their ‘tail’ (the knot of the neck) was in-line with the centre of the polystyrene box (from the camera’s perspective) and was sitting just off of the edge of the box.
6. The camera was started and the balloon released, allowing it to roll off of the box tail-down and fall to the ground. The balloon was placed and released again several times. Trials were repeated if the balloon drifted a significant distance horizontally (leaving the frame of the camera).
7. This process was repeated for all of the diameters (30, 45, 60, and 75 centimetres).
8. Import the videos into DaVinci resolve for processing. Trim videos into individual trials and repeat the following for each. Open fusion page, add a 'tracker' node; resize the bounding box to fit the balloon when its displacement is 1m; track forward and back, ensuring all frames have a keyframe; edit inaccurate keyframes; export data from Resolve using the spline editor; import into Excel.
## Results
### Raw Data
![[raw data.png]]
### Processed data
Radius of different balloons versus terminal velocity

| $radius$ | $\sqrt{radius}$ | terminal velocity (ms-1) | negative uncertainty | positive uncertainty |
| ------ | ------------ | ------------------------ | -------------------- | -------------------- |
| 0.15   | 0.38729833   | 2.1371                   | 0.9447               | 0.6745               |
| 0.225  | 0.47434165   | 1.6189                   | 0.2375               | 0.3375               |
| 0.3    | 0.54772256   | 1.2913                   | 0.2324               | 0.1781               |
| 0.375  | 0.61237244   | 1.2797                   | 0.1424               | 0.0454               |

#### Example calculations
**To calculate average displacement at each recorded time**
$$ \overline{s} = \frac{0.072188 + 0.176630 + 0.090990 + 0.148962}{4} $$
**To calculate positive uncertainty in the average**
$$ \Delta \overline{s} = |s_\mathrm{min} - \overline{s}| $$
$$\Delta \overline{s} = |0.09099 - 0.1221925|$$
**To calculate negative uncertainty in the average**
$$ \Delta \overline{s} = |s_\mathrm{max} - \overline{s}| $$
$$\Delta \overline{s} = |0.176630 - 0.1221925|$$
**To find cropped data range**
![[sample graph.png | 300]]
Using a plot of average displacement over time, draw a trend line where the terminal velocity is and record the values either side.
**To find the terminal velocity**
![[sample graph 2.png | 300]]
Using the cropped data, use Excel to plot a min, max, and average trend lines and record the gradient values.
## Graph
![[graph.png | 300]]
## Discussion
### Analysis and Conclusion
It was predicted in the hypothesis that the plot of the square root of balloon radius versus terminal velocity would result in a negative linear trend. This trend can be observed in the data, but not with much certainty.

Best fit gradient: $-3.9559 \; \mathrm{ms}^\mathrm{-1}\mathrm{m}^\mathrm{-\frac{1}{2}}$
Min fit gradient: $-0.5994 \; \mathrm{ms}^\mathrm{-1}\mathrm{m}^\mathrm{-\frac{1}{2}}$
Max fit gradient: $-5.1659 \; \mathrm{ms}^\mathrm{-1}\mathrm{m}^\mathrm{-\frac{1}{2}}$

Gradient: $-3.9559 \pm 2.8883 \; \mathrm{ms}^\mathrm{-1}\mathrm{m}^\mathrm{-\frac{1}{2}}$
Percentage uncertainty: $73.012\;\%$

The percentage uncertainty in this answer is very large. This makes it extremely unreliable. This is largely due to the uncertainty in the points because all of the points lie reasonably close to the trend line. In fact, the first 3 points appear to be extremely linear, while the last point deviates. 

In conclusion, it cannot be said that the squared radius of the balloon is not proportional to the terminal velocity.
### Evaluation
The design and method of this experiment was unsuitable to come to a clear conclusion relating radius and terminal velocity.

| Weakness                                                                                                                                                                                                                                                                                                                     | Significance                                                                                                                                                                                                                                                                                                                                                           | Improvement                                                                                                                                 |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------- |
| The values output by DaVinci resolve are a number ratios between 0 and 1 attached to time stamps. 0 being the starting position and 1 being the end position. These positions would have varied depending how much of the balloon was visible for its entire travel. It was assumed that 0 was 0m and 1 was 2m displacement. | This issue meant that in data analysis, the starting and ending points (where velocity was decreased) were inconsistent. This lead to very large error bars in the average displacement of starting and ending points. This had a flow on effect for the uncertainties in terminal velocity, especially for trials of smaller balloons due to their short flight time. | Use a second person or some form of controlled dropping method that clearly shows when the balloon has started accelerating due to gravity. |
| In cutting and tracking balloons in videos, finding the exact moment that a ballon began falling was inconsistent and difficult to see. This adds to the significance of the previous issue.                                                                                                                                 | This issue meant that the displacement values were further skewed between trials.                                                                                                                                                                                                                                                                                      | Use a second person or some form of controlled dropping method that clearly shows when the balloon has started accelerating due to gravity. |
| The balloons were subject to small drafts and gusts due to very small movements.                                                                                                                                                                                                                                             | This issue meant that the balloons would accelerate in directions other than downward, skewing displacement values.                                                                                                                                                                                                                                                    | Ensure the room has very little air flow and that no gusts of wind are present.                                                             |
| The balloons 'rolled' out of the polystyrene box giving them an initial momentum before any vertical displacement. This rolling was also inconsistent and unpredictable among trials.                                                                                                                                        | This issue meant that balloons would sometimes drop with an initial velocity, skewing their displacement values further.                                                                                                                                                                                                                                               | Use a second person or some form of controlled dropping method (mechanical machine) that drops the ball consistently                        |
| Balloons with a larger radius were subject to more wind and gusts due to their larger surface area.                                                                                                                                                                                                                          | This issue meant that balloons with larger radius had skewed displacement due to gusts that was higher than other balloons.                                                                                                                                                                                                                                            | Ensure the room has very little air flow and that no gusts of wind are present.                                                                                                                                            |
If the experiment is to be repeated, a very small enclosed room and some kind of device to consistently drop balloons would be recommended. 

<div style="page-break-before: always;"></div>

## References
_Gas exchange in the lungs - Respiratory system - GCSE Biology (Single Science) Revision_ n.d., _BBC Bitesize_, viewed 8 August 2022, <https://www.bbc.co.uk/bitesize/guides/z6h4jxs/revision/3>.

_Gases - Densities_ n.d., viewed 8 August 2022, <https://www.engineeringtoolbox.com/gas-density-d_158.html>.

_Terminal Velocity (gravity and drag)_ n.d., viewed 8 August 2022, <https://www.grc.nasa.gov/www/k-12/rocket/termvr.html>.
