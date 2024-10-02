# CMOS-Inverter-Design-and-GDSII-Generation-using-Cadence-Virtuoso-GPDK90-
This repository contains the design and analysis of a CMOS inverter using Cadence Virtuoso with GPDK90 technology. The project includes schematic and layout design, pre-layout and post-layout simulations, delay calculations, RC parasitics extraction, and final GDSII file generation.


The goal of this project was to successfully implement the design and perform a detailed analysis to compare pre-layout and post-layout simulation results.

## Tools & Technologies
- **Cadence Virtuoso** 
- **GPDK90 technology**.

I started with creating the schematic of the CMOS inverter and then generated its symbol.
![inv_sch](https://github.com/user-attachments/assets/f3d971e1-1e29-4b44-9145-5f932d00bc63)
Then, using that symbol created a new testbench schematic for getting the simulation results for the inverter.
![inv_tb](https://github.com/user-attachments/assets/c45662ae-9f0f-4d8b-80e8-7889fe0cca98)
Here, is the setup for the analysis for ADE.
![analysis_setup](https://github.com/user-attachments/assets/d328bff5-668f-4da7-a21e-fcd0a5f799ed)
Here are the transient analysis and DC sweep analysis results: Obtained the Volatge Tranfere Charcterstics and the Input and Output waveforms, in turn also calculated the threshold voltage using these results.
![threshold](https://github.com/user-attachments/assets/7b100c04-7dcf-4d43-8732-6f56dcfd2444)
Then, I completed the layout of the inverter.
![inv_lay](https://github.com/user-attachments/assets/64a3302a-abd6-44cd-91c9-7d9d1e5efcb1)
and here are the LVS and DRC check results:
![drc_check](https://github.com/user-attachments/assets/02eacb31-c253-4987-a5a6-d7a3b74e2638)
![lvs_check](https://github.com/user-attachments/assets/f79f7802-def9-4bae-9d16-5ee6bcde99b5)
![lvs_results](https://github.com/user-attachments/assets/dc69ede2-6cf8-46cc-92c8-9cefa9fc0f79)
Then, extracted the RC parasitics:
![rc_extr](https://github.com/user-attachments/assets/520e31ff-e19b-4d75-90a5-f86d82034f4d)
![rc_zoom](https://github.com/user-attachments/assets/2e7bc75e-37e0-4954-a8fc-2f1c8560ff38)
![rccap](https://github.com/user-attachments/assets/e1e001bd-b7c6-4933-85c9-3426ff44a232).
Now, hereafter i proceeded with making of config file and performed the pre layout and post layout analysis:
![inv_tb_config](https://github.com/user-attachments/assets/e44ec1da-2520-49c1-b058-f5de6d0de991)

### Pre - Layout Results:
![simulation](https://github.com/user-attachments/assets/3bdc41f5-9464-46fa-bc08-dd86324dc49e)
[delay_pre_layout](https://github.com/user-attachments/assets/1f73e199-d834-43f5-8abe-ad753f02587d)

Pre- Layout Delay was calculated to be : ```115.1ps```

### Post - Layout Results:
![post_layout_simulation](https://github.com/user-attachments/assets/b7266eaa-8747-4c5e-97d1-ab6946b39fa5)
![delay_post_layout_simulation](https://github.com/user-attachments/assets/5674c9b5-0b07-4d47-b18c-449a23d14e44)
Post- Layout Delay was calculated to be : ```122.4ps```

Next, Obtained the GDS:
![gds_export](https://github.com/user-attachments/assets/e03f77d5-74ea-4e58-9879-507c96b4f164)
![gds_layout](https://github.com/user-attachments/assets/27813c37-e44f-43ff-9660-b24404e8875b)


  

