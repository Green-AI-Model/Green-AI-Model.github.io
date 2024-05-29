+++
title = '2. Quantifiying the Environmental Footprint'
weight = 2
+++
# Quantifiying the Environmental Footprint
![](../figures/placeholder_green_ai.png)

> **Central Question**  
> - What is the ecological Footprint of AI Applications and why do we need it?  
>    -> To mitigate the ecological Impact of AI and this is only possible, if you can quantify the impact!

## Why is it important to know the footprint
Understanding the ecological impact of AI systems is crucial for effective mitigation efforts. For instance, simply replacing old hardware with new, more energy-efficient models can ironically result in a larger overall CO2 footprint when considering the emissions associated with producing new hardware and disposing of the old. Thus, before making optimizations, it's essential to fully understand the potential environmental benefits, which can only be achieved by comprehensively quantifying the entire footprint of the system.

## What are the environmental influences and sources for this?
Since AI-Systems are complex systems, so is their environmental influences. 
The complete footprint consist of multiple factors, first the execution on Hardware (energy consumption). Second the Infrastructure that is needed for this execution, e.g. the Data Center but also the Offices for workers. In infrastructure, emissions are mainly in the form of embodied emissions, but also water that is used to cool the servers and more. Last the Human that is tied to the development, marketing etc. of the AI-System. Life-Cycle-Assessment provides an effective framework for evaluating these emissions.

## But how do we measure those impacts?
The tricky part comes, when you try to measure those emissions. Measuring the energy-consumption of AI-Systems can be done in several ways, with both benefits and downsides. The most accurate would be to measure the energy-consumption with a power-meter. But sometimes you do not have Access to the machine or a capable power meter. Then the energy-consumption could be estimated by softwaretools, such as RAPL or NVIDI-SMI, wich is more accessible and easier to use but not as accurate.  Last, if you do not have Hardware that supports those Tools, you could estimate the energy-consumption by taking the time and utilisation of the system and combining it with the TDP of the system. Even this is impossible if you are on a public cloud and do not know the TDP of your system. Depending in the hardware used, there a other ressources that need to be measured. E.g. for Data Center with water-cooling, the water consumption plays an important role as well. 
No matter where the AI-System runs, it requires Hardware that comes with a CO2 footprint for its production and transport to the execution location. This is something that can't be measured. There you have to relay on estimations, if any exist. But even after use, the hardware could produce significant environmental impacts, since it has to be disposed or in best case recycled or reused.


## How do we report our results?
After measuring your System, you need to Report the numbers. Here it is very important to report the right number to the right audience. For example reporting the CO2 Footprint of a trained model to the public would be a good choice if other models to do the same. That way customers could choose the more environmently friendly model. But for a scientific audience this might be not enough. Maybe they want to compare your Architecture with theirs. Then they also need to know on what Hardware and how much energy it requires.

