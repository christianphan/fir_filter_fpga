# fir_filter_fpga
Making a simple FIR filter for audio and video processing on Zybo board

A FIR (finite impulse response) filter, meaning the filter's impulse response is of finite period and will settle to zer oin finite time. This can be created by applying a FFT to a signal that we want to filter out low.

"moving average"
"pole z = 0"
"filter response will decay to zero after some time"
"n = number of order"
"n + 1 = number of taps"
"n = number of delays"

Y[n] = Sum k=0 -> k=M  (b_k)*x[n-k]  
H[z] = Sum k=0 -> k=M  (b_k)*z^-k = bo *Multiplication k = 1 -> k=M (1 -c_k*(z^-1))

h[n] = bn, 0 <= n <= M
	 = 0 , otherwise



The other type of filter is IIR( infinite impulse response) filter which have feedback reponse so infinte number responses will out of the filter. It uses the concept of recursion

"poles at z = 0 and other locatoin"

y[n] = Sum k=0 -> k = M


