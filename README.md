# Fourier Transforms in action

## In this notebook, we shall see the implementation of fft, ifft, fftshift in the torch.fft module

```torch.fft.fft``` computes the FFT of the input signal, ```torch.fft.ifft``` computes the IFFT, and ```torch.fft.fftshift``` shifts the zero-frequency component to the center of the spectrum. ( The zero-frequency component of the spectrum is the region of the real domain where the function remains constant. This is possible in the region where the function is not defined, thus assumed to be zero. And just before this undefined region starts, the function drops rapidly from define to not define (assumed as zero). Thus, ```fftshift``` seems to shift the peaks from the edges to the centre, and if we want to compute the fourier transform, we must not forget to apply ```fftshift```.)

The relevant signal transforms have been marked with '(RELEVANT)'.
