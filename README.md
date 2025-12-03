# REM-phasic-tonic-analysis

**Implementation based on:**

Simor, P. et al. (2019). The paradox of rapid eye movement sleep in the light of oscillatory activity and cortical synchronization during phasic and tonic microstates.  
NeuroImage. [https://doi.org/10.1016/j.neuroimage.2019.116066](https://doi.org/10.1016/j.neuroimage.2019.116066)

**Data Source:**  
The data used in this project comes from the Sleep-EDF Expanded dataset (PhysioNet):  
[https://physionet.org/content/sleep-edfx/1.0.0/](https://physionet.org/content/sleep-edfx/1.0.0/)

**Method:**

Phasic and tonic REM were defined using short, non-overlapping 4-second windows inside REM sleep:

- **Phasic REM:** 4-second segments containing ≥ two consecutive eye movements in the horizontal EOG with amplitudes ≥ 100 µV.
- **Tonic REM:** 4-second segments within REM where all EOG deflections stayed ≤ 25 µV (no significant eye movements).

To avoid overlap or contamination between states, detected windows were separated by a minimum of 8 seconds.

**PSD of tonic and phasic REM sleep** was computed.
