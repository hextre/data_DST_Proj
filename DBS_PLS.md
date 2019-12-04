1.00.00.1
================
#### Prioritized load shedding 

Control based on the voltage level of the dc bus has also been proposed to ensure high-priority loads in dc systems enjoy an uninterrupted supply of power under overload conditions.
Prioritized load shedding is performed under overload conditions
conditions by controlling the loads to shut down at different voltage levels as the bus voltage collapses due to the overload. The main
difference between the load shedding based on the voltage level of the dc bus and DBS is that DBS uses the dc-bus voltage for
source scheduling, not load shedding. With DBS, the source and storage interface converters operate autonomously based
on the voltage level of the dc bus. Each converter is assigned to a voltage threshold to trigger the point at which it begins
discharging or charging.
The converters not only respond to the level of the dc bus, but they also change the level of the dc bus, automatically
controlling other converters in the system. This autonomous operation is achieved by controlling the converters to exhibit
three modes of operation: off, constant voltage, and constant power. Load changes and variations in generator output cause
the interface converters to switch between constant voltage and constant power operation, changing the level of the dc bus.
The utilization priority of each source is therefore dependent on the discharge/charge thresholds, hence, a control law is
implemented by prioritizing these thresholds. 

```The use of DBS to schedule interface converters supplying power to a nanogrid, or discharging.
The example system, comprises a renewable source, a nonrenewable source, and a constant power load.
The control law for the system has two operating states to prioritize the utilization of these sources.
In state 1, only the renewable source is online, and in state 2, the nonrenewable source comes online.
The control law is implemented by assigning the renewable source to discharge at threshold V0, and the 
nonrenewable source to discharge at threshold V1.
```
