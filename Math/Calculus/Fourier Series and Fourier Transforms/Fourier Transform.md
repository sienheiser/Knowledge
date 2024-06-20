Suppose function $f(x)$ has a [[Fourier Series|Fourier series]] given as

$$
f(x) = \sum_{n = -\infty}^{\infty} \frac{1}{T}\left(\int_{-T/2}^{T/2} f(t)\exp(-iw_nt)dt\right)\exp(iw_n x)
$$
where $w_n = \frac{2\pi n}{T}$ and we have plugged in the values of the Fourier coefficients. As $T$ becomes larger then $\Delta w = w_{n+1}-w_{n} = \frac{2\pi}{T}$ becomes smaller. If we substitute $\frac{1}{T} = \frac{\Delta w}{2\pi}$ Then we get
$$
f(x) = \frac{1}{\sqrt{2\pi}}\lim_{\Delta w \rightarrow 0}\sum_{n = -\infty}^{\infty} \frac{\Delta w}{\sqrt{2\pi}}\left(\int_{-T/2}^{T/2} f(t)\exp(-iw_nt)dt\right)\exp(iw_n x)
$$
which is just a Reimann sum giving us
$$
f(t) = \frac{1}{\sqrt{2\pi}}\int_{-\infty}^{\infty}\left(\frac{1}{2\pi}\int_{-\infty}^{\infty} f(t)\exp(-iwt)dt\right)\exp(iw t)dw = \frac{1}{\sqrt{2\pi}}\int_{-\infty}^{\infty}\tilde{f}(w)\exp(iw t)dw 
$$
where we define the Fourier transform to be 

$$
\tilde{f}(w) = \frac{1}{2\pi}\int_{-\infty}^{\infty} f(t)\exp(-iwt)dt
$$
and the inverse Frourier transform is 

$$
f(t) = \frac{1}{2\pi}\int_{-\infty}^{\infty} f(w)\exp(iwt)dw.
$$

The Fourier transform $\tilde{f}(w)$ can be interpreted as continuous Fourier coefficients. Then the integral 
$$
f(t)=\frac{1}{\sqrt{2\pi}}\int_{-\infty}^{\infty}\tilde{f}(w)\exp(iw t)dw 
$$
is viewed as summing over a continumm of plane waves.
