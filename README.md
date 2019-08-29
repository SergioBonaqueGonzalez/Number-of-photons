# Number-of-photons
Calculates the number of photons emmited by a light source and reaching a defined plane

Developed by Sergio Bonaque-González, PhD.

sergiob@wooptix.com

www.linkedin.com/in/sergiobonaque

September,2019 - Wooptix S.L.

According to the equation E=n*h*v (energy = number of photons times Planck's constant times the frequency), 
if you divide the energy by Planck's constant, you should get photons per second.

%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%

In the first function 'Calc_nphot_collimated.m', it is supposed to be a collimated monochromatic punctual light source, where all the emitted photons are reaching the detector.

[nphot]=Calc_nphot_collimated(exposuretime,power,lambda)

INPUTS:
- exposuretime = exposure time in seconds
- power = Source power in W
- lambda = %wavelength in meters

%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%

In the second function, it is supposed a light source with a uniform radiation across all
directions. So, the distance between the source and the entrance pupil of the system should be considered.

[nphot]=Calc_nphot_uniform(sourcedistance,power,exposuretime,area,lambda)

INPUTS:
- sourcedistance = distance in meters from the light source to the image
plane.
- power = Source power in W.
- exposuretime = exposure time in seconds.
- area = area of the image plane in meters. (i.e. area of a detector or the
entrance pupil of the optical system.
- lambda = %wavelength in meters.
