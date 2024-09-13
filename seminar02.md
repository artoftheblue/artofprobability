# Семинар 2

Если вероятностное событие $\Omega$ с вероятностными точками. События — это подмножества нашего множества всех событий. 

Нужно определить функцию $\mathbb{P}\mathcal{F}\colon \to[0,1]$. Ищем область определения.

$\mathcal{F}$ — $\sigma$-алгебра. Системы подмножеств множества $\Omega$. Это область определения из меры, которую мы определим позже.

```{prf:definition}
Пусть $\Omega\neq\varnothing$. Система подмножеств $\mathcal{A}$ в $\Omega$ называется **алгеброй**, если выполнены три аксиомы:

1. $\Omega \in \mathcal{A}$;
2. если $A\in\mathcal{A}$, то $A^c\in\mathcal{A}\ (A^c:=\Omega\setminus A)$;
3. если $A_1,A_2\in\mathcal{A}$, то $A_1\cup A_2\in\mathcal{A}$

$\Omega$ называется единицей алгебры $\mathcal{A}$.

$(\forall A\in\mathcal{A}, \underbrace{A\cap\Omega=A}_{A\subseteq\Omega})$

```

```{prf:example}
$\Omega=\{\heartsuit,\diamondsuit,\spadesuit,\clubsuit \}$
1. $\mathcal{K}_1=\{\varnothing,\Omega,\{\heartsuit,\diamondsuit\},\{\spadesuit,\clubsuit\}\}$ — алгебра
2. $\mathcal{K}_2=\{\varnothing,\Omega,\{\heartsuit,\diamondsuit\}\}$ — не алгебра, т. к. $\{\heartsuit,\diamondsuit\}\in\mathcal{K}$, но $\{\heartsuit,\diamondsuit\}^c=\{\spadesuit,\clubsuit\}\not\in\mathcal{K}$.

```

```{prf:definition}
Пусть $\Omega\neq\varnothing$. Система подмножеств $\mathcal{A}$ в $\Omega$ называется **$\sigma$-алгеброй**, если выполнены три аксиомы:

1. $\Omega \in \mathcal{F}$;
2. если $A\in\mathcal{F}$, то $A^c\in\mathcal{F}\ (A^c:=\Omega\setminus A)$;
3. если $A_1,\dots,A_n,\dots\in\mathcal{F}$, то $\bigcup^\infty_{n=1}A_n\in\mathcal{F}$.

$\Omega$ называется единицей $\sigma$-алгебры $\mathcal{F}$.

```

## Задание 1

$\mathcal{A}$ — алгебра. Докажите, что $\varnothing\in\mathcal{A}$.

---

$\Omega\in\mathcal{A},\varnothing=\Omega^c\in\mathcal{A}$

```{note}
Если $\mathcal{F}$ — $\sigma$-алгебра, то $\varnothing\in\mathcal{F}$.
```

## Задание 2

$\mathcal{A}$ — алгебра, $A_1,A_2\in\mathcal{A}$

### Подзадание A

$A_1\cap A_2\in\mathcal{A}$

$A_1\cap A_2=(\underset{\in A}{\boxed{A_1^c}}\cup \underset{\in A}{\boxed{A_2^c}})^c\in\mathcal{A}$

### Подзадание B

$$A_1\setminus A_2 \in \mathcal{A}$$

$$A_1\setminus A_2=\underbrace{A_1\cap \underbrace{A_2^c}_{\in A}}_{\in A}\in\mathcal{A}$$

## Задание 3

Докажите, что всякая $\sigma$-алгебра является алгеброй

---

$\mathcal{F}$ — $\sigma$-алгебра $\implies$ все три аксиомы выполнены
$(a_1)=(\sigma_1), (a_2)=(\sigma_2)$ выполнены

Проверим, что для $\mathcal{F}$ выполнена $(a_3)$.

Пусть $A_1, A_2\in\mathcal{F}$. Положим $A_n=\varnothing\in\mathcal{F}$ при $n\geq 3$. 

$$\bigcup^\infty_{n=1}A_n\in\mathcal{F}\overset{(a3)}{=}A_1\cap A_2$$

Из задач 2 и 3 следует, что если $\mathcal{F}$ — $\sigma$-алгебра и $A_1, A_2\in\mathcal{F}$, то 

$$A_1\cup A_2\in\mathcal{F},\ A_1\cap A_2\in\mathcal{F},\ A_1\setminus A_2\in\mathcal{F}$$

## Задача 4

Пусть $\mathcal{F}$ — $\sigma$-алгбера и $A_1,\dots, A_n,\dots\in\mathcal{F}$. Докажите, что $\bigcap^\infty_{n=1}A_n\in\mathcal{F}$.

$$\bigcap^\infty_{n=1}A_n=\left(\underbrace{\bigcup_{n=1}^\infty \underbrace{A_n^c}_{\in\mathcal{F} (\sigma 2)}}_{_{\in\mathcal{F} (\sigma 2)}}\right)^c$$

```{note}
Пусть $\mathcal{A}$ — алгебра. Тогда в общем случае из условия, что $A_1,\dots,A_n,\dots\in\mathcal{A}$ **не следует** ни одно из условий, что $\bigcap^\infty_{n=1}A_n\in\mathcal{A}$ и $\bigcup^\infty_{n=1}A_n\in\mathcal{A}$
```

## Задача 5

