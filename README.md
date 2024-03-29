[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/wM4-KOzy)
# Little-o

In addition to the big-O, big-$\Omega$, and big-$\Theta$ notation that
we covered at the beginning of this class, a few other notations are sometimes
used in asymptotic analysis.  For example, "little-$o$" notation.

Prove (i.e.\ give a formal mathematical proof) that $f(n)\in o(g(n))$ implies
that $f(n)\in O(g(n))$.

Hint: The proof will be *very* short and *very* easy. You can start by
identifying the differences between the definitions of O and o.

I have started with the formal definition of $o$ below. Add your answer to this
markdown file. [This
page](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions)
might help with the notation for mathematical expressions.

$f(n)\in o(g(n)) \iff \forall c>0, \exists n_0, \forall n\ge n_0: f(n) < c g(n)$


$f(n)\in O(g(n)) \iff \exists c,n_0 >0, \forall n\ge n_0: f(n) \le c g(n)$

Hence, the differences between little o and big O are the $\le$ (less than or equal to sign) 
regarding the relationship between f(n) and cg(n), and that little o demands $\forall c>0$, 
where as big O mentions $\exists c>0$. Suppose the little o definition remains true, that is,
$\forall c>0, \exists n_0, \forall n\ge n_0: f(n) < c g(n)$, so f(n) is less than c times g(n), 
for any value of c. This means $f(n)\in o(g(n))$ because f(n) is less than any c times g(n). 
Therefore, $f(n)\in O(g(n))$ because the differences between little o and big O are the $\le$ 
and the requirement for c, so if $f(n) < cg(n)$ with any/all c values, then $f(n)\le cg(n)$ 
with a specific c value because f(n) is less than cg(n), with any c value, so it must be 
less than or equal to cg(n), with a specific c value, by our supposition.
