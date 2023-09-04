Sign-Translator-Using-Wearables
=====

# Introduction

- Sign Language is a form of communication by people who are deaf, hard of hearing, and non-verbal. This mainly employs signs made by moving the hands. However, not only hands, but also palm orientation, movement, location, and expression/non-manual signals, ...  lead to the good performance of the Sign Language Recognition System.

- Over 466 million people(5%, might reach 900M in 2050) are speech or hearing impaired, and 80% of them are semi-illiterate or illiterate(WHO).
  - In US, ASL is a native language for around 2,50,000-5,00,000 people. 
  - In China, Chinese Sign Language is being used in China by approximately 1M to 20M deaf people. 
  - In UK, Approximately 1,50,000 people use British Sign Language (BSL).
  - In India, approximately 1.5 million signers use Indo-Pakistani Sign Language.

- Popular approach: A relay service (text and video based)​
  - Takes extra time, complex settings and inconsistent call ​
  - Only person should talk or type at a time​
  - Sensitive and private information or data & image might be leaked

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
    
- MyoSign: Enabling End-to-End Sign Language Recognition with Wearables (IUI 2019)​
  - Emphasize the application of EMG in SLR
  - Use CNN for feature extraction and then BiLSTM + CTC
    
- GASLA: Enhancing the Applicability of Sign Language Translation (Infocom 2022)​
  - Introduce a method for collecting suitable word and sentence data (synthesized by words)
  - Also use BiLSTM and CTC and use spectrogram as input
  - Focus on the translation task, which is a higher version of the recognition task when outputting spoken text instead of sign text.
    
- WearSign: Pushing the Limit of Sign Language Translation Using Inertial and EMG Wearables (IMWUT 2022)
  - Leverages a smartwatch and an armband of ElectroMyoGraphy (EMG) sensors to capture the sophisticated sign gestures​ to do translation task
  - Introduce a training method with 2 CTC layers and encoder-decoder architecture  together with an attention mechanism.
  - Borrow the idea of back-translation and leverage the much more available spoken language data to synthesize the paired sign language data
