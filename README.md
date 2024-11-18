Ex No: 04-Design-Implementation-of-6T---SRAM-Cell-using-Cadence-EDA-Tools
Aim:
To design and implement a 6T SRAM (Static Random-Access Memory) cell using Cadence EDA tools, simulate its functionality, and analyze key performance parameters such as read/write operations, power consumption, and stability to understand its behavior in memory design.

Tools Required:
Personal Computer
Cadence Virtuoso Software
Circuit Diagram:
WhatsApp Image 2024-11-13 at 16 25 39_50eac1b6

SCHEMATIC SIMULATION:
PROCEDURE FOR CREATING THE SCHEMATIC SIMULATION Commands to get into Cadence:

Right Click and open the terminal window
Type the following commands as follows and press enter. • csh • source /cadence/install/cshrc • virtuoso
Procedure for Schematic simulation using Cadence
Now two windows must open i) virtuoso/command interpreter window ii)”Whats New…”

Close the 2nd window

Use 1st window i.e virtuoso window (CIW) for further processing.

Create a New Library
Create Schematic Cell view.
Create the Symbol for schematic Cell view.
Create the test Cell view.
Analog simulation by spectre
Steps for Schematic Simulation using Cadence:
i) Procedure for Creating New Library.

File –New – Library
Name: Give name for ur library Ex: VLSILAB_EXP_1
Enable Attach to an existing technology library, Click OK
Attach the library to the technology library gpdk045.Click OK.
ii) Create Schematic Cell view.

Go to 1st window i.e virtuoso (CIW)

File-New-Cell view

Setup the new file form

Library: Select the one you created.
Cell: Give the experiment name Ex: Inverter ViewSchematic
Type: Schematic press OK
Add the required components from the libraries and make the connections.

Go to instance fixed menu or use shortcut key “I” from keypad to go instances
Click on browse. This opens the library browser
Now select the appropriate library for components like
Gpdk45 ------------------------nmos1v, pmos1v
Create Input and Output pins
Make the connections by using fixed narrow wire key
Click Check and Save button
iii) Creating the Symbol for schematic Cell view

In the schematic window, execute
Create – Cell view – From Cell view
The cell view from cell view window appears
Check Lib Name, Cell Name, From View name must be schematic Press ok
Now Symbol generation form appears. Click Ok If No changes required
A new window with with default symbol is created.
Edit the symbol if you want to give actual symbol shape else continue.
Execute Create-Cell view-from cell view
Library Name and Cell Name must be same which you have used for schematic. Press OK
Check for the position of pin side.Prss OK
Edit for the shape by Create-Shape-Choose required options to edit.
iv) Creating the new test cell view

Go to CIW window, Execute File-New-Cell view

Setup the new file form
Library: Select the one you created.
Cell: Cell name must be different from the name used in schematic cell view. Ex: Inverter_test
View: Schematic
Type: Schematic press OK
Follow the step 3(ii) d to make the required connections
WhatsApp Image 2024-10-19 at 10 41 43_ded08126

Analog simulation by SPECTRE.
In test cell view window
Launch – ADE L(Analog Design Environment)
Execute Setup—Simulation/directory/Host A new window opens
Set the simulation window to spectre and click ok
Execute Analysis – Choose. A window opens.
Select the type and set the specifications and press OK
Execute Output s—to be plotted – Select on Schematic
Then Select the INPUT WIRE(Vin ) and OUTPUT WIRE(Vout) from your test Schematic using mouse
Execute Simulation -- Net list and Run
Screenshot 2024-11-17 225149

For DC Analysis Settings and Output
In the simulation setup, choose DC analysis.
Specify the time range for the analysis (start and stop time).
Run the simulation and observe the output waveforms
Screenshot 2024-11-12 125526

Screenshot 2024-11-12 125609 Screenshot 2024-11-12 125544 Screenshot 2024-11-17 225344

Results:
The design and implementation of the 6T SRAM cell using Cadence EDA tools were successfully achieved. Simulation results validated the correct functionality and performance of the SRAM cell, including stable read/write operations,
