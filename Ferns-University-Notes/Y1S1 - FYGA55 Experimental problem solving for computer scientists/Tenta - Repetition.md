## Extra Exercises Mäta
### 1.

|                           |      |     |     |      |       |       |       |       |       |       |       |
| :-----------------------: | :--: | :-: | :-: | :--: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
|    ${}h(\pu{ km }){}$     |  0   |  1  |  2  |  3   |   4   |   5   |   6   |   7   |   8   |   9   |  10   |
| ${}T(\pu{ \degree C }){}$ | 15.0 | 8.5 | 2.0 | -4.5 | -11.0 | -17.5 | -24.0 | -30.5 | -37.0 | -43.5 | -50.0 |
#### A
Draw a diagram that shows the temperature T as a function of the height h
idk too lazy too, principle is simple
#### B
Decide the constants graphically
$$
\begin{align}
T=-6.5h+15
\end{align}
$$
#### C
if all variables are converted to SI base units, then the constants get different values, calculate these values and decide the SI base unit for the constant.

$$
\begin{align}
T=-0.0065h+288.15
\end{align}
$$
${}[T]=\pu{ K }{}$
${}[h]=\pu{ m }{}$
${}[a]=\pu{ K/m }{}$
${}[b]=K{}$
#### D
Write down the correlation
$$
\begin{align}
T=-6.5h+15, [h]=\pu{ km ,[T]=\pu{ \degree C }} \\
T=-0.0065h+288.15, [h]=\pu{ m },[T]=\pu{ K }
\end{align}
$$
### 2
#### A
The relationship seems nonlinear
${}\ln\left( \dfrac{t}{\pu{ min}} \right)=\ln k+a\ln \left( \dfrac{d}{\pu{ cm}} \right){}$
#### B
Linearisation!

| Thickness ${}\ln(\pu{ cm}){}$ | Boil time ${}\ln(\pu{ min}){}$ |
| :---------------------------: | :----------------------------: |
|         ${}1.0986{}$          |          ${}1.5041{}$          |
|         ${}1.5041{}$          |          ${}2.3026{}$          |
|         ${}1.7047{}$          |          ${}2.7081{}$          |
|         ${}1.9459{}$          |          ${}3.2189{}$          |
|         ${}2.1401{}$          |          ${}3.5553{}$          |
|         ${}2.3026{}$          |          ${}3.9120{}$          |
drawing a table gives ${}a=2{}$, ${}\ln k=-0.7\iff k=0.5{}$
${}t=0.5d^{2}{}$
${}[k]=\pu{ min/cm^{2} }{}$
### 3

#### A
$$
\begin{align}
\ln P=\ln \sigma+a\ln A+\beta \ln T \\
\ln P=\beta \ln T+k_{1} | k_{1}=\ln \sigma+\alpha \ln A \\
\ln P=\alpha\ln A+k_{2} | k_{2}=\ln \sigma+\beta \ln T
\end{align}
$$
#### B

| ${}\ln\left( \dfrac{T}{\pu{ K }} \right){}$ | ${}\ln\left( \dfrac{P}{\pu{ W }} \right){}$ |
| ------------------------------------------- | ------------------------------------------- |
| ${}6.1092{}$                                | ${}4.3174{}$                                |
| ${}6.2146{}$                                | ${}4.7185{}$                                |
| ${}6.3099{}$                                | ${}5.1120{}$                                |
| ${}6.3969{}$                                | ${}5.4596{}$                                |
| ${}6.4769{}$                                | ${}5.7807{}$                                |
| ${}6.5510{}$                                | ${}6.0776{}$                                |
Drawing a graph gives ${}\ln\left( \dfrac{P}{\pu{ W }} \right)=4\ln\left( \dfrac{T}{\pu{ K }} \right)-20.13{}$
${}\beta=4{}$
${}A=4\pi r^{2}=4\pi\left( \dfrac{d}{2} \right)^{2}=\dfrac{4\pi d^{2}}{2^{2}}=\pi d^{2}{}$

| ${}\dfrac{d}{\pu{ cm}}{}$ | ${}\dfrac{A}{\pu{ cm^{2}}}{}$ |
| ------------------------- | ----------------------------- |
| ${}5{}$                   | ${}78.540{}$                  |
| ${}10{}$                  | ${}314.16{}$                  |
| ${}15{}$                  | ${}706.86{}$                  |
| ${}20{}$                  | ${}1256.6{}$                  |
| ${}25{}$                  | ${}1963.5{}$                  |
| ${}31{}$                  | ${}3019.1{}$                  |
| ${}36{}$                  | ${}4071.5{}$                  |

| ${}\ln\left( \dfrac{A}{\pu{ cm^{2}}} \right){}$ | ${}\ln\left( \dfrac{P}{\pu{ W}} \right){}$ |
| ----------------------------------------------- | ------------------------------------------ |
| ${}4.3636{}$                                    | ${}4.4998{}$                               |
| ${}5.7499{}$                                    | ${}5.7683{}$                               |
| ${}6.5608{}$                                    | ${}6.6846{}$                               |
| ${}7.1362{}$                                    | ${}7.1701{}$                               |
| ${}7.5825{}$                                    | ${}7.6009{}$                               |
| ${}8.0127{}$                                    | ${}8.0064{}$                               |
| ${}8.3118{}$<br>                                | ${}8.3065{}$                               |
Drawing a graph gives us ${}\ln\left( \dfrac{A}{\pu{ cm^{2} }} \right)=1\ln\left( \dfrac{P}{\pu{ W }} \right)+0.267{}$
${}\alpha=1{}$
#### C

$$
\begin{align}
0.267=k_{2} \\
k_{2}=\ln \sigma+\beta \ln T \\
k_{2}=\ln \sigma T \\
0.267=\ln \sigma T \\
e^{0.267}=\sigma T \\
1.306=\sigma T \\
\dfrac{1.306}{T}=\sigma \\
\sigma=\dfrac{1.306}{650}=0.002009 \approx 0.002
\end{align}
$$
never mind fuck that

| ${}A{}$ | ${}P{}$ |
| ------- | ------- |
| 78.54   | 90      |
| 314.16  | 320     |
| 706.86  | 800     |
| 1256.6  | 1300    |
| 1963.5  | 2000    |
| 3019.1  | 3000    |
| 4071.5  | 4050    |
Throwing that into a graph gives
${}P=0.9854A+45.5{}$

$$
\begin{align}
0.9854=\sigma T^{4} \\
\dfrac{0.9854}{T^{4}}=\sigma \\
\dfrac{0.9854}{650^{4}}=\sigma \\
\sigma=5.5*10^{−12} \\
\sigma_{\text{SI}}= 5.5*10^{-8}
\end{align}
$$
#### D

$$
\begin{align}
P=\sigma AT^{4} \iff \sigma=\dfrac{P}{AT^{4}}\\
[\sigma]=\dfrac{W}{cm^{2}K^{4}} \\
[\sigma]_{\text{SI}}=\dfrac{W}{m^{2}K^{4}}
\end{align}
$$
#### E
${}P=\sigma AT^{4}{}$ where ${}\sigma=5.5*10^{-8}{}$
### 4
#### A
${}t=CR^{3/2}{}$
${}C=\dfrac{t}{R^{3/2}}{}$
${}[C]=\dfrac{T}{L^{3/2}}=TL^{-3/2}{}$
#### B
${}[C]=sm^{-3/2}{}$
### 5
#### A

$$
\begin{align}
I=\dfrac{P_{0}}{r^{2}}e^{ -ar } \\
a=\dfrac{8\pi^{2}f^{2}\eta}{3c^{3}\rho} \\
I=\dfrac{P_{0}}{r^{2}}e^{ -\left( \frac{8\pi^{2}f^{2}\eta}{3c^{3}\rho} \right)r } \\
\dfrac{Ir^{2}}{P_{0}}=e^{ -\left( \frac{8\pi^{2}f^{2}\eta}{3c^{3}\rho} \right)r } \\
\ln\left( \dfrac{Ir^{2}}{P_{0}} \right)=-\left( \dfrac{8\pi^{2}f^{2}\eta}{3c^{3}\rho} \right)r \\
-\dfrac{\ln\left( \dfrac{Ir^{2}}{P_{0}} \right)}{r}=\dfrac{8\pi^{2}f^{2}\eta}{3c^{3}\rho} \\
-\dfrac{3c^{3}\rho\ln\left( \dfrac{Ir^{2}}{P_{0}} \right)}{r}=8\pi^{2}f^{2}\eta \\
-\dfrac{3c^{3}\rho\ln\left( \dfrac{Ir^{2}}{P_{0}} \right)}{r8\pi^{2}f^{2}}=\eta \\
[P]=W=\dfrac{J}{s}=\dfrac{Nm}{s}=\dfrac{kg\dfrac{m}{s^{2}}m}{s}=\dfrac{kgm^{2}}{s^{3}} \\
[I]=\dfrac{W}{m^{2}}=\dfrac{kg}{s^{3}} \\
[\rho]=\dfrac{kg}{m^{3}} \\
[c]=\dfrac{m}{s} \\
[r]=s \\
[\eta]=\dfrac{\left( \dfrac{m}{s} \right)^{3}\dfrac{kg}{m^{3}}\ln\left( \dfrac{\dfrac{kg}{s^{3}}m^{2}}{\dfrac{kgm^{2}}{s^{3}}} \right)}{m \dfrac{1}{s^{2}}}=\dfrac{\dfrac{kg}{s^{3}}}{\dfrac{m}{s^{2}}}=\dfrac{kg}{ms}
\end{align}
$$
#### B

$$
[\eta]=\dfrac{M}{LT}
$$
### 6

$$
\begin{align}
pV=nRT \\
[p]=\dfrac{N}{m^{2}}=\dfrac{kg\dfrac{m}{s^{2}}}{m^{2}}=\dfrac{kg}{s^{2}m} \\
[V]=m^{3} \\
[n]=mol \\
[T]=K \\
R=\dfrac{pV}{nT} \\
[R]=\dfrac{\dfrac{kg}{s^{2}m}m^{3}}{mol K}=\dfrac{kgm^{2}}{Ks^{2}mol}
\end{align}
$$