# EXPT 1b: Computation-of-DFT-using-FFT-ALGORITHM

## AIM
To perform and verify DFT using FFT-ALGORITHM by SCILAB.
## APPARATUS REQUIRED
PC installed with SCILAB
## PROGRAM 
### DFT FFT-ALGORITHM
~~~
clear;
clc;
close;
xn = [1 2 3 4];
n1 = 0:1:length(xn)-1;

subplot(2,2,1);
plot2d3(n1,xn);

xlabel('Time n');
ylabel('Amplitude');
title('Input Sequence');


Xk = fft(xn);
K1 = 0:1:length(Xk)-1;
magnitude = abs(Xk)

subplot(2,2,2);
plot2d3(K1, magnitude);

xlabel('frequency(Hz)');
ylabel('magnitude(gain)');
title('magnitude spectrum');

angle = atan(imag(Xk), real(Xk))

subplot(2,2,3);
plot2d3(K1, angle);

xlabel('frequency(Hz)');
ylabel('Phase');
title('Phase spectrum');

y = ifft(Xk);
n2 = 0:1:length(y)-1;

subplot(2,2,4);
plot2d3(n2, y);

xlabel('Time n');
ylabel('Amplitude');
title('Inverse FFT OF X(K)');
~~~
<br>
<br>
<br>
<br>
<br>

<br>
### CALCULATIONS:
<img width="900" height="1600" alt="image" src="https://github.com/user-attachments/assets/05df4783-52ae-4094-893c-320a1131f580" />
<img width="900" height="1600" alt="image" src="https://github.com/user-attachments/assets/0de7d14a-3df4-40ca-bdfd-be847a15220f" />
<img width="900" height="1600" alt="image" src="https://github.com/user-attachments/assets/f82aebcc-a55d-496a-b92b-4b1f483bec89" />
<img width="900" height="1600" alt="image" src="https://github.com/user-attachments/assets/fcdb7410-5b96-444c-a26b-1dfe0fb40f67" />

<br>
<br>
<br>
<br>
<br>
### SAMPLE OUTPUT:
<img width="1600" height="775" alt="image" src="https://github.com/user-attachments/assets/0e6687a2-2ff5-4270-a2ff-dc2d3aa609bf" />

<br>
<br>
<br>
<br>



## RESULT:
Thus,  DFT using FFT-ALGORITHM for two given sequences were performed and its result was verified.

