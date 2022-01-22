# real-time-ecg-arrythmia-classification


This Projects is done using:
- Hardware:
  > Arduino
  > ad8232 ECG sensor
  > Some jumper and breadboard
  
- Software:
  > Arduino IDE
  > python, VSCode and Jupyter Notebook
  
- Method:
  > Low pass filter
  > Cubic spline interpolation
  > r peak detection
  > statistic for feature extraction
  > machine learning(Neural Net)
 
 This system will detect raw signal from ad8232 sensor and arduino from 60 seconds, and displaying every features such as Heart Rate, SDNN, RMSSD in real time
 and displayed on matplotlib GUI.
 After 60 seconds, system wil able to classify if the patient have Arrythmia or Normal Sinus Rythm.
