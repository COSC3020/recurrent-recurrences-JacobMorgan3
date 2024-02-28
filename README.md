[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/8KYthzwp)
# Recurrent Recurrences

Give big $\Theta$ bounds for the following recurrence relations.

1.
$$ T(n) =
    \begin{cases}
        1 & n \leq 1\\
        T\left(\frac{n}{13}\right) + 5 & n > 1
    \end{cases}
$$

$T(n/13^i) + 5i$ <br/>
From $13^i = n$ we get $i = log_{13}(n)$ <br/>
Plugging i back in we get that $T(n) \in \Theta(log(n))$ <br/>

3.
$$ T(n) =
    \begin{cases}
        1 & n \leq 1\\
        13 T\left(\frac{n}{13}\right) + 5 & n > 1
    \end{cases}
$$

$13^i * T(n/13^i) + ($ $\sum_{j=0}^{i-1} 13^j)$ <br/>
From $13^i = n$ we get $i = log_{13}(n)$ <br/>
Plugging i back in we get that $T(n) \in \Theta(n))$ <br/>

4.
$$ T(n) =
    \begin{cases}
        1 & n \leq 1\\
        13 T\left(\frac{n}{13}\right) + 2n & n > 1
    \end{cases}
$$

$13^i * T(n/13^i) + (($ $\sum_{j=0}^{i-1} 13^j) * n)$ <br/>
From $13^i = n$ we get $i = log_{13}(n)$ <br/>
Plugging i back in we get that $T(n) \in \Theta(n + n))$ <br/>
