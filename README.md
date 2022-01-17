# Urban-Block-Generator
Grasshopper script for adaptive generation of shop house units with balconies within urban blocks.

![](Urban-Block-Generator/sample-preview.png)

Generative rules:

- The script verifies if the parcel boundary is within the user determined plot size requirements. If it is out of bounds, the output will flag that the land parcel area is exceeding/under the size limit.
- In no case does the overall building footprint exceed the site coverage percentage.
- The floor count (3-5) is a function of plot ratio and site coverage percentage. Once the site coverage is maximised, the plot ratio is maximised as well by increasing the number of floors. Balconies and terraces are considered part of the overall GFA.
- Balcony flat roofs are generated at random locations (edge or middle of the shophouse unit block).
- Vehicular access is also added for each block at the side of the front road edge.
- The internal shops are generated if the parcel is very large, i.e. the site coverage is yet to be maximized. If the parcel size is small, the internal shops are not created.

The grasshoper script has the following plugin dependencies:

- Pufferfish, Version=2.9.0.0
- NumericalEnvironmentForGH, Version=1.0.0.0
- Human, Version=1.7.2.0

