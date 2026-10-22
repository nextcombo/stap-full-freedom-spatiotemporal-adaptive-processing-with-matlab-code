# [STAP] Full-Freedom Spatiotemporal Adaptive Processing [with MATLAB Code]

1. Full-Dimension STAP
\tThe core of STAP processing is to estimate the clutter covariance matrix through multiple distance gate samples, thereby removing clutter signals in the target's distance gate based on the clutter covariance matrix and separating target signals from clutter signals.
\tConsidering uniform linear array for STAP processing. Matched filtering should be performed before STAP to concentrate the energy of the echo signal into a single distance gate. The multichannel three-dimensional radar echo data after matched filtering can be represented by Figure 3-12.
2. Reduced-Dimension STAP
\tAs analyzed in the previous section, in order to accurately estimate the clutter covariance matrix, it is necessary to extract a large number of time-space snapshots across multiple distance gates. For example, with 16 antenna elements and 32 pulses per CPI, at least 1024 distance rings are required to meet the requirements. At the same time, due to the high number of antenna elements and pulses per CPI, the dimension of the clutter covariance matrix calculated according to Equation (3-18) is large. The inverse of this large matrix has a significant computational cost in practical applications, thus requiring improvements to the full-dimensional STAP algorithm.
\tCommon methods of improvement mainly include dimensionality reduction and rank reduction. This article mainly introduces the reduced-dimensional STAP algorithm, which transforms the antenna-pulse domain to the angle-Doppler domain by using a reduced-dimensionality matrix, using the main channel and auxiliary channels to reduce the dimensionality of the clutter covariance matrix, thus avoiding the inverse of the large matrix.
\tCommon reduced-dimensional STAP algorithms include mDT, JDL, etc. Below are introductions to these algorithms.
\tThe flow of all reduced-dimensional algorithms is similar: through a linear transformation matrix T, the time-space snapshots are transformed from the antenna-pulse domain to the angle-Doppler domain, then select an auxiliary channel in the angle-Doppler domain and several auxiliary channels for subsequent reduced-dimensional STAP. The difference between 3DT and JDL algorithms lies only in the number of auxiliary channels selected.
MATLAB simulation results

## Images

![(STAP)Full-Freedom Spatiotemporal Adaptive Processing [with MATLAB Code]](01.jpg)
![(STAP)Full-Freedom Spatiotemporal Adaptive Processing [with MATLAB Code]](02.jpg)
![(STAP)Full-Freedom Spatiotemporal Adaptive Processing [with MATLAB Code]](03.jpg)
![(STAP)Full-Freedom Spatiotemporal Adaptive Processing [with MATLAB Code]](04.jpg)
![(STAP)Full-Freedom Spatiotemporal Adaptive Processing [with MATLAB Code]](05.jpg)
![(STAP)Full-Freedom Spatiotemporal Adaptive Processing [with MATLAB Code]](06.jpg)

<!-- PAYMENT_BLOCK -->

## Get this dataset

- Payment link (Stripe): [Buy now](https://buy.stripe.com/3cs8yP7sY87d0vu9AB)
- Payment QR code: ![Payment QR code](pay.png)

<!-- /PAYMENT_BLOCK -->
