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

```{seealso} Замечание
Для $A_1,A_2,A_3$:
$$P(A_1\cap A_2)=P(A_2\cap A_3)=P(A_1\cap A_3)\\ P(A_1\cap A_2\cap A_3)=P(A_1)P(A_2)P(A_3)$$

Контрпример, где все попарные события независимы.

3 стороны тетраэдра покрашены в красный, жёлтый и зелёный. Четвёртая покрашена во все три цвета. 

* $A$ — есть красный
* $B$ — есть зелёный
* $C$ — есть жёлтый

$$\frac{1}{4}=P(A\cap B\cap C)$$

$$P(A)=P(B)=P(C)=\frac{1}{2}$$

$$\frac{1}{8}=P(A)P(B)P(C)\neq P(A\cap B\cap C)$$
```

```{seealso} Замечание
Если $A_1,\ldots,A_n$ независимы в совокупности, то над любым из событий можно поставить отрицание и система останется неизменной.
```

```{prf:example}
$A_1,A_2,A_3$ — независимы в совокупности, то $\overline A_1,A_2,A_3$ — независимы в совокупности.

$$P(\overline A_1\cap A_2)\overset{?}{=}P(\overline A_1)P(A_2)$$

$$P(\overline A_1\cap A_2)=P(A_2\setminus A_1)=P(A_2)$$
```