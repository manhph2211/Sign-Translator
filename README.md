Sign-Translator-Using-Wearables
=====

# Introduction

- Sign Language is a form of communication by people who are deaf, hard of hearing, and non-verbal. This mainly employs signs made by moving the hands, and each individual sign is characterized by:
  
  - Hand shape
  - Hand movement
  - Relative location of two hands

- Over 466 million people(5%, might reach 900M in 2050) are speech or hearing impaired, and 80% of them are semi-illiterate or illiterate(WHO).
  - In US, ASL is a native language for around 2,50,000-5,00,000 people. 
  - In China, Chinese Sign Language is being used in China by approximately 1M to 20M deaf people. 
  - In UK, Approximately 1,50,000 people use British Sign Language (BSL).
  - In India, approximately 1.5 million signers use Indo-Pakistani Sign Language.
 
- SLR is really necessary but not easy to create a tool that meets daily conversation and there are gaps to fill in such as real-time and natural output decoding, sensor selection and placement optimization, and robustness with non-uniform background environments ...

- Proposed pipeline

![image](https://github.com/manhph2211/Sign-Translator/assets/61444616/68110ed0-4e69-4bca-beb6-5e7f889aca52)

# Related Works

- Wearable System for Recognizing American Sign Language in Real-Time Using IMU and Surface EMG Sensors (2016):
  - Fusion IMU and sEMG signals and give suitable feature extraction and selection 
  - Adaptive auto-segmentation to extract periods during which signs are performed using sEMG
  - Proved sEMG is useful to combine by experiments
    
- DeepASL: Enabling Ubiquitous and Non-Intrusive Word and Sentence-Level Sign Language Translation (2017):
  - Uses Leap Motion – an infrared light-based sensing device extracting the skeleton joints information of fingers, palms and forearms
  - Propose 2 branch models for corresponding hands and fusion 

- SignSpeaker: A Real-time, High-Precision SmartWatch-based Sign Language Translator (2019)
  - Using portable and lightweight smartwatch and mobile phone
  - Supporting both fingerspelling and sentence-level using bilstm given extracted spectrogram
  - Additional TTS engine

- SonicASL: An Acoustic-based Sign Language Gesture Recognizer Using Earphones (2021)
  - First method for using Sonic wav(inaudible) + earphones
  - Propose CNN-LSTM CTC 
  - Support TTS engine

- SignFi: Sign Language Recognition Using WiFi (2018 - IMWUT)
  - Collects CSI measurements to capture wireless signal characteristics of sign gestures. 
  - Raw CSI measurements are pre-processed to remove noises and recover CSI changes over sub-carriers and sampling time
  - Only word-level recognition and relatively low accuracy in new-user
 
  
