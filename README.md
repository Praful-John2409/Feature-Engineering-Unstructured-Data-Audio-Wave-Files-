# Feature Engineering Unstructured Data: Audio Wave Files

This project explores feature engineering techniques for audio wave files using the `librosa` library. The objective is to derive various audio features such as spectrograms, mel-scaled spectrograms, chromagrams, beat tracking, constant-Q transform, and MFCCs (Mel-Frequency Cepstral Coefficients) from wave files. The wave files used in this analysis are from NASA, showcasing audio signals from space.

## Features Extracted

1. **Spectrogram**: Visual representation of the frequency spectrum of the audio signal as it varies with time.
2. **Mel-Scaled Spectrogram**: A spectrogram that scales the frequency axis according to the mel scale, better approximating human auditory perception.
3. **Chromagram**: Displays the energy content of each pitch class, highlighting harmonic structures.
4. **Constant-Q Transform (CQT)**: A time-frequency representation where the frequency bins are geometrically spaced, ideal for music analysis.
5. **Beat Tracking**: Estimates the tempo and locates beat events within the audio.
6. **MFCCs (Mel-Frequency Cepstral Coefficients)**: Encodes the short-term power spectrum of a sound, capturing key perceptual features.

## NASA Audio Files Used

- Kepler: Star KIC12268220C Light Curve Waves to Sound
- NASA - Kepler: Star KIC7671081B Light Curve Waves to Sound
- NASA - Whistler Waves
- Johns Hopkins APL - Parker Solar Probe - Whistler Mode Waves 2
- NASA - Audio from NASA’s Juno Mission: Europa Flyby

## Steps Performed

1. **Download Audio Files**: The required audio files were downloaded from [NASA Halloween Sounds](https://www.nasa.gov/vision/universe/features/halloween_sounds.html).
   
2. **Load Audio Files**: Each audio file is loaded using `librosa`, allowing for feature extraction.

3. **Display Spectrogram**: Computes the short-time Fourier transform (STFT) to visualize the spectrogram of the audio signal.

4. **Compute Mel-Scaled Spectrogram**: Uses `librosa.feature.melspectrogram` to compute a spectrogram on a mel scale, giving insight into perceptual audio frequencies.

5. **Display Chromagram**: Displays harmonic content by showing the intensity of each pitch class present in the audio.

6. **Perform Constant-Q Transform (CQT)**: Uses `librosa.cqt` to analyze the audio with a geometrically spaced frequency axis.

7. **Beat Tracking**: Estimates the beats per minute (BPM) and shows the timing of detected beats using `librosa.beat.beat_track`.

8. **Extract MFCCs**: Computes MFCCs using `librosa.feature.mfcc`, capturing the audio signal’s key perceptual features, essential for audio analysis tasks like speech recognition.

## Link to the Colab
[click here](https://colab.research.google.com/drive/1_9cJEhQyoTYdatl3dp2JSDgtitiCmF-g?usp=sharing)
