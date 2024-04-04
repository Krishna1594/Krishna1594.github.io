---
title: Visualizing Satellite Orbits using Matlab
tags: [Matlab, Astrodynamics, Planetary Science, Data Visualization, 3D-Mesh]
style: Border
color: secondary
comments: true
description: A method in matlab to visualize the orbits of satellites around the Earth at a given time.
---

![preview](https://i.postimg.cc/rmJVBDkW/satellite-orbit-info.png)
#### Source: Dewesoft [link](https://dewesoft.com/blog/every-satellite-orbiting-earth-and-who-owns-them)

## The Purpose of this visualization
I really gave this a thought and my reason is simple. Most of the time when I begin analysing a dataset, I simply use a function I know and my results appear or I search for such functions online and use them simply to get my results but what is the mathematics behind it. Did I forget the mathematics? I am an engineer, I rely on equations to solve problems. So, here I am telling my laptop how to use mathematics and visualize satellites orbittintg around our planet. I want to know the mathematics involved in this topic. A data analyst should also know the mathematics behind the analysis. I can confidently apply this idea to my data; geoscience or data science. Alas! I love astronomy too.

### Satellite Data
Probably the complex imagination is being able to pin-point the position of objects in space. We need a coordinate system to effectively understand the behaviour of space and track the movements of objects in space. Such cordinate system called '3-Dimensional Cartesian Coordinate System', is used for understanding and navigating objects and phenomena in space, from celestial bodies and satellites to spacecraft and space missions. It provides a standardized framework for describing positions and movements in the vastness of the cosmos.

#### Data Format: Introducing TLE
A two-line element set (TLE) or three-line element set (3LE) is a data format encoding a list of orbital elements of an Earth-orbiting object for a given point in time, the 'epoch'. The United States Space Force tracks all detectable objects in Earth orbit, creating a corresponding TLE for each object, and makes publicly available TLEs for many of the space objects on the websites Space Track and Celestrak, except classified objects. The TLE format is a standard for distribution of an Earth-orbiting object's orbital elements.

If you want to know how to comprehend a TLE file, then please refer [here](https://en.wikipedia.org/wiki/Two-line_element_set).

#### Data Sources
I needed the latest orbital details of satellites so, I leveraged [celestrack](https://celestrak.org/satcat/search.php)'s database to gather information of satellites and thier orbital data. There are other sources but requires registration. I donwloaded the TLE files of satellites are operational. 

In this visualization, I searched for Medium Earth Orbit (MEO) satellites and couple of Low Earth Orbit (LEO) satellites to understand the magnitude of the distance and how cloose satellites actually revolve around Earth. I googled some MEO satellite names and searched for data in Celestrak. Once you get the TLE data, I copied and pasted the 2 lines in the '.txt' file.

#### Mathematics involved
To visualize Earth and orbits of satellite, we need 3-D co-ordinate systems for spherical objects (however, Earth is not exactly a sphere, but instead is a Spheroid. This is the closest approximation in our case.). The following equations enables us to imagine a 3D object using cartesian system:

![preview](https://i.postimg.cc/fTG61t2B/spherecoord.png)

The same can be replicated in matlab using 'Mesh":

<script src="https://gist.github.com/Krishna1594/05017a216dac3cf422e3d6be04b0991d.js"></script>


