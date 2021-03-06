

> **引理9:**
> 设 $x$ 是大偶数, 则有:
> $$P_{x} (x , x^{\frac{1}{10}}) - \frac{1}{2} \sum_{x^\frac{1}{10} < r \leq x^{\frac{1}{3}}} P_{x} (x , p , x^{\frac {1} {10}}) \geq \frac {2.6408 x C_{x}} {(\log x)^{2}}$$
> 其中 $\displaystyle{C_{x} = \prod_{{p|x}\vee{p > 2}} \frac {p - 1} {p - 2} \prod_{p > 2} \left(1 - \frac {1} {(p - 1)^{2}}\right)}.$

\comment: $$\prod_{\begin{aligned} p &\mid x \\ p &> 2\end{aligned}}$$



取 $\displaystyle{r(p) = \frac {p} {p - 1} , K = x , Z = x^{\frac {1} {10}}}$, 我们有

$$\begin{aligned}
\Gamma_{x} (x^{\frac {1} {10}})
&=\frac {x} {\varphi (x)} \prod_{p\nmid x} \frac {1 - \frac {1} {p - 1}} {1 - \frac {1} {p}} \frac {e^{- r}} {\log x^{\frac {1} {10}}} \left\{1 + O\left(\frac {1} {\log x}\right) \right\}\\
&= \frac {x} {\varphi (x)}\prod_{{p|x}\vee{p > 2}}\frac {(p - 1)^{2}} {p (p - 2)}\prod_{p > 2} \left(1 - \frac {1} {(p - 1)^{2}}\right) \frac {e^{- r}} {\log x^{\frac {1} {10}}} \left\{1 + O \left(\frac {1}{\log x}\right) \right\}\\
&= \frac {20 e^{- \gamma} C_{x}} {\log x}\left\{1 + O \left(\frac {1}{\log x}\right) \right\}
\end{aligned}$$

其中 $\gamma$ 是 Euler 常数. 

又当 $0\le u\leq2$ 时, 令 $F(u)=\dfrac{2e^r}{u},f(u)=0$, 而当 $u\geq2$ 时, 令 $(uF(u))'=f(u-1),(uf(u))'=F(u-1)$.

当 $2\le u\leq 3$ 时, 有:

$$uF(u)=2F(2),F(u)=\frac{2e^r}{u}$$

又当 $2\leq u\leq 4$ 时, 则有

$$u f (u) = \int_{2}^{u} F (t - 1) d t = 2 e^{r} \log (u - 1) , \quad f (u) = \frac {2 e^{r} \log (u - 1)} {u}$$

当 $3\leq u\leq 4$ 时, 我们有:

$$u F (u) = 2 e^r + \int_{3}^{u} f (t - 1) d t = 2 e^r \left(1 + \int_{2}^{u - 1} \frac {\log (t - 1)} {t} d t\right)$$

又有:

$$5 f (5) = 2 e^r \log 3 + \int_{4}^{5} F (u - 1) d u = 2 e^r \left(\log 4 + \int_{3}^{4} \frac {d u} {u} \int_{2}^{n - 1} \frac {\log (t - 1)} {t} d t\right)$$

取 $\xi^{2} = x^{\frac {1} {2} - \epsilon} , q = 1 ,  z = x^{\frac {1}{10}}$, 则由上式可知, 当 $x$ 很大时, 有: 

$$\begin{aligned}
P_{x} (x , x^{\frac {1} {10}}) 
&\geq \frac {2 (1 - \sqrt {e}) e^{- r} x C_{x} f (5)} {(\log x) (\log x^{\frac {1} {10}})} \\
&\geq \left\{\frac {8 (1 - \sqrt {e}) x C_{x}} {(\log x)^{2}} \right\}\cdot \left\{\log 4 + \int_{3}^{4} \frac {d u} {u} \int_{2}^{n - 1} \frac {\log (t - 1)} {t} \mathrm{d} t \right\}
\end{aligned}$$

再取 $\xi^{2} = \dfrac{x^{\frac {1} {2} - \epsilon}}{p} , q = p ,  z = x^{\frac {1}{10}}$, 我们有

$$\begin{aligned}
\sum_{x^\frac{1}{10} < r \leq x^{\frac{1}{3}}} P_{x} (x , p , x^{\frac {1} {10}})
&\leq\left\{\frac {20 (1 + \sqrt {e}) e^{- r} x C_{r}} {(\log x)^{2}} \right\}
\left\{\sum_{x^\frac{1}{10} < r \leq x^{\frac{1}{5}}}\left(\frac {2 c^{r}} {p}\right)\cdot \left(1 + \int_{2}^{4 - \frac {100 \log p} {\log x}} \frac {\log (t - 1)} {t} \mathrm{d}t\right)\left(\frac {\log x^{\frac {1} {10}}} {\log \frac {x^{\frac {1} {2}}} {p}}\right)+\sum_{x^\frac{1}{5} < r \leq x^{\frac{1}{3}}}\frac {2 e^{r} \log x^{\frac {1} {10}}} {p \log \frac {x^{\frac {1} {2}}} {p}}\right\}\\
&\leq\left\{\frac {(4 + 5 \sqrt {e}) x C_{x}} {\log x} \right\}
\left\{\int_{x^\frac{1}{10}}^{x^\frac{1}{5}}\frac {\mathrm{d} S} {S (\log S) (\log \frac {x^{\frac {1} {2}}} {S})}\int_{2}^{4 - \frac {10 \log s} {\log x}} \frac {\log (t - 1)} {t} \mathrm{d} t+ \int_{x^{\frac {1} {2}}}^{x^{\frac {1} {3}}} \cdot \frac {d S} {S (\log S) (\log \frac {x^{\frac {1} {2}}} {S})}\right\}\\
&=\left\{\frac {(4 + 5 \sqrt {e}) x C_{x}} {\log x} \right\}
\left\{\int_{\frac {1} {10}}^{\frac {1} {5}} \frac {d \alpha} {u (\frac {1} {2} - \alpha)} \int_{2}^{t - 10 a} \frac {\log (t - 1)} {t} \mathrm{d} t+\int_{\frac {1} {10}}^{\frac {2} {3}} \frac {d \alpha} {\alpha (\frac {1} {2} - \alpha)}\right\}\\
&=\left\{\frac {(8 + 10 \sqrt {e}) x C_{x}} {\log x} \right\}
\left\{\log 8 + \int_{\frac {1} {10}}^{\frac {1} {5}} \frac {d \alpha} {2 \pi (\frac {1} {2} - \alpha)} \int_{2}^{4 - 10 a} \frac {\log (t - 1)} {t} d t \right\}
\end{aligned}$$

显见, 当 $1\leq x \leq 2$时, 有 $\log x \leq \dfrac {x - 1} {2} + \dfrac {x - 1} {1 + x}$, 故有:

$$\begin{aligned}
&\int_{3}^{4} \frac {d u} {u} \int_{2}^{u - 1} \frac {\log (t - 1)} {t} d t - \frac {1} {4} \int_{\frac {1} {10}}^{\frac {1} {3}} \frac {d \alpha} {\alpha (\frac {1} {2} - \alpha)} \int_{2}^{4 - 1) a} \frac {\log (t - 1)} {t} d t\\
=& \int_{3}^{4} \left(\frac {1} {u} - \frac {2.5} {u (5 - u)}\right) d u \int_{2}^{u - 1} \frac {\log (t - 1)} {t} d t \\
\geq& \int_{3}^{4} \frac {2.5 - u} {u (5 - u)} \mathrm{d}t \int_{2}^{u - 1} (\frac {t - 2} {2} + \frac {t - 2} {t}) \frac {d t} {t} \\
=& \int_{3}^{4} \left\{\frac {2.5 - u} {2 u (5 - u)} \right\} (u - 3 + \frac {4} {u - 1} - 2) d u\\
=& \int_{3}^{4} \left(\frac {1} {2} - \frac {2.25} {u} - \frac {1} {4 (5 - u)} + \frac {0.75} {u - 1}\right) d u \\
=& \frac {1} {2} - 2.25 \log \frac {4} {3} - \frac {\log 2} {4}+ 0.75 \log \frac {3} {2} \\
=& \frac {1} {2} + 0.75 \log \frac {9} {8} - 1.5 \log \frac {4} {3} - \frac {\log 2} {4}\\
\geq& 0.588335 - 0.6048075 \\
=& - 0.0164725
\end{aligned}$$

综上所述:
$$\begin{aligned}
&P_{x} (x , x^{\frac {1} {10}}) - \frac {1} {2}\sum_{x^\frac{1}{10} < r \leq x^{\frac{1}{3}}} P_{x} (x , p , x^{\frac {1} {10}}) \\
\geq& \left(\frac {(8 - 50 \sqrt {e}) x C_{x}} {(\log x)^{2}}\right)\cdot (\log 4 - \frac {\log 8} {2} - 0.0164725) \\
\geq& \frac {(8 x C_{x}) (0.3301)} {(\log x)^{2}}
\end{aligned}$$

于是原命题得证

> **注:**
> 
> ```
> i1=Integrate[Log[t-1]/t,{t,2,4-10a},Assumptions->0.2>a>0.1]
> i2=Log[8]+NIntegrate[i1/(Pi-2Pi a),{a,1/10,1/5}]
> i3=i2(8+10Sqrt[E])
> ```
