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

#Use ez Track environmnet (script:  Ka_Step_1_MotionExtract.ipynb)


![Fig_1](https://github.com/user-attachments/assets/d2bbdfc5-1288-4614-8b2c-cdf6b705b82b)


![Fig_2](https://github.com/user-attachments/assets/5182daca-5d07-493b-a5b2-f8a7e860d75c)



#########################################################################################################
# Align with Ca Imaging data

#Use ka_Ca_Imaging environmnet (script:  Ka_Step_2_Alignment_W_5_SecondPulse_Plus_WholeSession.ipynb)

![Fig_3](https://github.com/user-attachments/assets/cbc9cdf1-39b5-4642-ab73-84040741f6ed)


#########################################################################################################
# Re-threshold locomotion data 



#########################################################################################################
# Human manual verification of locomotion (1s bin) 


#
