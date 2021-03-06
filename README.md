# Valve Amp emulation with MPEG 7 Audio Features
## Final Year project audio feature extraction for solid-state emulation of vacuum tube amplifiers

The goal of this project was to emulate the circuitry of a Vox AC15 Vacuum tube amplifier with analogue solid state Electronics. This is an old design from the early
1960s that is still in production to this day. Vacuum Tube Amps are coveted in the guitar community because of their characteristic tone. This tone is generated by
non-linear characteristics of triode and pentode vacuum tubes. An amplifier with similar topology was created and specifically biased to try and achieve as similar 
as possible non-linear distortion. 

To evaluate the design I used various MPEG 7 audio features that were found to be good descriptors for harmonic stringed instruments. This was done to evaluate 
the timbral quality of the sound being produced. The response of an instrument, as well as the amplifier, is so dynamic in the frequency domain over time that regular
function generator excitation and measurment would not provide enough meaningful information. Some of the MPEG-7 descriptors are common throughout audio analysis and
were taken from librosa. The Log-Attack time, Harmonic Spectral Variation, Harmonic Spectral Deviation and Odd to Even Harmonic Energy Ratio were calcualted from scratch
using Short Time Fourier Transform (STFT). The amplifiers frequency response was also measured using a sinusoidal chirp and the recorded data was filtered with
a Savitsky-Golay filter to give a smooth legible frequency response. 

*3D STFT of E Chord Through JFET emulation Amplifier:* 
![alt text](https://github.com/AidanJST/MPEG7-Guitar-Amp-Features/blob/main/img/Vox.png)

*JFET Circuit*
![alt text](https://github.com/AidanJST/MPEG7-Guitar-Amp-Features/blob/main/img/Amp.png)




