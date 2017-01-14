# striking

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

