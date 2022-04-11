# Depression Detection In EEG
## About
CNN model classifying mild - moderate depression from EEG data using PyTorch. 

EEG data preprocessed with Python3 on jupyter notebook. EEG data for patients at rest (open eyes and closed eyes) was taken from J. Cavanagh's 2008 study published on the OpenNeuro database. All data was already semi-preprocessed by Cavanagh's team with a low-pass filter, epoched, and marked for events. Further preprocessing was needed to remove noise, deprecated channels, and visualize all events into topoplots for CNN preparation (raw .fif data files were missing, so vectorization was impossible).

## 1. Setting the EEG Cap
<img width="483" alt="Screen Shot 2022-04-08 at 3 39 34 PM" src="https://user-images.githubusercontent.com/71576247/162516984-01ee4463-9ca6-4234-8d2f-7d7df3e85741.png">
Using dataframe's XYZ values for each electrode, I created a map of the electrode cap and labelled it. This would set-up the heatmap to be overlaid on top of these electrodes. 

## 2. PSD Plot 
<img width="750" alt="Screen Shot 2022-04-08 at 3 39 42 PM" src="https://user-images.githubusercontent.com/71576247/162517008-47d4e9bc-e4ac-4eaa-b932-261992494d5f.png">


<img width="524" alt="Screen Shot 2022-04-08 at 3 39 48 PM" src="https://user-images.githubusercontent.com/71576247/162517014-26a1a41e-eec4-462b-bd64-939e1d708152.png">
<img width="572" alt="Screen Shot 2022-04-08 at 3 41 15 PM" src="https://user-images.githubusercontent.com/71576247/162517018-9f428cab-0fd9-459e-9ab5-69e408569c33.png">
<img width="345" alt="Screen Shot 2022-04-08 at 3 41 25 PM" src="https://user-images.githubusercontent.com/71576247/162517026-d1e238e4-7818-4186-81a4-432f77e2c41b.png">
