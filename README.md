# striking

## LATEST
"single bell templates" now has cells that take an initial template,
use it to extract most of the bell strikes, then overlay those bell
strikes to make another template, then repeat.
This seems to converge to excellent template derived from the recording
(but seeded with a single bell strike template).  The template discriminates
clearly between hand and back stroke - picking out one, but not the other.

A key element is looking at the sharpness of the peak produced by the
correlation of the template with the ringing.  I have been using a
measurement of the peak minus the average of the values at 4 samples on
either side of the peak.  A threshold of .02 seems to work quite well, but
this should probably be fit to the data, by detecting the threshold range
in which the peaks are appropriately spaced apart.

## NMF TODO
1. Approach to expressing signals as probabilities of bell strike times.
1. Algorithm to optimize number of noise channels in nmf.
1. Algorithm to identify which component corresponds to which bell.
1. Algorithm to identify how many bells are ringing.

## Spectrogram Matched Filter
The second exploration uses a spectrogram of an individual bell as
a matched filter to identify the strike times of that bell.  This
is explored in "single bell templates" and is currently very preliminary.

It looks likely that for best results, this would either require

a. individual recordings and consistent microphone placement and acoustics
b. a strategy for extracting the single bell spectrogram from the
recording.

