### Section 6.4:  
#### Q3
$$
\mathcal{L}\{y(t)\} = Y(s)
$$
$$
\mathcal{L}\left\{\frac{dy}{dt}\right\} = sY(s) - y(0)
$$
$$
\mathcal{L}\left\{\frac{d^2y}{dt^2}\right\} = s^2Y(s) - sy(0) - y'(0)
$$
$$
\mathcal{L}\{y'' + 4y\} = \mathcal{L}\{\sin t - u_{2\pi}(t) \sin(t - 2\pi)\}
$$
$$
[s^2Y(s) - sy(0) - y'(0)] + 4Y(s) = \frac{1}{s^2 + 1} - \frac{1}{s^2 + 1} e^{-2\pi s}
$$
$$
y(0) = 0, \, y'(0) = 0
$$
$$
[s^2Y(s) + 4Y(s)] = \frac{1}{s^2 + 1} - \frac{1}{s^2 + 1} e^{-2\pi s}
$$
$$
(s^2 + 4)Y(s) = \frac{1}{s^2 + 1} - \frac{1}{s^2 + 1} e^{-2\pi s}
$$
$$
Y(s) = \frac{1}{(s^2 + 1)(s^2 + 4)} - \frac{1}{(s^2 + 1)(s^2 + 4)} e^{-2\pi s}
$$
$$
\frac{1}{(s^2 + 1)(s^2 + 4)} = \frac{As + B}{s^2 + 1} + \frac{Cs + D}{s^2 + 4}
$$
$$
1 = (As + B)(s^2 + 4) + (Cs + D)(s^2 + 1)
$$
$$
s = 0: \, 1 = 4B + D
$$
$$
s = 1: \, 1 = 5A + 5B + 2C + 2D
$$
$$
s = 2: \, 1 = 16A + 8B + 10C + 5D
$$
$$
s = 3: \, 1 = 39A + 13B + 30C + 10D
$$
$$
A = 0, \, B = \frac{1}{3}, \, C = 0, \, D = -\frac{1}{3}
$$
$$
Y(s) = \frac{1}{3}\left(\frac{1}{s^2 + 1} - \frac{1}{s^2 + 4}\right) - \frac{1}{3}\left(\frac{1}{s^2 + 1} - \frac{1}{s^2 + 4}\right)e^{-2\pi s}
$$
$$
\mathcal{L}^{-1}\left\{Y(s)\right\} = y(t)
$$
$$
y(t) = \mathcal{L}^{-1}\left\{\frac{1}{3}\left(\frac{1}{s^2 + 1} - \frac{1}{s^2 + 4}\right)\right\} - \mathcal{L}^{-1}\left\{\frac{1}{3}\left(\frac{1}{s^2 + 1} - \frac{1}{s^2 + 4}\right)e^{-2\pi s}\right\}
$$
$$
= \frac{1}{3} \sin t - \frac{1}{6} \sin 2t - \left[\frac{1}{3} \sin(t - 2\pi) - \frac{1}{6} \sin 2(t - 2\pi)\right] H(t - 2\pi)
$$
$$
= \frac{1}{6}(2 \sin t - \sin 2t) - \frac{1}{6} \left[2 \sin(t - 2\pi) - \sin 2(t - 2\pi)\right] H(t - 2\pi)
$$
$$
= \frac{1}{6}(2 \sin t - \sin 2t) - \frac{1}{6}(2 \sin t - \sin 2t) u_{2\pi}(t)
$$
$$
= \frac{1}{6}(2 \sin t - 2 \sin t \cos t) - \frac{1}{6}(2 \sin t - 2 \sin t \cos t) u_{2\pi}(t)
$$
$$
= \frac{1}{3} \sin t (1 - \cos t) - \frac{1}{3} \sin t (1 - \cos t) u_{2\pi}(t)
$$
$$
= \frac{1}{3} \sin t (1 - \cos t) [1 - u_{2\pi}(t)]
$$
![[Pasted image 20240723114045.png]]




#### Q5

$$
\mathcal{L}\{y(t)\} = Y(s)
$$
$$
\mathcal{L}\left\{\frac{dy}{dt}\right\} = sY(s) - y(0)
$$
$$
\mathcal{L}\left\{\frac{d^2y}{dt^2}\right\} = s^2Y(s) - sy(0) - y'(0)
$$
$$
\mathcal{L}\{y'' + y' + \frac{5}{4}y\} = \mathcal{L}\{t - u_{\pi/2}(t)(t - \pi/2)\}
$$
$$
[s^2Y(s) - sy(0) - y'(0)] + sY(s) - y(0) + \frac{5}{4}Y(s) = \frac{1}{s^2} - \int_{\pi/2}^{\infty} e^{-st}(t - \pi/2)dt
$$
$$
y(0) = 0, \, y'(0) = 0
$$
$$
[s^2 + s + \frac{5}{4}]Y(s) = \frac{1}{s^2} - \int_{\pi/2}^{\infty} e^{-st}(t - \pi/2)dt
$$
$$
\int_{\pi/2}^{\infty} e^{-st}(t - \pi/2)dt = \left[ \frac{e^{-st}(t - \pi/2)}{-s} \right]_{\pi/2}^{\infty} + \int_{\pi/2}^{\infty} \frac{e^{-st}}{s} dt = \frac{e^{-\pi s/2}}{s^2}
$$
$$
(s^2 + s + \frac{5}{4})Y(s) = \frac{1}{s^2} - \frac{e^{-\pi s/2}}{s^2}
$$
$$
Y(s) = \frac{1}{s^2(s^2 + s + \frac{5}{4})} - \frac{e^{-\pi s/2}}{s^2(s^2 + s + \frac{5}{4})}
$$
$$
\frac{1}{s^2(s^2 + s + \frac{5}{4})} = \frac{A}{s} + \frac{B}{s^2} + \frac{Cs + D}{s^2 + s + \frac{5}{4}}
$$
$$
1 = A s(s^2 + s + \frac{5}{4}) + B(s^2 + s + \frac{5}{4}) + (Cs + D)s^2
$$
$$
s = 0: \, 1 = \frac{5}{4}B
$$
$$
s = 1: \, 1 = \frac{13}{4}A + \frac{13}{4}B + C + D
$$
$$
s = 2: \, 1 = \frac{29}{2}A + \frac{29}{4}B + 8C + 4D
$$
$$
s = 3: \, 1 = \frac{159}{4}A + \frac{53}{4}B + 27C + 9D
$$
$$
A = \frac{16}{25}, \, B = \frac{4}{5}, \, C = \frac{16}{25}, \, D = -\frac{4}{25}
$$
$$
Y(s) = \left( -\frac{16}{25} \frac{1}{s} + \frac{4}{5} \frac{1}{s^2} + \frac{16}{25} \frac{s + \frac{1}{2}}{(s + \frac{1}{2})^2 + 1} - \frac{12}{25} \frac{1}{(s + \frac{1}{2})^2 + 1} \right) - \left( -\frac{16}{25} \frac{1}{s} + \frac{4}{5} \frac{1}{s^2} + \frac{16}{25} \frac{s + \frac{1}{2}}{(s + \frac{1}{2})^2 + 1} - \frac{12}{25} \frac{1}{(s + \frac{1}{2})^2 + 1} \right)e^{-\pi s/2}
$$
$$
y(t) = \mathcal{L}^{-1}\left\{Y(s)\right\}
$$
$$
y(t) = \mathcal{L}^{-1}\left\{ -\frac{16}{25} \frac{1}{s} + \frac{4}{5} \frac{1}{s^2} + \frac{16}{25} \frac{s + \frac{1}{2}}{(s + \frac{1}{2})^2 + 1} - \frac{12}{25} \frac{1}{(s + \frac{1}{2})^2 + 1} \right\} - \mathcal{L}^{-1}\left\{ \left( -\frac{16}{25} \frac{1}{s} + \frac{4}{5} \frac{1}{s^2} + \frac{16}{25} \frac{s + \frac{1}{2}}{(s + \frac{1}{2})^2 + 1} - \frac{12}{25} \frac{1}{(s + \frac{1}{2})^2 + 1} \right)e^{-\pi s/2} \right\}
$$
$$
= \frac{16}{25} - \frac{4}{5}t + \frac{16}{25}e^{-t/2}\cos t - \frac{12}{25}e^{-t/2}\sin t - \left[\frac{16}{25} - \frac{4}{5}(t - \frac{\pi}{2}) + \frac{16}{25}e^{-(t - \pi/2)/2}\cos(t - \pi/2) - \frac{12}{25}e^{-(t - \pi/2)/2}\sin(t - \pi/2)\right]H(t - \frac{\pi}{2})
$$
$$
= \frac{4}{25}[-4 + 5t + e^{-t/2}(4\cos t - 3\sin t)] + \frac{2}{25}[(5\pi + 8) - 10t - 2e^{-(t - \pi/2)/4}(4\sin t + 3\cos t)]H(t - \frac{\pi}{2})
$$
$$
= \frac{4}{25}[-4 + 5t + e^{-t/2}(4\cos t - 3\sin t)] + \frac{2}{25}[(5\pi + 8) - 10t - 2e^{-(t - \pi/2)/4}(4\sin t + 3\cos t)]u_{\pi/2}(t)
$$


![[Pasted image 20240723112220.png]]

#### Q9


$$
f(t) = \frac{h}{k}(t - t_0)H(t - t_0) - \frac{h}{k}(t - t_0 - k)H(t - t_0 - k) + hH(t - t_0 - k)
$$
$$
f(t) = \frac{h}{k}(t - t_0)[H(t - t_0) - H(t - t_0 - k)] + hH(t - t_0 - k)
$$
$$
= \frac{h}{k}(t - t_0)[u_{t_0}(t) - u_{t_0 + k}(t)] + hu_{t_0 + k}(t)
$$

![[Pasted image 20240723113250.png]]

Graph for $k = 1,h = 2,t_{0} = 3$
#### Q12  

##### Part a

![[Pasted image 20240723113815.png]]

$$
f(t) = \frac{1}{k}[u_5(t)(t - 5) - u_{5+k}(t)(t - 5 - k)]
$$

$$
\text{The value of } k \text{ determines the horizontal length of the ramp. } f(t) \text{ is identical to } g(t) \text{ if } k = 5.
$$


##### Part b

$$
y'' + 4y = f(t), \quad y(0) = 0, \quad y'(0) = 0
$$

$$
\mathcal{L}\{y(t)\} = Y(s)
$$

$$
\mathcal{L}\left\{\frac{dy}{dt}\right\} = sY(s) - y(0)
$$

$$
\mathcal{L}\left\{\frac{d^2y}{dt^2}\right\} = s^2Y(s) - sy(0) - y'(0)
$$

$$
\mathcal{L}\{y'' + 4y\} = \mathcal{L}\{f(t)\}
$$

$$
[s^2Y(s) - sy(0) - y'(0)] + 4Y(s) = \frac{1}{k}\left[\int_5^\infty (t-5)e^{-st}dt - \int_{5+k}^\infty (t-5-k)e^{-st}dt\right]
$$

$$
y(0) = 0, \quad y'(0) = 0
$$

$$
[s^2 + 4]Y(s) = \frac{1}{k}\left[\int_5^\infty (t-5)e^{-st}dt - \int_{5+k}^\infty (t-5-k)e^{-st}dt\right]
$$

$$
(s^2 + 4)Y(s) = \frac{1}{k}\left(\frac{e^{-5s}}{s^2} - \frac{e^{-(5+k)s}}{s^2}\right)
$$

$$
Y(s) = \frac{1}{k}\left(\frac{1}{s^2(s^2 + 4)} e^{-5s} - \frac{1}{s^2(s^2 + 4)} e^{-(5+k)s}\right)
$$

$$
Y(s) = \frac{1}{k}\left[\left(\frac{1}{4}\frac{1}{s^2} - \frac{1}{8}\frac{1}{s^2 + 4}\right)e^{-5s} - \left(\frac{1}{4}\frac{1}{s^2} - \frac{1}{8}\frac{1}{s^2 + 4}\right)e^{-(5+k)s}\right]
$$

$$
y(t) = \mathcal{L}^{-1}\{Y(s)\}
$$

$$
y(t) = \frac{1}{k}\left[\frac{1}{4}(t - 5) - \frac{1}{8}\sin[2(t - 5)]\right]u_5(t) - \frac{1}{k}\left[\frac{1}{4}(t - 5 - k) - \frac{1}{8}\sin[2(t - 5 - k)]\right]u_{5+k}(t)
$$

$$
y(t) = \frac{1}{k}\left[\frac{1}{4}(t - 5) - \frac{1}{8}\sin[2(t - 5)]\right]u_5(t) - \frac{1}{k}\left[\frac{1}{4}(t - 5 - k) - \frac{1}{8}\sin[2(t - 5 - k)]\right]u_{5+k}(t)
$$

##### Part c

$$
\text{Below are several plots of } y(t) \text{ versus } t \text{ for several values of } k.
$$
![[Pasted image 20240723114154.png]]

![[Pasted image 20240723114214.png]]


![[Pasted image 20240723114232.png]]
$$
\text{For sufficiently large } t, \text{ the solution is always a simple harmonic oscillation about } y = 1/4.
$$

$$
\text{The amplitude of the eventual oscillation depends on } k.
$$


### Section 6.5:  
#### Q1
$$
\mathcal{L}\{y(t)\} = Y(s)
$$
$$
\mathcal{L}\left\{\frac{dy}{dt}\right\} = sY(s) - y(0)
$$
$$
\mathcal{L}\left\{\frac{d^2y}{dt^2}\right\} = s^2Y(s) - sy(0) - y'(0)
$$
$$
\mathcal{L}\{y'' + 2y' + 2y\} = \mathcal{L}\{\delta(t - \pi)\}
$$
$$
[s^2Y(s) - sy(0) - y'(0)] + 2[sY(s) - y(0)] + 2Y(s) = e^{-\pi s}
$$
$$
y(0) = 1, \quad y'(0) = 0
$$
$$
[s^2Y(s) - s - 0] + 2[sY(s) - 1] + 2Y(s) = e^{-\pi s}
$$
$$
(s^2 + 2s + 2)Y(s) - s - 2 = e^{-\pi s}
$$
$$
(s^2 + 2s + 2)Y(s) = s + 2 + e^{-\pi s}
$$
$$
Y(s) = \frac{s + 2}{s^2 + 2s + 2} + \frac{e^{-\pi s}}{s^2 + 2s + 2}
$$
$$
\frac{s + 2}{s^2 + 2s + 2} = \frac{2}{(s + 1)^2 + 1} + \frac{s + 1}{(s + 1)^2 + 1}
$$
$$
Y(s) = \frac{2}{(s + 1)^2 + 1} + \frac{s + 1}{(s + 1)^2 + 1} + \frac{e^{-\pi s}}{(s + 1)^2 + 1}
$$
$$
y(t) = \mathcal{L}^{-1}\{Y(s)\}
$$
$$
y(t) = \mathcal{L}^{-1}\left\{\frac{2}{(s + 1)^2 + 1}\right\} + \mathcal{L}^{-1}\left\{\frac{s + 1}{(s + 1)^2 + 1}\right\} + \mathcal{L}^{-1}\left\{\frac{e^{-\pi s}}{(s + 1)^2 + 1}\right\}
$$
$$
= e^{-t}\sin t + e^{-t}\cos t + e^{-\pi s}e^{-(t - \pi)}\sin(t - \pi)H(t - \pi)
$$
$$
= e^{-t}(\sin t + \cos t) - e^{-\pi}e^{-(t - \pi)}\sin(t - \pi)H(t - \pi)
$$
$$
= e^{-t}(\sin t + \cos t) - e^{-\pi}e^{-(t - \pi)}\sin(t - \pi)u_\pi(t)
$$
![[Pasted image 20240723114509.png]]


#### Q4


$$
\mathcal{L}\{y(t)\} = Y(s)
$$
$$
\mathcal{L}\left\{\frac{dy}{dt}\right\} = sY(s) - y(0)
$$
$$
\mathcal{L}\left\{\frac{d^2y}{dt^2}\right\} = s^2Y(s) - sy(0) - y'(0)
$$
$$
\mathcal{L}\{y'' + 2y' + 3y\} = \mathcal{L}\{\sin t + \delta(t - 3\pi)\}
$$
$$
[s^2Y(s) - sy(0) - y'(0)] + 2[sY(s) - y(0)] + 3Y(s) = \frac{1}{s^2 + 1} + e^{-3\pi s}
$$
$$
y(0) = 0, \quad y'(0) = 0
$$
$$
[s^2 + 2s + 3]Y(s) = \frac{1}{s^2 + 1} + e^{-3\pi s}
$$
$$
Y(s) = \frac{1}{(s^2 + 1)(s^2 + 2s + 3)} + \frac{e^{-3\pi s}}{s^2 + 2s + 3}
$$
$$
\frac{1}{(s^2 + 1)(s^2 + 2s + 3)} = \frac{As + B}{s^2 + 1} + \frac{Cs + D}{s^2 + 2s + 3}
$$
$$
1 = (As + B)(s^2 + 2s + 3) + (Cs + D)(s^2 + 1)
$$
$$
s = 0: \quad 1 = 3B + D
$$
$$
s = 1: \quad 1 = 6A + 6B + 2C + 2D
$$
$$
s = 2: \quad 1 = 22A + 11B + 10C + 5D
$$
$$
s = 3: \quad 1 = 54A + 18B + 30C + 10D
$$
$$
A = -\frac{1}{4}, \quad B = \frac{1}{4}, \quad C = \frac{1}{4}, \quad D = \frac{1}{4}
$$
$$
Y(s) = -\frac{1}{4}\frac{s}{s^2 + 1} + \frac{1}{4}\frac{1}{s^2 + 1} + \frac{1}{4}\frac{s + 1}{(s + 1)^2 + 2} + \frac{1}{\sqrt{2}}\frac{e^{-3\pi s}}{(s + 1)^2 + 2}
$$
$$
y(t) = \mathcal{L}^{-1}\{Y(s)\}
$$
$$
y(t) = \frac{1}{4}\mathcal{L}^{-1}\left\{-\frac{s}{s^2 + 1} + \frac{1}{s^2 + 1} + \frac{s + 1}{(s + 1)^2 + 2}\right\} + \frac{1}{\sqrt{2}}\mathcal{L}^{-1}\left\{\frac{e^{-3\pi s}}{(s + 1)^2 + 2}\right\}
$$
$$
= \frac{1}{4}\left(-\cos t + \sin t + e^{-t}\cos \sqrt{2}t\right) + \frac{1}{\sqrt{2}}e^{-t} \sin \left[\sqrt{2}(t - 3\pi)\right]u_{3\pi}(t)
$$
$$
= \frac{1}{4}(\sin t - \cos t + e^{-t}\cos \sqrt{2}t) + \frac{1}{\sqrt{2}}e^{-t}\sin \left[\sqrt{2}(t - 3\pi)\right]u_{3\pi}(t)
$$
#### Q9

$$
2y'' + y' + 2y = \delta(t - 5), \quad y(0) = 0, \quad y'(0) = 0
$$

$$
\mathcal{L}\{y(t)\} = Y(s)
$$

$$
\mathcal{L}\left\{\frac{dy}{dt}\right\} = sY(s) - y(0)
$$

$$
\mathcal{L}\left\{\frac{d^2y}{dt^2}\right\} = s^2Y(s) - sy(0) - y'(0)
$$

$$
2[s^2Y(s) - sy(0) - y'(0)] + [sY(s) - y(0)] + 2Y(s) = e^{-5s}
$$

$$
y(0) = 0, \quad y'(0) = 0
$$

$$
2s^2Y(s) + sY(s) + 2Y(s) = e^{-5s}
$$

$$
(2s^2 + s + 2)Y(s) = e^{-5s}
$$

$$
Y(s) = \frac{e^{-5s}}{2s^2 + s + 2}
$$

$$
= \frac{1}{2}\frac{e^{-5s}}{\left(s + \frac{1}{4}\right)^2 + \frac{15}{16}}
$$

$$
y(t) = \mathcal{L}^{-1}\left\{\frac{1}{2}\frac{e^{-5s}}{\left(s + \frac{1}{4}\right)^2 + \frac{15}{16}}\right\}
$$

$$
= \frac{2}{\sqrt{15}}e^{-(t - 5)/4}\sin\left(\frac{\sqrt{15}}{4}(t - 5)\right)H(t - 5)
$$

$$
t_0 = 5 + \frac{8\pi}{\sqrt{15}}
$$

$$
2y'' + y' + 2y = \delta(t - 5) + k\delta(t - t_0), \quad y(0) = 0, \quad y'(0) = 0
$$

$$
2[s^2Y(s) - sy(0) - y'(0)] + [sY(s) - y(0)] + 2Y(s) = e^{-5s} + ke^{-st_0}
$$

$$
2s^2Y(s) + sY(s) + 2Y(s) = e^{-5s} + ke^{-st_0}
$$

$$
(2s^2 + s + 2)Y(s) = e^{-5s} + ke^{-st_0}
$$

$$
Y(s) = \frac{e^{-5s}}{2s^2 + s + 2} + k\frac{e^{-st_0}}{2s^2 + s + 2}
$$

$$
= \frac{1}{2}\left[\frac{e^{-5s}}{\left(s + \frac{1}{4}\right)^2 + \frac{15}{16}} + k\frac{e^{-st_0}}{\left(s + \frac{1}{4}\right)^2 + \frac{15}{16}}\right]
$$

$$
y(t) = \mathcal{L}^{-1}\left\{\frac{2}{\sqrt{15}}e^{-(t - 5)/4}\sin\left(\frac{\sqrt{15}}{4}(t - 5)\right)H(t - 5)\right\} + k\mathcal{L}^{-1}\left\{\frac{2}{\sqrt{15}}e^{-(t - t_0)/4}\sin\left(\frac{\sqrt{15}}{4}(t - t_0)\right)H(t - t_0)\right\}
$$

$$
y(t) = \frac{2}{\sqrt{15}}e^{-(t - 5)/4}\sin\left(\frac{\sqrt{15}}{4}(t - 5)\right)H(t - 5) + \frac{2k}{\sqrt{15}}e^{-(t - t_0)/4}\sin\left(\frac{\sqrt{15}}{4}(t - t_0)\right)H(t - t_0)
$$

$$
\text{Once } t \text{ takes the value of } t_0, \text{ the amplitude of the first term is }
$$

$$
\frac{2}{\sqrt{15}}e^{-2\pi/\sqrt{15}}
$$

$$
\text{and the amplitude of the second term is }
$$

$$
\frac{2k}{\sqrt{15}}.
$$

$$
\text{For the second term to cancel the first one, we require that }
$$

$$
\frac{2k}{\sqrt{15}} = -\frac{2}{\sqrt{15}}e^{-2\pi/\sqrt{15}}
$$

$$
k = -e^{-2\pi/\sqrt{15}}.
$$

![[Pasted image 20240723115247.png]]


#### Q13

$$
\mathcal{L}\{y(t)\} = Y(s)
$$

$$
\mathcal{L}\left\{\frac{dy}{dt}\right\} = sY(s) - y(0)
$$

$$
\mathcal{L}\left\{\frac{d^2y}{dt^2}\right\} = s^2Y(s) - sy(0) - y'(0)
$$

$$
y'' + y = \sum_{k=1}^{20} \delta(t - k\pi), \quad y(0) = 0, \quad y'(0) = 0
$$

$$
[s^2Y(s) - sy(0) - y'(0)] + Y(s) = \sum_{k=1}^{20} e^{-k\pi s}
$$

$$
y(0) = 0, \quad y'(0) = 0
$$

$$
(s^2 + 1)Y(s) = \sum_{k=1}^{20} e^{-k\pi s}
$$

$$
Y(s) = \sum_{k=1}^{20} \frac{e^{-k\pi s}}{s^2 + 1}
$$

$$
y(t) = \mathcal{L}^{-1}\left\{\sum_{k=1}^{20} \frac{e^{-k\pi s}}{s^2 + 1}\right\}
$$

$$
= \sum_{k=1}^{20} \mathcal{L}^{-1}\left\{\frac{e^{-k\pi s}}{s^2 + 1}\right\}
$$

$$
= \sum_{k=1}^{20} \sin(t - k\pi)H(t - k\pi)
$$

$$
= \sum_{k=1}^{20} \sin(t - k\pi)u_{k\pi}(t)
$$

![[Pasted image 20240723115919.png]]

Graph for $t = 20$

The arrows indicate the time, magnitude, and direction that the delta functions strike.

![[Pasted image 20240723120012.png]]

Graph for $t= 80$
#### Q14


$$
y'' + y = \sum_{k=1}^{20} (-1)^{k+1}\delta(t - k\pi), \quad y(0) = 0, \quad y'(0) = 0
$$

$$
[s^2Y(s) - sy(0) - y'(0)] + Y(s) = \sum_{k=1}^{20} (-1)^{k+1}e^{-k\pi s}
$$

$$
y(0) = 0, \quad y'(0) = 0
$$

$$
(s^2 + 1)Y(s) = \sum_{k=1}^{20} (-1)^{k+1}e^{-k\pi s}
$$

$$
Y(s) = \sum_{k=1}^{20} (-1)^{k+1} \frac{e^{-k\pi s}}{s^2 + 1}
$$

$$
y(t) = \mathcal{L}^{-1}\left\{\sum_{k=1}^{20} (-1)^{k+1} \frac{e^{-k\pi s}}{s^2 + 1}\right\}
$$

$$
= \sum_{k=1}^{20} (-1)^{k+1} \mathcal{L}^{-1}\left\{\frac{e^{-k\pi s}}{s^2 + 1}\right\}
$$

$$
= \sum_{k=1}^{20} (-1)^{k+1} \sin(t - k\pi)H(t - k\pi)
$$

$$
= \sum_{k=1}^{20} (-1)^{k+1} \sin(t - k\pi)u_{k\pi}(t)
$$
![[Pasted image 20240723120131.png]]

Graph for $t = 20$

![[Pasted image 20240723120159.png]]

Graph for $t = 100$

#### Q17


$$
y'' + 0.1y' + y = \sum_{k=1}^{20} (-1)^{k+1}\delta(t - k\pi), \quad y(0) = 0, \quad y'(0) = 0
$$

$$
[s^2Y(s) - sy(0) - y'(0)] + 0.1[sY(s) - y(0)] + Y(s) = \sum_{k=1}^{20} (-1)^{k+1}e^{-k\pi s}
$$

$$
y(0) = 0, \quad y'(0) = 0
$$

$$
\left(s^2 + 0.1s + 1\right)Y(s) = \sum_{k=1}^{20} (-1)^{k+1}e^{-k\pi s}
$$

$$
Y(s) = \sum_{k=1}^{20} (-1)^{k+1} \frac{e^{-k\pi s}}{s^2 + 0.1s + 1}
$$

$$
= \sum_{k=1}^{20} (-1)^{k+1} \frac{e^{-k\pi s}}{\left(s + \frac{1}{20}\right)^2 + \frac{399}{400}}
$$

$$
y(t) = \mathcal{L}^{-1}\left\{\sum_{k=1}^{20} (-1)^{k+1} \frac{e^{-k\pi s}}{\left(s + \frac{1}{20}\right)^2 + \frac{399}{400}}\right\}
$$

$$
= \sum_{k=1}^{20} (-1)^{k+1} \mathcal{L}^{-1}\left\{\frac{e^{-k\pi s}}{\left(s + \frac{1}{20}\right)^2 + \frac{399}{400}}\right\}
$$

$$
= \sum_{k=1}^{20} (-1)^{k+1} \frac{\sqrt{399}}{20}e^{-(t - k\pi)/20}\sin\left(\frac{\sqrt{399}}{20}(t - k\pi)\right)H(t - k\pi)
$$

$$
= \sum_{k=1}^{20} (-1)^{k+1} \frac{\sqrt{399}}{20}e^{-(t - k\pi)/20}\sin\left(\frac{\sqrt{399}}{20}(t - k\pi)\right)u_{k\pi}(t)
$$

![[Pasted image 20240723120807.png]]

Graph for $t = 20$

![[Pasted image 20240723120826.png]]

Graph for $t = 200$



### Section 6.6:  
#### Q1

$$
f * g = \int_0^t f(t - \tau)g(\tau) \, d\tau 
$$

Substitute $\xi = t - \tau$, then $d\xi = -d\tau$.

##### Part a

$$
f * g = \int_t^0 f(\xi)g(t - \xi) (-d\xi) = \int_0^t f(\xi)g(t - \xi) \, d\xi = \int_0^t g(t - \xi)f(\xi) \, d\xi = g * f
$$


##### Part b
$$
f * (g_1 + g_2) = \int_0^t f(t - \tau)[g_1(\tau) + g_2(\tau)] \, d\tau = \int_0^t f(t - \tau)g_1(\tau) \, d\tau + \int_0^t f(t - \tau)g_2(\tau) \, d\tau = f * g_1 + f * g_2
$$

##### Part c
$$
f * (g * h) = \int_0^t f(t - \tau)(g * h)(\tau) \, d\tau = \int_0^t f(t - \tau) \left(\int_0^\tau g(\tau - \xi)h(\xi) \, d\xi\right) \, d\tau 
$$

Switch the order of integration by integrating over the domain shown in the figure:

![[Pasted image 20240723121559.png]]

$$
f * (g * h) = \int_0^t \int_0^{t-\xi} f(t - \tau)g(\tau - \xi) \, d\tau \, h(\xi) \, d\xi = \int_0^t f(t - \xi) \left(\int_0^{t-\xi} g(u) \, du \right) h(\xi) \, d\xi 
$$

Make the substitution $u = \tau - \xi$, then $du = d\tau$:

$$
f * (g * h) = \int_0^t f(t - \xi) \left(\int_0^{t-\xi} g(u) \, du \right) h(\xi) \, d\xi = \int_0^t \left(\int_0^t f(t - \xi) g(t - \xi - u) \, du \right) h(\xi) \, d\xi 
$$

$$
= \int_0^t (f * g)(t - \xi) h(\xi) \, d\xi = (f * g) * h
$$

#### Q6


$$
f(t) = \int_0^t \sin(t - \tau) \cos \tau \, d\tau
$$

Recognize that \( f(t) \) is a convolution integral of the two functions, \( \sin t \) and \( \cos t \). The Laplace transform of \( f(t) \) can be found using the convolution theorem:

$$
\mathcal{L} \left\{ \int_0^t g(t - \tau) h(\tau) \, d\tau \right\} = G(s) H(s)
$$

where \( G \) and \( H \) are the Laplace transforms of \( g \) and \( h \), respectively. Therefore,

$$
\mathcal{L}\{f(t)\} = \mathcal{L} \left\{ \int_0^t \sin(t - \tau) \cos \tau \, d\tau \right\} = \mathcal{L}\{\sin t\} \mathcal{L}\{\cos t\}
$$

$$
= \left( \frac{1}{s^2 + 1} \right) \left( \frac{s}{s^2 + 1} \right) = \frac{s}{(s^2 + 1)^2}
$$

#### Q9

$$
F(s) = \frac{1}{(s + 1)^2 (s^2 + 4)}
$$

Recognize that \( F(s) \) is a product of the two Laplace transforms,

$$
\frac{1}{(s + 1)^2} = \mathcal{L}\{t e^{-t}\} \quad \text{and} \quad \frac{1}{s^2 + 4} = \frac{1}{2} \frac{2}{s^2 + 4} = \mathcal{L} \left\{ \frac{1}{2} \sin 2t \right\}
$$

According to the convolution theorem, the inverse Laplace transform of a product is a convolution integral:

$$
\mathcal{L}^{-1} \{ G(s) H(s) \} = \int_0^t g(t - \tau) h(\tau) \, d\tau
$$

where \( g \) and \( h \) are the inverse Laplace transforms of \( G \) and \( H \), respectively. Therefore,

$$
f(t) = \mathcal{L}^{-1} \{ F(s) \} = \mathcal{L}^{-1} \left\{ \frac{1}{(s + 1)^2 (s^2 + 4)} \right\} = \int_0^t (t - \tau) e^{-(t - \tau)} \frac{1}{2} \sin 2\tau \, d\tau
$$




#### Q11



$$
y'' + \omega^2 y = g(t); \quad y(0) = 0, \quad y'(0) = 1
$$

Because this ODE is linear, the Laplace transform can be applied to solve it. The Laplace transform of a function \(y(t)\) is defined as

$$
Y(s) = \mathcal{L}\{y(t)\} = \int_0^\infty e^{-st} y(t) \, dt.
$$

Consequently, the first and second derivatives transform as follows.

$$
\mathcal{L} \left\{ \frac{dy}{dt} \right\} = sY(s) - y(0)
$$

$$
\mathcal{L} \left\{ \frac{d^2 y}{dt^2} \right\} = s^2 Y(s) - sy(0) - y'(0)
$$

Apply the Laplace transform to both sides of the ODE.

$$
\mathcal{L}\{y''\} + \omega^2 \mathcal{L}\{y\} = \mathcal{L}\{g(t)\}
$$

Use the fact that the transform is a linear operator.

$$
\mathcal{L}\{y''\} + \omega^2 \mathcal{L}\{y\} = \mathcal{L}\{g(t)\}
$$

$$
[s^2 Y(s) - sy(0) - y'(0)] + \omega^2 Y(s) = G(s)
$$

Plug in the initial conditions, \( y(0) = 0 \) and \( y'(0) = 1 \).

$$
[s^2 Y(s) - 1] + \omega^2 Y(s) = G(s)
$$

As a result of applying the Laplace transform, the ODE has reduced to an algebraic equation for \( Y \), the transformed solution.

$$
(s^2 + \omega^2) Y(s) - 1 = G(s)
$$

Solve for \(Y(s)\) and write it in terms of known transforms.

$$
Y(s) = \frac{1}{s^2 + \omega^2} + \frac{G(s)}{s^2 + \omega^2}
$$

$$
Y(s) = \frac{1}{\omega} \frac{\omega}{s^2 + \omega^2} + \frac{1}{\omega} \frac{\omega G(s)}{s^2 + \omega^2}
$$

Now take the inverse Laplace transform of \(Y(s)\) to get \(y(t)\).

$$
y(t) = \mathcal{L}^{-1} \{ Y(s) \}
$$

$$
y(t) = \mathcal{L}^{-1} \left\{ \frac{1}{\omega} \frac{\omega}{s^2 + \omega^2} + \frac{1}{\omega} \frac{\omega G(s)}{s^2 + \omega^2} \right\}
$$

$$
y(t) = \frac{1}{\omega} \mathcal{L}^{-1} \left\{ \frac{\omega}{s^2 + \omega^2} \right\} + \frac{1}{\omega} \mathcal{L}^{-1} \left\{ \frac{\omega G(s)}{s^2 + \omega^2} \right\}
$$

$$
y(t) = \frac{1}{\omega} \sin(\omega t) + \frac{1}{\omega} \mathcal{L}^{-1} \left\{ \frac{G(s)}{s^2 + \omega^2} \right\}
$$

Since we're taking the inverse Laplace transform of a product of two transforms, we can use the convolution theorem. It says that

$$
\mathcal{L}^{-1} \{ F(s) G(s) \} = \int_0^t f(t - \tau) g(\tau) \, d\tau.
$$

Therefore,

$$
y(t) = \frac{1}{\omega} \sin(\omega t) + \frac{1}{\omega} \int_0^t \sin[\omega (t - \tau)] g(\tau) \, d\tau.
$$


#### Q13


$$
\text{Because the ODE is linear, the Laplace transform can be applied to solve it. The Laplace transform of a function } y(t) \text{ is defined here as}
$$

$$
Y(s) = \mathcal{L}\{y(t)\} = \int_0^{\infty} e^{-st}y(t) \, dt.
$$

$$
\text{Consequently, the first and second derivatives transform as follows.}
$$

$$
\mathcal{L}\left\{\frac{dy}{dt}\right\} = sY(s) - y(0)
$$
$$
\mathcal{L}\left\{\frac{d^2 y}{dt^2}\right\} = s^2 Y(s) - sy(0) - y'(0)
$$

$$
\text{Apply the Laplace transform to both sides of the ODE.}
$$

$$
\mathcal{L} \left\{ y'' + y' + \frac{5}{4}y \right\} = \mathcal{L}\{1 - u_\pi(t)\}
$$

$$
\text{Use the fact that the transform is a linear operator.}
$$

$$
[s^2 Y(s) - sy(0) - y'(0)] + [sY(s) - y(0)] + \frac{5}{4} [Y(s)] = \mathcal{L}\{1 - u_\pi(t)\}
$$

$$
\text{Plug in the initial conditions, } y(0) = 1 \text{ and } y'(0) = -1.
$$

$$
[s^2 Y(s) - s - 1] + [sY(s) - 1] + \frac{5}{4} [Y(s)] = \mathcal{L}\{1 - u_\pi(t)\}
$$

$$
\text{As a result of applying the Laplace transform, the ODE has reduced to an algebraic equation for } Y, \text{ the transformed solution.}
$$

$$
\left( s^2 + s + \frac{5}{4} \right) Y(s) - s - 1 = \mathcal{L}\{1 - u_\pi(t)\}
$$

$$
\text{Solve for } Y(s) \text{ and write it in terms of known transforms.}
$$

$$
Y(s) = \frac{s}{(s + \frac{1}{2})^2 + 1} + \frac{1}{(s + \frac{1}{2})^2 + 1} \mathcal{L}\{1 - u_\pi(t)\}
$$

$$
\text{Make it so that } s + \frac{1}{2} \text{ appears in the numerator of the first term.}
$$

$$
Y(s) = \frac{s + \frac{1}{2} - \frac{1}{2}}{(s + \frac{1}{2})^2 + 1} + \frac{1}{(s + \frac{1}{2})^2 + 1} \mathcal{L}\{1 - u_\pi(t)\}
$$

$$
Y(s) = \frac{s + \frac{1}{2}}{(s + \frac{1}{2})^2 + 1} - \frac{\frac{1}{2}}{(s + \frac{1}{2})^2 + 1} + \frac{1}{(s + \frac{1}{2})^2 + 1} \mathcal{L}\{1 - u_\pi(t)\}
$$

$$
\text{Now take the inverse Laplace transform of } Y(s) \text{ to get } y(t).
$$

$$
y(t) = \mathcal{L}^{-1} \{Y(s)\}
$$

$$
= \mathcal{L}^{-1} \left\{ \frac{s + \frac{1}{2}}{(s + \frac{1}{2})^2 + 1} - \frac{\frac{1}{2}}{(s + \frac{1}{2})^2 + 1} + \frac{1}{(s + \frac{1}{2})^2 + 1} \mathcal{L}\{1 - u_\pi(t)\} \right\}
$$

$$
= \mathcal{L}^{-1} \left\{ \frac{s + \frac{1}{2}}{(s + \frac{1}{2})^2 + 1} \right\} - \frac{1}{2} \mathcal{L}^{-1} \left\{ \frac{1}{(s + \frac{1}{2})^2 + 1} \right\} + \mathcal{L}^{-1} \left\{ \frac{1}{(s + \frac{1}{2})^2 + 1} \mathcal{L}\{1 - u_\pi(t)\} \right\}
$$

$$
= e^{-t/2} \cos t - \frac{1}{2} e^{-t/2} \sin t + \mathcal{L}^{-1} \left\{ \frac{1}{(s + \frac{1}{2})^2 + 1} \mathcal{L}\{1 - u_\pi(t)\} \right\}
$$

$$
\text{Since we’re taking the inverse Laplace transform of a product of two transforms, we can use the convolution theorem. It says that}
$$

$$
\mathcal{L}^{-1} \{F(s)G(s)\} = \int_0^t f(t - \tau)g(\tau) \, d\tau.
$$

$$
\text{Therefore,}
$$

$$
y(t) = e^{-t/2} \cos t - \frac{1}{2} e^{-t/2} \sin t + \int_0^t e^{-(t-\tau)/2} \sin(t - \tau)[1 - u_\pi(\tau)] \, d\tau.
$$



#### Q14

Same steps as before:

$$
y'' + 3y' + 2y = \cos \alpha t; \quad y(0) = 1, \quad y'(0) = 0
$$

$$
Y(s) = \mathcal{L}\{y(t)\} = \int_{0}^{\infty} e^{-st}y(t) \, dt
$$

$$
\mathcal{L}\left\{ \frac{dy}{dt} \right\} = sY(s) - y(0)
$$

$$
\mathcal{L}\left\{ \frac{d^2y}{dt^2} \right\} = s^2Y(s) - sy(0) - y'(0)
$$

$$
\mathcal{L}\{y'' + 3y' + 2y\} = \mathcal{L}\{\cos \alpha t\}
$$

$$
[s^2Y(s) - sy(0) - y'(0)] + 3[sY(s) - y(0)] + 2Y(s) = \frac{s}{s^2 + \alpha^2}
$$

$$
[s^2Y(s) - s \cdot 1 - 0] + 3[sY(s) - 1] + 2Y(s) = \frac{s}{s^2 + \alpha^2}
$$

$$
(s^2 + 3s + 2)Y(s) - s - 3 = \frac{s}{s^2 + \alpha^2}
$$

$$
(s^2 + 3s + 2)Y(s) = s + 3 + \frac{s}{s^2 + \alpha^2}
$$

$$
Y(s) = \frac{s + 3}{(s + 1)(s + 2)} + \frac{1}{(s + 1)(s + 2)} \mathcal{L}\{\cos \alpha t\}
$$

$$
= \left( \frac{2}{s + 1} - \frac{1}{s + 2} \right) + \left( \frac{1}{s + 1} - \frac{1}{s + 2} \right) \mathcal{L}\{\cos \alpha t\}
$$

$$
= \mathcal{L}^{-1} \left\{ \frac{2}{s + 1} - \frac{1}{s + 2} \right\} + \mathcal{L}^{-1} \left\{ \frac{1}{s + 1} - \frac{1}{s + 2} \right\} \mathcal{L}\{\cos \alpha t\}
$$

$$
y(t) = 2e^{-t} - e^{-2t} + \mathcal{L}^{-1} \left\{ \left( \frac{1}{s + 1} - \frac{1}{s + 2} \right) \mathcal{L}\{\cos \alpha t\} \right\}
$$

$$
y(t) = 2e^{-t} - e^{-2t} + \int_{0}^{t} \left( e^{-(t - \tau)} - e^{-2(t - \tau)} \right) \cos \alpha \tau \, d\tau
$$
