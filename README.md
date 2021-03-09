# REE-Data-Processing
#This Python script is being developed to process and analyze calorimetry experiments performed on rare earth elements
## **Abstract**

#A series of calorimetry experiments were performed on Rare Earth Elements (REE) of the Lanthanide Series in order to empirically determine the enthalpy of reaction. The Lanthanide Series elements were  precipitated in the form of phosphates in a calorimeter. The standard enthalpy of reaction for a precipitation reaction of the Lanthanide phosphates can be calculated if the concentration, masses and the change in the temperature of the reaction is carefully measured. For this project, the Lanthanides studied included Cerium Phosphate, Neodymium Phosphate, Praseodymium Phosphate and Samarium Phosphate. Additionally, experiments were performed containing a mixture of endmembers along a solid solution. Relevant data collected during experimentation included the change in temperature, enthalpy values, the mass and concentration of aqueous species and preciptates. For this project, a robust graphical and statistical analysis was run on the on the data. The standard enthlapy of reaction for the lanthanide phosphates was the main emphasis of study in this project. A thorough graphical and statisticial analysis of the enthalpy data collected for the Lanthanide Phosphates was produced in this project.

## **Introduction and Background**

Rare Earth Elements (REE) have become an increasingly important resource as they have many uses in the production of electronics, car batteries, magnets and defense equipment, to name just a few of its uses. The majority of REE currently is mined and processed in China. Given the value of REE and the fragile relationship the US has with China, the US is attempting to mine REE domestically. 

This specific project was started by Alex Gysi in order to gain a better understanding of the thermodynamic properties of REE in the Lanthanide Series. The long term goal is to gain a more thorough understanding of the pressure and temperature conditions where REE can be found in the earth. 

A colleague and I started performing experiments in the spring of 2020 with Dr. Gysi, but experimentation was halted when the pandemic arrived in the US. Therefore the dataset below is largely incomplete. Hopefully, data collection will resume in the near future. One of the main goals of this project was to build a data loading and analysis script for when the project resumes using the data that has already been collected. 

Four main REEs were tested and analyzed in this project: Cerium (Ce), Neodymium (Nd), Samarium (Sm), and Praseodymium (Pr). The standard enthalpies of reaction required to precipitate each of these elements in the form of phosphates were recorded. Additionally, experiments were run on the solid-solutions of each of these minerals. The majority of this project analyzes how the enthalpy of mixing varies with different solid-solution compositions.

Rare Earth Elements typically precipitate in phosphate rock in very low concentrations. The enthalpy of mixing describes the heat released or absorbed when a substance mixes. In this case, the enthlapy of mixing describes heat absorbed when the mixed lanthanides are precipitated in the form of phosphate. In a non-ideal solid solution containing two components, the activity, also known as the effective concentration, will change based on the mole fraction of the two components in the solution. In this case, there were three solid-solutions analyzed: Cerium-Neodymium, Cerium-Praseodymium, and Cerium-Samarium. Since all three reactions are endothermic, I would expect the enthalpy of reaction to increase as the solution becomes more mixed, then decrease as the mole fraction approaches 100% of either endmember. 

## **Methods**

The data was imported from Google Sheets. The data layout on the spreadsheet was very disorganized, and had to be rearranged in the Google Sheet to make it more pandas friendly. Additional data wrangling and cleaning was then performed using pandas after the data was uploaded into python, and can be seen in the code below. 

A graphical analysis was then performed on the dataset using matplotlib, seaborn and ternary packages. Relevant scatter plots, KDE plots, histograms and box plots can be seen in the graphical analysis section below. 

A statistical analysis of relevant data was then performed using numpy and scipy packages. T-tests and other relevant statistical metrics can be seen in the statistial analysis section below. 
