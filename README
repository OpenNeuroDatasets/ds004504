This dataset contains the EEG resting state-closed eyes recordings from 88 subjects in total.

Participants: 36 of them were diagnosed with Alzheimer's disease (AD group), 23 were diagnosed with Frontotemporal Dementia (FTD group) and 29 were healthy subjects (CN group).
Cognitive and neuropsychological state was evaluated by the international Mini-Mental State Examination (MMSE). MMSE score ranges from 0 to 30, with lower MMSE indicating more severe cognitive decline.
The duration of the disease was measured in months and the median value was 25 with IQR range (Q1-Q3) being 24 - 28.5 months.
Concerning the AD groups, no dementia-related comorbidities have been reported. The average MMSE for the AD group was 17.75 (sd=4.5), for the FTD group was 22.17 (sd=8.22) and for the CN group was 30.
The mean age of the AD group was 66.4 (sd=7.9), for the FTD group was 63.6 (sd=8.2), and for the CN group was 67.9 (sd=5.4).

Recordings: Recordings were aquired from the 2nd Department of Neurology of AHEPA General Hospital of Thessaloniki by an experienced team of neurologists. For recording, a Nihon Kohden EEG 2100 clinical device was used,
with 19 scalp electrodes (Fp1, Fp2, F7, F3, Fz, F4, F8, T3, C3, Cz, C4, T4, T5, P3, Pz, P4, T6, O1, and O2) according to the 10-20 international system and 2 reference electrodes (A1 and A2) placed on the mastoids for impendance check, according to the manual of the device. Each recording was performed according to the clinical protocol with participants being in a sitting position having their eyes closed.
Before the initialization of each recording, the skin impedance value was ensured to be below 5k?. The sampling rate was 500 Hz with 10uV/mm resolution.
The recording montages were anterior-posterior bipolar and referential montage using Cz as the common reference. The referential montage was included in this dataset.
The recordings were received under the range of the following parameters of the amplifier: Sensitivity: 10uV/mm, time constant: 0.3s, and high frequency filter at 70 Hz.
Each recording lasted approximately 13.5 minutes for AD group (min=5.1, max=21.3), 12 minutes for FTD group (min=7.9, max=16.9) and 13.8 for CN group (min=12.5, max=16.5).
In total, 485.5 minutes of AD, 276.5 minutes of FTD and 402 minutes of CN recordings were collected and are included in the dataset.

Preprocessing: The EEG recordings were exported in .eeg format and are transformed to BIDS accepted .set format for the inclusion in the dataset.
Automatic annotations of the Nihon Kohden EEG device marking artifacts (muscle activity, blinking, swallowing) have not been included for language compatibility purposes
(If this is an issue, please use the preprocessed dataset in Folder: derivatives).
The unprocessed EEG recordings are included in folders named: sub-0XX. Folders named sub-0XX in the subfolder derivatives contain the preprocessed and denoised EEG recordings.
The preprocessing pipeline of the EEG signals is as follows. First, a Butterworth band-pass filter 0.5-45 Hz was applied and the signals were re-referenced to A1-A2.
Then, the Artifact Subspace Reconstruction routine (ASR) which is an EEG artifact correction method included in the EEGLab Matlab software was applied to the signals,
removing bad data periods which exceeded the max acceptable 0.5 second window standard deviation of 17, which is considered a conservative window.
Next, the Independent Component Analysis (ICA) method (RunICA algorithm) was performed, transforming the 19 EEG signals to 19 ICA components.
ICA components that were classified as “eye artifacts” or “jaw artifacts” by the automatic classification routine “ICLabel” in the EEGLAB platform were automatically rejected.
It should be noted that, even though the recording was performed in a resting state, eyes-closed condition, eye artifacts of eye movement were still found at some EEG recordings.

A complete analysis of this dataset can be found in the published Data Descriptor paper "A Dataset of Scalp EEG Recordings of Alzheimer’s Disease, Frontotemporal Dementia and Healthy Subjects from Routine EEG", https://doi.org/10.3390/data8060095
