## Link budget
* A link budget is the accounting of all the gains and losses that a radio signal encounters as it travels from a transmitter, through the air (or a cable), to a receiver.
* It is the primary tool telecommunication engineers use to predict if a wireless system (like Wi-Fi, 4G/5G, or satellite) will have a strong, reliable connection.

#### 1. The Core Equation
* Think of a link budget like a financial budget, where gains are income and losses are expenses. The basic formula is:
* $\(\text{Received\ Power\ (dBm)}=\text{Transmitter\ Power\ (dBm)}+\text{Gains\ (dB)}-\text{Losses\ (dB)}\)$
* To successfully close the link and get a connection, the **Received Power** must be greater than the **Receiver Sensitivity** (the minimum signal the receiver needs to hear data).

#### 2. The Components of a Link Budget
* **Transmitter Power (+ dBm):** The raw electrical power output of the radio hardware.
* **Cable/Connector Losses (- dB):** Signal lost in the wires and plugs between the radio and the antenna.
* **Antenna Gains (+ dBi or + dBd):** The amplification achieved by the transmitting and receiving antennas focusing the signal.
* **Free Space Path Loss (- dB):** The natural weakening of the signal as it travels through the air over a distance.
* **Fading/Obstacle Margin (- dB):** Extra safety cushion added to account for weather, walls, or moving obstacles.

#### 3. Quick Practical Example
Imagine you are setting up an outdoor Wi-Fi link:
* **Tx Power:** +20 dBm
* **Tx Antenna Gain:** +10 dBi
* **Path Loss over distance:** -100 dB
* **Rx Antenna Gain:** +10 dBi
* **Rx Cable Loss:** -2 dB
* **Calculation:** $\(20 + 10 - 100 + 10 - 2 = \mathbf{-62\text{ dBm}}\)$
* If your receiver has a sensitivity of **-75 dBm**, your signal (-62 dBm) is strong enough to connect with a **13 dB safety margin**.
  
<img width="721" height="487" alt="image" src="https://github.com/user-attachments/assets/b8560f3f-50c1-44ae-870f-5e9fc60ba9c7" />

#### Ejercicio

<img width="827" height="502" alt="image" src="https://github.com/user-attachments/assets/6d317599-1a67-4c24-b012-66f965a4a0e8" />

<img width="753" height="482" alt="image" src="https://github.com/user-attachments/assets/6d5b9cc7-91ff-4056-a1fe-e825c406f14c" />

<img width="767" height="502" alt="image" src="https://github.com/user-attachments/assets/2767a78d-b8ae-4590-90bf-9640eb1968be" />

#### Line of sight Fresnel zone
* The Fresnel Zone (pronounced freh-nel) is an elliptical (football-shaped) three-dimensional region of space surrounding the direct line of sight path between a transmitter and a receiver.
* **The Principle:** Radio waves do not travel in a razor-thin straight line; they spread out.
* **The 60% Rule:** For an RF link to be reliable, at least 60% of the first Fresnel zone must be completely free of obstacles (such as buildings, trees, or the ground). If obstacles breach this 60% radius, signal power is severely lost due to diffraction and phase cancellation.
  
<img width="661" height="441" alt="image" src="https://github.com/user-attachments/assets/0fde6c6b-e7df-431f-ad3f-7a619f6afb17" />

### EIRP and ERP
are **absolute units of measurement** in telecommunications that express the **total actual power radiated by an antenna** in its strongest direction. The fundamental difference between the two lies exclusively in the **reference antenna** used to calculate the gain.

#### 1. EIRP (Equivalent Isotropically Radiated Power)
* EIRP compares the performance of your transmission system against a theoretical **isotropic antenna** (an ideal antenna that radiates energy equally in a perfect sphere, with a gain of **0 dBi**).
* **Reference:** Isotropic Antenna (0 dBi).
* **Common Usage:** Wireless networking (Wi-Fi), satellite links, microwave links, and cellular regulatory limits (FCC/IEEE).
* **formula:** $\(\text{ERP\ (dBm)}=\text{Transmitter\ Power\ (dBm)}-\text{Cable\ Losses\ (dB)}+\text{Antenna\ Gain\ (dBi)}\)$

#### 2. ERP (Effective Radiated Power)
* ERP compares the performance of your system against a real-world **half-wave dipole antenna** (which has a natural directional focus and a baseline gain of **2.15 dBi** or **0 dBd**).
* **Reference:** Dipole Antenna (0 dBd = 2.15 dBi).
* **Common Usage:** Commercial broadcasting towers (FM Radio, Television), land mobile radio systems, and lower frequency telecommunications.
* **Formula:** $\(\text{ERP\ (dBm)}=\text{Transmitter\ Power\ (dBm)}-\text{Cable\ Losses\ (dB)}+\text{Antenna\ Gain\ (dBd)}\)$

#### 3. The Conversion Between EIRP and ERP
* Because a physical dipole antenna naturally concentrates a signal more than a theoretical sphere (by exactly 2.15 dB), the EIRP value will always be mathematically higher than the ERP value for the exact same system.
* The direct conversion formulas are:
* $\(\text{EIRP\ (dB)}=\text{ERP\ (dB)}+2.15\)$
* $\(\text{ERP\ (dB)}=\text{EIRP\ (dB)}-2.15\)$
* **Quick Practical Example:** If a cellular base station is transmitting with an **ERP of 100 Watts (50 dBm)**, its **EIRP is 52.15 dBm** (approximately 164 Watts). The hardware emits the exact same amount of energy; only the reference yardstick changes
