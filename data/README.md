# Data

This folder contains three files, each with 30 seconds of 
EEG data from a healthy subject during propofol‑induced unconsciousness:
-  `eeganes07laplac250_detrend_all_t180.mat` Awake, before propofol induction
-  `eeganes07laplac250_detrend_all_t3070.mat` Unconscious, at a low dose of propofol
-  `eeganes07laplac250_detrend_all_t4710.mat` Unconscious, at a high dose of propofol

Each file contains is 64 channels of EEG under propofol anesthesia (from the same subject during the same session). The data has been Laplacian referenced, filtered and downsampled to 250 Hz, and detrended.

You can load the files using:
```
import scipy

l = scipy.io.loadmat(<filepath>,squeeze_me=True)
y = l['y']
fs = l['Fs']
ta = l['ta']
egrid_1indexed = l['egrid_1indexed']
```

The contents of each file are:
- `y`: (7500,64) The EEG voltage signals (in uV)
- `Fs`: the sampling frequency in Hz (250)
- `ta`: (7500,) the time axis
- `egrid_0indexed`: A grid layout of the electrode indices for visualization

Propofol anesthesia is characterized by two rhythms꞉ a slow
wave (<1 Hz) and an alpha rhythm (~10 Hz). 

Indices of good example electrodes
- Frontal electrode with good propofol alpha: 41
- Occipital electrode with good awake alpha: 52

Here is some example code of how to use `egrid_0indexed`. Suppose that the vector `S` (64,) has the alpha power for all electrodes. Here is how you would plot an image with the alpha power as though looking down at the top of the head:
```
grid = S[egrid_0indexed.astype(int)]
grid[np.isnan(egrid_indexed)] = np.nan
plt.imshow(grid)
```

