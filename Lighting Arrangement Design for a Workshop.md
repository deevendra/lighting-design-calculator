Lighting Arrangement Design for a Workshop 
This repository features a Python-based tool I've created for designing the lighting arrangement and calculating fixture requirements for a workshop. This project represents a hands-on exploration in electrical design, applying fundamental illumination principles to streamline lighting planning.

Project Overview
This calculator helps determine:

The optimal number and initial spacing of lighting fixtures.

The total luminous flux (lumens) required on the working plane.

The necessary flux emitted and wattage per fixture.

The actual illuminance level achieved based on a chosen fixture wattage.

How to Use
To use this lighting design calculator, simply run the Python script.

Save the Code: Copy all the Python code provided in the "Python Code" section below into a single file named lighting_calculator.py.

Run the Script: Open your terminal or command prompt, navigate to the directory where you saved the file, and execute it using Python:

📊 Sample Output
Running the above script with its predefined parameters yields the following results:

area= 900

spacing= 7.5

rows= 2.0 

columns= 8.0

number of locations/fixtures= 16.0

total flux recieved/required on working plane in lumen= 90000

flux emitted per fixture= 17578.124999999996

wattage per fixture= 1098.6328124999998

actual wattage per fixture=  1100

actual flux emitted=  281600.0

actual flux received =  90112.0

actual flux density= 100.12444444444445

📐 Underlying Principles & Formulas
This calculator employs the fundamental Lumen Method (also known as the Zonal Cavity Method), a standard engineering approach for general lighting design. The calculations involve:

Spacing-to-Mounting Height Ratio (SHR): Used to determine appropriate fixture spacing: s=SHR×h

Room Area: Basic geometric calculation: Area=l×b

Number of Fixtures/Locations: Based on room dimensions and calculated spacing: n=(width/spacing)×(length/spacing)

Total Required Luminous Flux (f): The total light needed on the working plane: f=E×Area

E: Desired Illuminance (Lux)

Flux Emitted Per Fixture (fe): Calculates the light output each fixture must emit:


fe= 
n×e×m
f
​
 
e: Efficiency of the lamp/luminaire

m: Maintenance Factor (accounts for light loss over time)

Wattage Per Fixture (wl): Determines power consumption based on efficacy:


wl= 
ef
fe
​
 
ef: Efficacy of the lamp (lumens per watt)

Actual Illumination (Ea): Verifies the illuminance achieved with selected fixtures:


Ea= 
Area
actual wattage per fixture×n×ef×e×m
​
 
This systematic approach provides a practical framework for efficient lighting design.

🛠️ Technologies Used
Python: The core programming language for all calculations.

🌱 My Learning Journey & Insights
As a fresher exploring the vast field of electrical design and automation, this project has been a valuable step in bridging theoretical knowledge with practical application. I particularly enjoyed:

Translating engineering formulas into functional code: This process deeply solidified my understanding of lighting design principles and the relationships between various parameters.

Understanding parameter impact: Seeing how changes in room dimensions, fixture properties, or efficiency factors directly influence the overall design and required components.

The iterative nature of design: Realizing how initial calculations lead to practical component selection, followed by verification of the actual outcome.

This project represents a tangible step in my journey to understand and contribute to smart, efficient, and reliable electrical solutions.

💡 Future Enhancements
Future iterations and explorations for this calculator could include:

Interactive Input: Implement a more user-friendly interface using a GUI library (e.g., Tkinter, PyQt) or a web framework.

Fixture Database: Create a predefined list of common light fixtures with their standard lumen outputs and efficacies for easier selection.

Room Type Presets: Offer common desired lux levels based on typical room categories (e.g., "Living Room," "Office," "Industrial Workshop").

Room Cavity Ratio (RCR) Calculation: Integrate RCR for more precise Coefficient of Utilization (CU) determination.

Energy Efficiency Metrics: Add calculations for power density (W/m²) and estimated annual energy consumption.

📄 License
This project is open-sourced under the MIT License. See the LICENSE file for more details.
