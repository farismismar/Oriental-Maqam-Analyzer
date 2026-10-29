# Oriental Maqam Analyzer

This is a program I wrote in C that reads a wave file and finds the scale (Maqam) the file plays.  The algorithm uses pitch detection and a rule-based algorithm to detect the maqams, the jins a maqam is composed of, and the tonic.  It has been ported to Android for faster adoption.

## Usage
On an Android device, install the `.apk` file and follow the prompts.

## Support
If you like the work, consider leaving a donation on [PayPal](https://paypal.me/FarisMismar "PayPal") to keep the code maintenance effort going.

# Version History
| Version |  Date  | Changes |
| ------- |:---------------| :---------------|
| 1.0 | Sep 21, 2022 | Implementing FFT |
| 1.1 | Sep 21, 2022 | Uses FFT and pitch detection |
| 1.2 | Sep 21, 2022 | Playback of the input file |
| 1.3 | Sep 23, 2022 | Command line operation |
| 1.4 | Sep 25, 2022 | Autocorrelation for pitch detection |
| 1.41 | Sep 26, 2022 | Playback before analysis |
| 1.5 | Sep 28, 2022 | Bug fixes |
| 2.0 | Oct 2, 2022 | Introduction of maqam segments (jins) |
| 3.0 | Oct 9, 2022 | Detection of maqam and jins segments.  Preparation for deep learning pitch detection |
| 3.1 | Oct 12, 2022 | Fixed sampling rate for playback.  Introduced cents as measure of detection error |
| 3.2 | Oct 15, 2022 | Minor bug fixes and introduction of a grand output dataframe with timestamp and jins or maqam |
| 4.0 | Oct 2, 2026 | Implementation of SALIENCE to allow for human pitch detection and hidden Markov models instead of histograms |
| 4.1 | Oct 5, 2026 | Detection of all maqams time stamped over the entire waveform |
| 4.2 | Oct 6, 2026 | Minor tweaks for the Egyptian Jiharkah and interface |
| 4.3 | Oct 7, 2026 | Summary table shows jins and relevant transition |
| 4.4 | Oct 8, 2026 | Improved detection of human notes |
| 4.5 | Oct 8, 2026 | Summary table shows the confidence score |
| 4.51 | Oct 8, 2026 | Minor tweaks for the note detection |
| 4.6 | Oct 9, 2026 | Minor bug fixes |
| 4.67 | Oct 9, 2026 | Detected jins bug fixes (beta production) |
| 4.671 | Oct 10, 2026 | Minor fixes for jins |
| 4.672 | Oct 11, 2026 | Minor fixes and tweaks |
| 4.674 | Oct 13, 2026 | Silence as a maqam, split a maqam over different tonic, and sole jins as a maqam |
| 4.675 | Oct 13, 2026 | De-noising gate implemented and minor fixes for Jiharkah |
| 4.676 | Oct 15, 2026 | Bug fixes |
| 4.678 | Oct 17, 2026 | New maqam Saba Zamzam and preventing any segment less than 3 seconds from getting a verdict |
| 4.681 | Oct 19, 2026 | Bug fixes and improvements |
| 4.682 | Oct 21, 2026 | Improved noise detection |
| 4.685 | Oct 25, 2026 | Better maqam discernment model parameters |
| 4.7 | Oct 27, 2026 | New maqams: Huzam, Hussaini, and Nawa Athar |
