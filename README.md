#########################################################################################################
# Motion Analysis for Ca Imaging 

Need:

0. Install ezTrack (https://github.com/denisecailab/ezTrack)
1. Overhead view of a video (.mp4)
2. Fully pre-processed cell data that has been behaviorally aligned with arduino data (.csv)

[Example:  DS12-S6, P5-5]
#########################################################################################################
# Motion_Extract with ezTrack (Freezing detection) (modified to also detect intensity changes in LED timestamps)
(doi: 10.1038/s41598-019-56408-9.)

Use ez Track environmnet (script:  Ka_Step_1_MotionExtract.ipynb)


![Fig_1](https://github.com/user-attachments/assets/d2bbdfc5-1288-4614-8b2c-cdf6b705b82b)


![Fig_2](https://github.com/user-attachments/assets/5182daca-5d07-493b-a5b2-f8a7e860d75c)



#########################################################################################################
# Align with Ca Imaging data (5s + whole session alignment, result locomotion trace will be in 20 frames/s)

Use ka_Ca_Imaging environmnet (script:  Ka_Step_2_Alignment_W_5_SecondPulse_Plus_WholeSession.ipynb)

* Adjust thresholds as needed (the LED signal amplitdue is influenced by the signal extraction from the previous step)

1. Look at the length of the Imaging file (.csv) and input that length.  
2. Make sure the duration of 5s pulse (in frames) falls within the two red line AND the number of 5s pulse is 481 (for a 40 minute session)
3. Session onset and End is correctly identified
4. The 5s pulses are correctly identified
5. Infared port activities are correctly identified 

![Fig_3](https://github.com/user-attachments/assets/407265e9-cac0-463e-96ce-4a0827608a90)




#########################################################################################################
# Re-threshold locomotion data 

Use ka_Ca_Imaging environmnet (script:  Ka_Step_4_Threshold_and _BinnedTime.ipynb)

1.  Look at the video file (.mp4) and see the first time when the session indicator light turns on, put the time (in seconds) to the script
   (In this case,  the Ca imaging session starts at 45 seconds).  This is only important for labeling time for manual verifications, but it is not important for the     actual Ca Imgaging analysis.  

![Fig_4](https://github.com/user-attachments/assets/fd7b6963-20b6-4034-a9ba-c0003bb28ed1)



#########################################################################################################
# Human manual verification of locomotion (1s bin) 


#
