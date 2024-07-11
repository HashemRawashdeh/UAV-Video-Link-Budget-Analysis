# UAV Video Link Budget Analysis

<p align="justify">
This project provides high level analysis and design of a UAV video communication link using MATLAB's RF Budget Analysis toolbox, antenna designer toolbox and programming for path loss calculations. The objective is to thoroughly assess the performance of a video link between a Ground Control Station (GCS) and a UAV, which operates at 5 GHz. Design parameters were meticulously researched and selected based on established practices for such applications.
</p>

## Project Overview

### System Block Diagram
![System Block Diagram](./Block%20Diagram.png)
<p align="justify">
This is the full block diagram of the system in Simulink. The design includes essential components such as antennas, amplifiers, and path loss models to accurately simulate a real-world scenario. The system diagram comprehensively illustrates the flow of the signal from the input to the output, ensuring a detailed understanding of each stage in the communication link. The output power available to the user is calculated to ensure adequate performance.
</p>

### Variables and Objects
![Workspace Variables](./Workspace.png)
<p align="justify">
The above image shows the variables and objects gathered from the workspace:
<ul>
    <li><strong>TA</strong>: Transmitter Antenna</li>
    <li><strong>RA</strong>: Receiver Antenna</li>
    <li><strong>PL</strong>: Path Loss</li>
</ul>
</p>

### Path Loss Contour Plot
![Path Loss Contour Plot](./PL.png)
<p align="justify">
This contour plot shows the path loss for a use case where a GCS and UAV are communicating at 5 GHz. The distance between the UAV and the GCS is ~150 km, and the elevation difference is around 500m. The <a href="https://github.com/HashemRawashdeh/UAV-Video-Link-Budget-Analysis/blob/main/Channel.mlx">channel code</a> calculates the distance given the positions of the GCS and the UAV, including elevation, not just movements in the azimuth plane. The path loss value is calculated using the free space path loss model with a path loss exponent of 2, emulating a rural outdoor environment. 
</p>

### Receiver Antenna Design
![Receiver Antenna](./RA.png)
<p align="justify">
This image shows the design of the receiver antenna. The design parameters were chosen to optimize the reception quality and ensure efficient communication between the UAV and the GCS. The receiver antenna design is tailored to the specific frequency and environmental conditions, ensuring that the received signal is as strong and clear as possible.
</p>

### Transmitter Antenna Design
![Transmitter Antenna](./TA.png)
<p align="justify">
This image shows the design of the transmitter antenna. The transmitter antenna was designed to provide sufficient output power to ensure a reliable communication link with the receiver. The design focuses on achieving the required gain and directivity to maintain a robust link between the UAV and the GCS.
</p>
