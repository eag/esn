# **esn**

### Purpose <br>

to predict epoched EEG data some "k" steps ahead
<br>
<br>


# **Quick Start**

### Input
- input should be stored as 64 bit floats in a binary file
- first value in the binary file stores the number of timepoints in the epoch
- second value stores the number of epochs in the file
- remaining values store the epoched data for a single channel or multiple channels
- values are generally normalized to lie between 0 and 1

### Output
- first value in the binary file stores the number of timepoints in the epoch
- second stores the number of epochs in the file
- third value stores the number of prediction steps
- remaining values store the prediction k steps ahead

### Execution
- see https://github.com/eag/esn/blob/main/bash/run_esn for an example

### Example output
- 20 step prediction (40 ms) of eeg activity in delta band (obtained using MATLAB's "wavedec" function): https://github.com/eag/esn/blob/main/demo/predict_k20.mp4
- 8 step prediction (16 ms) of broadband eeg activity (0.1 to 40 Hz): https://github.com/eag/esn/blob/main/demo/predict_k8.mp4
<br>
<br>

# **Dependencies**
- cxxopts (https://github.com/jarro2783/cxxopts)
- armadillo (https://github.com/EmanueleCannizzaro/armadillo)



