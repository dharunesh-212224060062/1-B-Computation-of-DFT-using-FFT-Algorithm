# EXPT 1b: Computation-of-DFT-using-FFT-ALGORITHM

## AIM
To perform and verify DFT using FFT-ALGORITHM by SCILAB.
## APPARATUS REQUIRED
PC installed with SCILAB
## PROGRAM 
### DFT FFT-ALGORITHM
```
clc;
clear;

xn = [2 2 1 1];
N = length(xn);

n1 = 0:N-1;

// FFT Calculation
Xk = fft(xn,-1);

disp('FFT of the given sequence =', Xk);

// Magnitude Spectrum
subplot(3,1,1);
plot2d3(n1,xn);
xlabel('Time n');
ylabel('Amplitude');
title('Input Sequence');

subplot(3,1,2);
plot2d3(0:N-1,abs(Xk));
xlabel('Frequency k');
ylabel('Magnitude');
title('FFT Magnitude Spectrum');

// Phase Spectrum
subplot(3,1,3);
plot2d3(0:N-1,atan(imag(Xk),real(Xk)));
xlabel('Frequency k');
ylabel('Phase (rad)');
title('FFT Phase Spectrum');
```
### CALCULATIONS:

<img width="728" height="1280" alt="WhatsApp Image 2026-06-10 at 6 43 07 PM" src="https://github.com/user-attachments/assets/65992b6a-315d-49f1-be7c-8acc5dac8ab2" />

### SAMPLE OUTPUT:

<img width="1011" height="267" alt="WhatsApp Image 2026-06-10 at 6 40 42 PM" src="https://github.com/user-attachments/assets/0d5d090d-1778-42b2-8b9c-c6a387cca619" />
<img width="1600" height="877" alt="WhatsApp Image 2026-06-10 at 6 40 43 PM" src="https://github.com/user-attachments/assets/bf3c814c-5fd3-47a8-8e20-a6b5d94a4537" />


## RESULT:
Thus,  DFT using FFT-ALGORITHM for two given sequences were performed and its result was verified.

