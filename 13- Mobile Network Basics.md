## Mobile Network Basics
* **Radios and mobiles:** works with non-ionizing radiation

<img width="793" height="443" alt="image" src="https://github.com/user-attachments/assets/c9073fce-c18c-4786-9106-dee9ed3dc429" />

* **ISM Band (Industrial, Scientific & Medical Band):** it's an unlicensed frequency band which does not require a permit (license) from MinTIC. Common bands are 5 GHz and 2.4 GHz (in Tx microwaves and WiFi)
* $P_{Tx}$ > 1W Requires license
* $P_{Tx}$ 1 smartphone  <= 600 mW = 0,6 W

<img width="741" height="356" alt="image" src="https://github.com/user-attachments/assets/51dc0825-a521-48e2-984d-378dded537f9" />

### Mobile Networks (cellular networks)
They are wireless communication systems that allow mobile devices to connect to a telecommunication network to make calls, send messages, connect to the internet, and perform other functions. These networks use **radio waves** to transmit data and voice between the mobile device and the network infrastructure.

#### Mobile Network Components
* **Cell towers (base stations):** These are structures that contain devices that transmit and receive radio waves
* **Mobile devices:** Smartphones, tablets, and other devices that connect to the network
* **Network infrastructure:** Wires, devices, and servers that manage the data and voice transmission.
* **Core network switching centers:** these feature technology that enables network management and access to telecommunications services.

## How a cellphone works?
1. The microphone transforms your voice (an analog signal) into a digital signal (consisting of 0s and 1s) with the help of a MEMS sensor. This digital signal, containing your voice in binary format, is then received by the cellphone's antenna, which transmits it as an electromagnetic wave.

2. To enable the propagation of the electromagnetic wave, the system utilizes base station antennas.

3. In cellphone technology, a geographic area is divided into hexagonal cells. Each cell is equipped with its own base station antennas and frequency band. Every antenna site is connected to the others via fiber optic cables. These cables are located underground or undersea to provide national and international connectivity.

4. The electromagnetic waves produced by your cellphone are received by the base station antennas and transformed into high-frequency light pulses. These light pulses are routed to the base transceiver station (BTS) box located at the base of the tower for processing. Later, the voice signal is routed to the destination base station, which receives the pulses and radiates them as an electromagnetic wave. Finally, your friend's cellphone receives the signal, where it undergoes an inverse process: digital-to-analog conversion through the earpiece.

### How mobile networks can locate your friend's antenna?
1. For this process, the base station antenna receives information from the Mobile Switching Center (MSC), which acts as the central point for a group of base station antennas.
2. When you buy a SIM card, all subscription information is registered in a specific MSC. This MSC is your Home MSC, which stores information such as your service plan, current location, and activity status.
3. If you move out of coverage of your Home MSC, the new MSC that serves you is known as a Foreign MSC (or Visited MSC), which communicates with your Home MSC.

### Determining a Client's Position Within a Cell Inside an MSC Zone: MSC Location Update Techniques
1. **Periodic Location Update:** The cellphone updates its location at predefined time intervals (time-based tracking).
2. **Zone-Based Location Update:** The cellphone triggers a location update when it crosses into a new designated tracking or routing area after passing a specific number of antennas (location area-based tracking).
3. **Power-On Location Registration:** The cellphone automatically registers its location the moment the device is turned on.

## Process 1 (The Receiver is Located Within Their Home MSC)
Emma wants to call John. When Emma dials John's number, the call request arrives at Emma's Home MSC. Once Emma's MSC receives John's number, the request is routed to John's Home MSC. At that moment, John's MSC checks his current status. If John is within his Home MSC zone, the call request is immediately sent to his cellphone's location. The network then validates whether John is busy on another call or if his phone is turned off. If all validations are successful, John's phone rings and the call is connected.

### Process 2 (The Receiver is Located Outside Their Home MSC)
In this case, the **Home MSC simply routes the** call request to the **Foreign MSC**. It then follows the **previously explained steps** to locate **John's** phone and establish the call.

### Importance of the Frequency Spectrum in Mobile Networks
To transmit binary data, each client requires a frequency range. However, the frequency spectrum for mobile communications is limited, and there are billions of users. This problem is resolved using two technologies:
1. **Frequency Band Allocation:** Different frequency bands are assigned carefully to different base station antennas.
2. **Multiple Access Techniques:** The frequency band is allocated efficiently among all active users within the cell area.

### Why There Are Different Mobile Technology Generations
* **1G:** Enabled users to use a wireless cellphone, but it suffered from two main drawbacks. First, wireless communication used analog signals, which were easily distorted by external sources, resulting in poor voice quality and low security. Second, it used Frequency Division Multiple Access (FDMA) inefficiently.
* **2G:** Introduced digital multiple access techniques such as Time Division Multiple Access (TDMA) and Code Division Multiple Access (CDMA). In addition, it introduced data services like SMS and basic internet browsing (with a data rate of around 50 kbps).
* **3G:** Introduced faster data transmission and Wideband Code Division Multiple Access (WCDMA), achieving a data rate of up to 2 Mbps. This enabled data transmission for GPS, videos, and higher-quality voice calls.
* **4G:**  Delivered significantly higher data rates (20 - 100 Mbps), allowing high-definition video streaming and television. This was possible due to Orthogonal Frequency Division Multiple Access (OFDMA) and Multiple-Input Multiple-Output (MIMO) technology.
* **5G:** : Provides ultra-fast data rates of up to 10 Gbps by utilizing Advanced MIMO and millimeter waves (mmWave), offering the necessary infrastructure for reliable IoT (Internet of Things) communication.

### Extra information

<img width="770" height="472" alt="image" src="https://github.com/user-attachments/assets/27640b55-2801-4e18-a3e1-2d06206ef387" />

<img width="797" height="461" alt="image" src="https://github.com/user-attachments/assets/358acfa2-3aa9-4f8b-b28f-0ccf6c7cea31" />

<img width="727" height="472" alt="image" src="https://github.com/user-attachments/assets/1d1d6277-979f-4e3d-894d-fba499018c14" />

<img width="673" height="472" alt="image" src="https://github.com/user-attachments/assets/002424bb-6597-4cd7-9116-d12306c44cfd" />

<img width="757" height="446" alt="image" src="https://github.com/user-attachments/assets/87937857-0ee1-4f0a-985d-bc51e1569c66" />

<img width="766" height="490" alt="image" src="https://github.com/user-attachments/assets/69247ea5-3188-4910-9d99-caaddbb8c6bf" />
