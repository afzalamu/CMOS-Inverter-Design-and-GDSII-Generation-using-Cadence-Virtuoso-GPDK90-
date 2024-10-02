# CMOS Inverter Design and GDSII Generation using Cadence Virtuoso (GPDK90)

This repository documents the design and analysis of a CMOS inverter using **Cadence Virtuoso** with **GPDK90 technology**. The project covers the entire workflow from schematic design to GDSII generation, including pre-layout and post-layout simulations, delay calculations, RC parasitics extraction, and validation through DRC and LVS checks.

The goal was to successfully implement the CMOS inverter design and perform a detailed comparison between pre-layout and post-layout simulation results.

## Tools & Technologies
- **Cadence Virtuoso**
- **GPDK90 technology**

## Project Workflow

1. **Schematic Design**: Created the schematic for the CMOS inverter and generated its symbol for further use.
   ![inv_sch](https://github.com/user-attachments/assets/f3d971e1-1e29-4b44-9145-5f932d00bc63)

2. **Testbench Setup**: Designed a testbench for simulating the inverter's behavior.
   ![inv_tb](https://github.com/user-attachments/assets/c45662ae-9f0f-4d8b-80e8-7889fe0cca98)

3. **Analysis Setup**: Configured the Analog Design Environment (ADE) for transient and DC sweep analyses.
   ![analysis_setup](https://github.com/user-attachments/assets/d328bff5-668f-4da7-a21e-fcd0a5f799ed)

4. **Simulation Results**: Performed transient and DC sweep analyses to obtain the **Voltage Transfer Characteristics (VTC)** and **threshold voltage**.
   ![threshold](https://github.com/user-attachments/assets/7b100c04-7dcf-4d43-8732-6f56dcfd2444)

5. **Layout Design**: Completed the physical layout of the CMOS inverter, ensuring design integrity.
   ![inv_lay](https://github.com/user-attachments/assets/64a3302a-abd6-44cd-91c9-7d9d1e5efcb1)

6. **DRC & LVS Checks**: Successfully cleared Design Rule Check (DRC) and Layout Versus Schematic (LVS) checks.
   ![drc_check](https://github.com/user-attachments/assets/02eacb31-c253-4987-a5a6-d7a3b74e2638)
   ![lvs_check](https://github.com/user-attachments/assets/f79f7802-def9-4bae-9d16-5ee6bcde99b5)
   ![lvs_results](https://github.com/user-attachments/assets/dc69ede2-6cf8-46cc-92c8-9cefa9fc0f79)

7. **RC Parasitics Extraction**: Extracted the parasitics from the layout to understand the impact on performance.
   ![rc_extr](https://github.com/user-attachments/assets/520e31ff-e19b-4d75-90a5-f86d82034f4d)
   ![rc_zoom](https://github.com/user-attachments/assets/2e7bc75e-37e0-4954-a8fc-2f1c8560ff38)

8. **Pre-Layout and Post-Layout Simulations**: Performed simulations to compare performance before and after layout.

   - **Pre-Layout Results**:
     ![simulation](https://github.com/user-attachments/assets/3bdc41f5-9464-46fa-bc08-dd86324dc49e)
     Delay: **115.1 ps**
     
     ![delay_pre_layout](https://github.com/user-attachments/assets/1f73e199-d834-43f5-8abe-ad753f02587d)

   - **Post-Layout Results**:
     ![post_layout_simulation](https://github.com/user-attachments/assets/b7266eaa-8747-4c5e-97d1-ab6946b39fa5)
     Delay: **122.4 ps**
     
     ![delay_post_layout_simulation](https://github.com/user-attachments/assets/5674c9b5-0b07-4d47-b18c-449a23d14e44)

9. **GDSII File Generation**: Exported the final GDSII file for tapeout.
   ![gds_export](https://github.com/user-attachments/assets/e03f77d5-74ea-4e58-9879-507c96b4f164)
   ![gds_layout](https://github.com/user-attachments/assets/27813c37-e44f-43ff-9660-b24404e8875b)

## Conclusion
This project successfully completed the design, simulation, and layout of a CMOS inverter using Cadence Virtuoso. The pre-layout and post-layout results were compared, revealing a slight increase in delay post-layout, as expected due to parasitics. The final GDSII file is ready for fabrication.


## License
This project is licensed under the MIT License.
