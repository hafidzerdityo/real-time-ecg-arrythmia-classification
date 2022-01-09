
Hardware Used:
1. Arduino UNO
2. AD8232 ECG sensor and 3 electrode

Software:
1. Arduino IDE
2. Python IDLE
3. ECG Dataset from physionet.org (feature already extracted at Dataset.csv)

Using python library "Serial", you can communicate arduino serial monitor value to python.
Low pass filter, and cubic spline interpolation is used to eliminate unecessary noise, so you can detect r peak easier.
Classification is done using artificial neural network, using MLPClassifier from sci-kit learn.
Monitoring done in 60 seconds, and every 1 seconds ECG curve will updated while also showing BPM,SDNN,RMSSD,PNN50 value in real time via matplotlib.
After 60 seconds, system will automatically determine one of the two classes, which Normal Sinus Rythm or Arrythmia.
