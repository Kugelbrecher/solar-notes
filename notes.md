# <center>Photovaltaic Notes</center>

In a solar facility, sunlight is captured by photovoltaic (PV) modules series-connected into strings. These strings transform the solar energy into direct current (DC). The DC then travels to a junction box that groups parallelly aligned, electronically identical strings. This box is equipped with diodes, an isolator, and fuses to provide protections such as preventing reverse current flow and overheating of individual strings.

Next, the DC flows into the inverter, and is converted to alternating current (AC) that can be used to power our homes. The inverters also help to monitor maximum power (MPP) and other operation data. Self-commutated inverters are widely used in this process for their ability to switch on and off, generating a sinusoidal current wave. While transformers within inverters provide electrical isolation and minimize interferences, transformerless inverters have the highest efficiency due to the elimination of energy loss.


----
## **1. Photovoltaic (PV) Modules**

PV: The process of converting light (photons) to electricity (voltage).

PV Modules: modules are connected in series and parallel. As shown in table below:

|  | **series connection** | **parallel connection** |
| --- | --- | --- |
| **system** | grid-connected PV system | stand-alone PV system |
| **current(in A) vs. voltage(in V)** | same current, add up voltage | same voltage, add up current |
| **name** | string | - |
| **structure** | <img src='./src/pvmodseries.png' width='300' height='200'/> | <img src='./src/pvmodparallel.png' width='300' height='200'/> |

Note: 
- Use same type of modules to avoid power loss. Same type means same manufacturer, model, etc.
- We also want the module to be electrically identical, meaning same current and voltage.


----
## **2. PV Array Junction Box**

Purpose: combine all parallelly aligned strings into one DC output. As shown in image below:
<img src='./src/pvarray.png' width='500' height='300' />


Components: diodes, isolator, fuses, DC main cable
- fuses: 
  - protect wiring against overloading
  - it will blow when current exceeding has occurred
- diodes: 
  - used to decouple individual module strings
  - if short circuit or shading occurred for one string, other strings should not be affected, meaning current will not flow back through the failed string??
- isolator:
  - functions mainly to switch off, isolate, and protect the system, eg when testing or maintenance
- DC main cable:
  - connects the junction box to the inverter


----
## **3. Inverter**
Definition: DC-AC converter, link between PC array and AC grid/load. As shown in image below:

<img src='./src/invertersymbol.png' width='100' height='100' />

Funtions:
- convert DC to AC
- adjustment of the inverter’s operating point to the MPP of the PV modules (MPP tracking)
- recording of the operating data and signalling (e.g. display, data storage and data transfer)
- Grid monitoring or grid management


Two types: grid-connected inverter and stand-alone inverter. As shown in table below:

|  | **grid-connected inverter** | **stand-alone inverter** |
| --- | --- | --- |
| **components** | bridge circuit with thyristors | blur yet |
| **principle** | <img src='./src/invertergridprin.png' width='300' height='200'/> | <img src='./src/inverterselfcomprin.png' width='300' height='200'/> |
| **wave** | add img | add img, this is more popular |


Due to problem of electromagnetic compatibility (EMC), transformer is introduced to the inverter. It mainly functions to:
- provide electrical isolation
- minimize interferences
- etc

One phase and three phase inverter.

|  | **transformer** | **transformerless** |
| --- | --- | --- |
| **pros** | - | less weight so reduce energy loss |

We also need to compare low-frequency and high-frequency transformer. As shown in table below:

|  | **low-frequency transformer** | **high-frequency transformer** |
| --- | --- | --- |
| **pros** | - | - |


----
## **4. Efficiency Calculation**

Conversion efficiency

Adaptive efficiency

Static efficiency

Euro efficiency

Californian efficiency

Overall efficiency