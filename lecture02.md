# Лекция 2, 09.09.2024

$$P(A)=\sum_{w_i\in A}P(w_i)$$

```{note} Замечание
$$P(\overline A)=1-P(A), P(\Omega)=1, P(\varnothing)=0$$
```

```{prf:example} Задача об авариях
Известно, что 40% автомобильных аварий совершаются людьми в состоянии алкогольного опьянения.
$$P(\Pi|\Alpha)=0.4\implies P(T|\Alpha)=0.6$$

$$P(\Pi)=0.05$$

$$\frac{P(\Alpha|\Pi)}{P(\Alpha|\Tau)}=\frac{P(\Alpha\cap \Pi)/P(\Pi)}{P(\Alpha \cap \Tau)/P(\Tau)}=\frac{P(\Pi|\Alpha)\cancel{P(\Alpha)}}{P(\Tau|\Alpha)\cancel{P(\Alpha)}}\cdot\frac{P(\Tau)}{P(\Pi)}=\frac{0.4}{0.6}\frac{0.95}{0.05}=12.7$$
```

## Независимость событий

Для независимых событий:

$$P(A|B)=P(A)$$

```{prf:definition}
$A$ и $B$ называются **попарно независимыми**, если 

$$\frac{P(A\cap B)=P(A)P(B)}{P(A|B)\cancel{P(B)}=P(A)\cancel{P(B)}}$$
```

```{prf:definition}
$A_1,\dots, A_n$ **независимы в совокупности**, если 

$$\forall i_1<i_2<\dots<i_k,\forall k=1,\dots,n$$

$$P(A_{i1}\cap A_{i2}\cap\ldots\cap A_{ik})=P(A_{i1})\cdot P(A_{i2})\cdot\ldots\cdot P(A_{ik})$$
```