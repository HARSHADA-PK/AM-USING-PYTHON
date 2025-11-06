# AM-USING-PYTHON

# AIM

To implement and analyze Amplitude Modulation (AM) using Python's NumPy and Matplotlib libraries.

# Apparatus Required

1.Software: Python with NumPy and Matplotlib libraries
2.Hardware: Personal Computer
    
# THEORY

Amplitude Modulation (AM) is a technique used in electronic communication, most commonly for transmitting information via a radio carrier wave. In AM, the amplitude of the carrier signal is varied in proportion to the instantaneous amplitude of the message signal, while the frequency and phase of the carrier remain constant.The general form of an AM signal is given by

# Algorithm

1.Initialize Parameters:
Set the values for carrier amplitude, message amplitude, carrier frequency, message frequency, and sampling frequency.

2.Generate Time Axis:
Create a time vector for the signal duration.

3.Generate Message Signal:
Define the message signal as a cosine wave.

4.Generate Carrier Signal:
Define the carrier signal as a cosine wave of higher frequency.

5.Plot the Signals:
Use Matplotlib to plot the message signal, carrier signal, and amplitude-modulated signal.

# PROGRAM:
```
import numpy as np
import matplotlib.pyplot as plt
Am=2.3
Ac=4.6
fm=208
fc=2080
fs=20800
t=np.arange(0,2/fm,1/fs)
m=Am*np.cos(2*np.pi*fm*t)
c=Ac*np.cos(2*np.pi*fc*t)
s = (Ac + m) * np.cos(2 * np.pi * fc * t)
plt.subplot(3,1,1)
plt.plot(t,m)
plt.subplot(3,1,2)
plt.plot(t,c)
plt.subplot(3,1,3)
plt.plot(t,s)
```
# OUTPUT WAVEFORM:

<img width="784" height="544" alt="image" src="https://github.com/user-attachments/assets/615f518f-6934-40ec-b9e0-e96bdd21061d" />

# TABULAR COLUMN:

![WhatsApp Image 2025-11-06 at 10 42 14_ee5ae6bd](https://github.com/user-attachments/assets/0b3c917e-4dc8-4792-b9a3-91c840a0972f)

# Calculation
![WhatsApp Image 2025-11-06 at 18 09 23_9fa5949b](https://github.com/user-attachments/assets/a3b89804-b3ef-4756-b516-a74efa252813)


# RESULT:

The message signal, carrier signal, and amplitude modulated (AM) signal are plotted successfully.The AM waveform clearly shows the variation of carrier amplitude according to the message signal amplitude.

