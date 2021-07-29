+++
categories = ["math"]
draft = false
image = "img/blog/cube.jpg"
showonlyimage = false
date = "2020-2-25T19:50:47+05:30"
title = "Permutation Group"
weight = 1
description = "# Algebraic Structure"
+++

## Definition

1. **Permutation:** a function from $A$ to $A$ that is one-to-one and onto

2. **Permutation group:** a set of permutations of $A$ that forms a group under function composition

3. **Symmetric group:** $S_n = $ permutations of $\{1, 2, ..., n\}$, $|S_n| = n!$

4. Disjoint cycles commute

5. multiply the following two permutations in cycle notation 

6. Write the permutation as a product of transpositions: $(12)(23)...(n-1n) = (12)(13)...(1n)$ 

7. **Order of a permutation**: The order of a permutation of a finite set is the least common multiple of the lengths of the cycles

8. **Always even or always odd theorem for permutations:** If $\alpha \in S_n$, and $\alpha = t_1...t_k = s_1...s_l$, then $k$ and $l$ are both even or odd

9. If $A_n$ is the subset of even permutations, then $|A_n| = |B_n| = \frac{n!}{2}$, $|A_n|$ is a subgroup

## Exercise

1.  Suppose that H is a subgroup of $S_n$ of odd order. Prove that H is
    a subgroup of $A_n$.

    Lemma: If H is a subgroup of $S_n$, then either every member of H is
    an even permutation or exactly half of the members are even.

    If there is no odd member, then every member of $H$ is an even
    permutation.

    If there is an odd member $a \in H$,

    we can permute an odd member by $ab$ for all even member
    $b \in S_n$, since odd multiples even is odd. Also, since each
    permuted member is unique to each other, the number of odd member
    $\ge$ number of even member.

    For every odd permutation $b \in H$, $ab$ is an even permutation,
    since odd multiplies odd is equal to even. Thus, the number of even
    member $\ge$ number of odd member.

    Thus, if there is odd members, exactly half of the members are even.

    Since we know $H$ is odd order, $H$ has an odd number of elements,
    then $H$ cannot have same number of even and odd members, which
    results in an even order. By lemma, every member of $H$ is an even
    permutation, and therefore $H \in A_n$.

2.  How many elements of order 4 does $S_6$ have? How many elements of
    order 2 does $S_6$ have?

    Since the order is the least common multiple of the length of the
    cycle, the order is 4 iff the length of cycles is 4+2 or 4+1+1.

    We first permute 4 elements from 6, and since the elements is
    circular, we count each circle 4 times.

    There are $$P^6_4 / 4 = 90$$ elements in the group such as their
    cycles are 4+2.

    Similarly, there are $$P^6_4 / 4 = 90$$ elements in the group such
    as their cycles are 4+1+1.

    Thus, there are 90+90=180 elements of order 4 in $S_6$.\
    The possible length of circles for order 2 is 2+1+1+1+1 and 2+2+2
    and 2+2+1+1

    Thus, there are
    $$P^6_2 \times C^4_2 / 3! + C^6_2 + C^6_2C^4_2/2! = 75$$ elements in
    order 2 in $S_6$.

3.  Let G be a group of permutations on a set $X$. Let $a \in X$ and
    define stab(a) $= \{\alpha \in  G | \alpha(a) = a\}$. We call
    stab(a) the stabilizer of a in G (since it consists of all members
    of G that leave a fixed). Prove that stab(a) is a subgroup of G.
    (This subgroup was introduced by Galois in 1832.) This exercise is
    referred to in Chapter 7.

    1.  Let $e$ be the identity in $G$, since $G$ is a group of
        permutations, $e(a) = a$, so $e \in stab(a)$

    2.  Let $\alpha, \beta \in stab(a)$,
        $(\alpha \beta) (a) = \alpha (\beta(a)) = \alpha(a) = a$. Thus,
        $\alpha \beta \in stab(a)$.

    3.  Let $\alpha^{-1}$ be the inverse of $\alpha \in stab(a)$,
        $$\begin{aligned}
            \alpha(a) &= a \\\\
            \alpha^{-1}(\alpha(a)) &= \alpha^{-1}(a) \\\\
            (\alpha^{-1}\alpha)(a) &= \alpha^{-1}(a) \\\\
            e(a) &= \alpha^{-1}(a) \\\\
            a &= \alpha^{-1}(a) \\\\
        \end{aligned}$$

        Thus, $\alpha^{-1} \in stab(a)$

    Thus, stab(a) is a subgroup of G.

4.  Let $H=\{b\in S_5|b(1) = 1, b(3)=3\}$.Prove that H is a
    subgroup of $S_5$. How many elements are in H? Is your argument
    valid when $S_5$ is replaced by $S_n$ for $n \ge 3$? How many
    elements are in H when $S_5$ is replaced by $A_n$ for $n \ge 4$?

    Since $H = \{b\in S_5|b(1) = 1\} \cap \{b\in S_5|b(3) = 3\}$,
    $H= stab(1) \cap stab(3)$. Since the intersection of 2 subgroups are
    subgroups, and we know $stab(1)$ and $stab(3)$ are subgroup of
    $S_5$, $H$ is a subgroup of $S_5$.

    There are $P^3_3 = 3! = 6$ elements in $H$.

    Since $stab(1) \le S_n$, and $stab(3) \le S_n$, so
    $H = stab(1) \cap stab(3) \le H$. Thus, the argument is valid when
    $S_5$ is replaced by $S_n$ for $n \ge 3$

    When $S_5$ is replaced by $S_n$ there are $(n-2)!$ elements $\in H$.

    When $b \in S_n$, we know from the lemma that $H$ either has all
    even members or half even or odd member. Since we can always get an
    odd member by times the odd member with an even member, then $H$ has
    half even and half odd member.

    When $S_5$ is replaced by $A_n$ there are $(n-2)!/2$ elements
    $\in H$.

5.  In S4, find a cyclic subgroup of order 4 and a noncyclic subgroup of
    order 4.

    $\langle (1, 2, 3, 4) \rangle = \{(1, 2, 3, 4), (1, 3)(2, 4), (1, 4, 3, 2), e \}$
    is a cyclic subgroup of order 4, since
    $|\langle a \rangle| = |a| = 4$.

    An noncyclic subgroup is
    $G = \{(1), (2), (1, 2), (3, 4), (1, 2)(3, 4)\}$

    We can confirm it is a subgroup by viewing its Cayley table.

      ---------- ---------- ---------- ---------- ----------
                    (1)        (12)       (34)     (12)(34)
         (1)        (1)        (12)       (34)     (12)(34)
         (12)       (12)       (1)      (12)(34)     (34)
         (34)       (34)     (12)(34)     (1)        (12)
       (12)(34)   (12)(34)     (34)       (12)       (1)
      ---------- ---------- ---------- ---------- ----------

    Since each element has an order of 2, no element can generate a
    group of order 4, the group is not acyclic.

6.  Find a cyclic subgroup of $A_8$ that has order 4.

    An example is $G = \langle (1, 2, 3, 4)(5, 6) \rangle$

    $= \{(1, 2, 3, 4)(5, 6), (1, 3)(2, 4), (1, 4, 3, 2)(5, 6), e \}$

    $(1, 2)(2, 3)(3, 4)(5, 6) = (1, 2, 3, 4)(5, 6)$

    Since the permutation can be expressed as a product of an even
    number of 2-cycles, $a \in A_8$.

    Since $lcm(4, 2) = 4$, the order of $a$ is 4.

    Since $|a|=|\langle a \rangle| = 4$, the group is acyclic.

7.  Shown below are four tire rotation patterns recommended by the
    Dunlop Tire Company. Explain how these patterns can be represented
    as permutations in S4 and find the smallest subgroup of S4 that
    contains these four patterns. Is the subgroup Abelian?

    We can treat each tire as a number as shown in the above picture,
    and the arrow be a function mapped a tire to another tire.

    Thus, each vehicles from top left to bottom right can be expressed
    as:

    a = (1423)

    b = (1324)

    c = (14)(23)

    d = (13)(24)

    Since $a^{-1} = (1324) = b$, and
    $b^2c = (1324)^2(14)(23) = (13)(24) = d$, we can generate a, b, c, d
    with b, c, $\langle a, b, c, d \rangle = \langle b, c \rangle$.

    Since $|\langle b \rangle| = |b| = |(1324)| = 4$, and
    $|\langle c \rangle| = |c| = 2$, also since there is another
    relation $cb^{-1} = bc = (34)$, the smallest subgroup is
    $G = \{e, b, b^2, b^3, c, bc, b^2c, b^3c\}$.

    By counterexample,

    $bc = (1324)(14)(23) = (34)$

    $cb = (14)(23)(1324) = (12)$

    Since $bc \neq cb$, the subgroup is not Abelian.

8.  Find 2 permutations in $A_4$ (the alternating group of even
    permutations in $S_4$) a and b, so that a and b are squares in A4
    (i.e., $a  = x^2$ and $b = y^2$ for x and y in A4) but ab is not a
    square in A4. Show that this solves the extra credit problem from
    HW2. (This is the smallest group that has this property).

    From the table, we can see $e$ and every 3-cycle permutation forms
    $K=\{g^2 \in A_4 | g \in A_4\}$, since the square of the element is
    either a 3-cycle or the identity. However, it is not a subgroup of
    $A_4$, since $(132)(142) = (13)(24) \not \in K$, so it is not closed
    under operation. Since $A_4$ is not Abelian, this serves as an
    example.
