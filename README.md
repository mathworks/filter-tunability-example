The three Simulink files used as an example in the "How to Use Tunable and Non-Tunable Filters in DSP System Toolbox" video.

Non-tunable filter blocks independently filter each channel of the input signal over time using the filter design specified by their block parameters. As they are non-tunable, their block parameters and filter response cannot be changed during runtime. On the other hand, tunable Simulink blocks can have their block parameters modified during a simulation, removing the need to update the model diagram between runs and speeding up testing.  

If you know beforehand that your filter’s response will be unchanging at runtime, the non-tunable filter design blocks can be used to design and implement FIR and IIR filters. In contrast, the Variable Bandwidth FIR and IIR filters, Discrete FIR filter, and Biquad filter blocks can be used to tune filter responses at runtime via filter parameters and coefficients. 

To open the non-tunable bandpass filter implementation, launch "Bandpass_IIR.slx".

To open the bandpass filter implemented with a Variable Bandwidth IIR block and tuned via block parameters, launch "VB_IIR.slx".

To open the bandpass filter implemented with a Biquad Filter block and tuned via filter coefficients, launch "Biquad_IIR.slx".

For each example, you can view the performance of the bandpass filter by comparing the signal to noise ratio (SNR) values for the original and filtered signals in the Spectrum Analzyer. The SNR values can be displayed in the Spectrum Analzyer by enabling "Distortion Measurements" under Tools>Measurements. For the example files, this display is enabled by default.


