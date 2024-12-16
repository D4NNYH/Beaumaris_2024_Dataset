# Beaumaris_2024_Dataset
Dataset for "Towards the measurement of sea ice thickness using a time domain inductive measurement system"

Data is structured in folders per experiment.
.TRaNSMIT are raw hexadecimal files containing 16 bit integers corresponding to ADC values of the STM32H723VGT6 (in the ranges of 0 and +3.3v), this is post hardware gain and offsetting.

The .TRaNSMIT files in measurments are named corresponding to their time of measurement (1 file per second), these are the datasets used for published results.

The nulling_waveform file corresponds to the waveform output by the DAC for active Nulling.

These files are structured in multiples of 1024 integers, every 1024 integers corresponding to 1 waveform.
measurement_times.csv in each experiment folder states what time each measurement was taken and details on it.

Log files were used for debugging the microcontroller.
