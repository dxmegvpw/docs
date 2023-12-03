---
layout: default
title: Senior thesis
---

# Detail of the computation

We feel frustrated with the challenging computations involved in studying SUSY. I will document the process of such challenging computations.

## Derivation of the  zero-mode equations

10D SYM action in $\mathcal{N}=1$ is given by
$$
    \begin{equation}
        S
        =
        \int\text{d}^{10}X
        \sqrt{-G}
        \left[
            \int\text{d}^{4}\theta\ 
            \mathcal{K}
            +
            \left\{
                \int\text{d}^{2}\theta
                \left(
                    \frac{1}{4g^2}
                    \text{Tr}\ \mathcal{W}^{\alpha}\mathcal{W} _ {\alpha}
                    +
                    \mathcal{W}
                \right)
                +
                \text{h.c.}
            \right\}
        \right]
    \end{equation}
$$
where
$$
    \begin{align}
        \mathcal{K}
        &=
        \frac{2}{g^2}
        h^{\bar{i}j}
        \text{Tr}
        \left[
            \left\{
            (
                \sqrt{2}\bar{\partial _ {\bar{i}}}
                +
                \bar{\phi} _ {\bar{i}}
            )
            e^{-V}
            \right\}
            \left\{
            (
                \sqrt{2}\partial _ {j}
                +
                \phi _ {j}
            )
            e^{V}
            \right\}
        \right.
        \nonumber
        \\
        &\hspace{100pt}
        \left.
            +
            (
                \bar{\partial} _ {\bar{i}}e^{-V}
            )
            (
                \partial _ {j}e^{V}
            )
        \right]
        +
        \mathcal{K} _ \text{WZW}
        ,
        \\
        \mathcal{W}
        &=
        \frac{1}{g^2}
        \varepsilon^{\text{ijk}}
        e^{\ i} _ {\text{i}}e^{\ j} _ {\text{j}}e^{\ k} _ {\text{k}}
        \text{Tr}
        \left[
            \sqrt{2}\phi _ {i}
            \left(
                \partial _ {j}\phi _ {k}
                -
                \frac{1}{3\sqrt{2}}[\phi _ {j},\phi _ {k}]
            \right)
        \right]
        .
    \end{align}
$$
The term $\mathcal{K} _ \text{WZW}$ is so called Wess-Zumino-Witten term which vanishes when we take Wess-Zumino gauge
$$
    \begin{align}
        V
        &=
        -
        \theta\sigma^{\mu}\bar{\theta}A _ {\mu}
        +
        i\overline{\theta\theta}\theta\lambda _ {0}
        -
        i\theta\theta\overline{\theta\lambda} _ {0}
        +
        \frac{1}{2}\theta\theta\overline{\theta\theta}D
        ,
        \\
        \phi _ {i}
        &=
        \frac{1}{\sqrt{2}}
        A _ i
        +
        \sqrt{2}\theta\lambda _ {i}
        +
        \theta\theta F _ {i}.
    \end{align}
$$

### SUSY condition

By carrying out the derivative with respect to the $F _ {i}$ and $D _ {i}$, we can obtain the on-shell relation of the auxiliary fields. First, let us focus on the Kähler potential. The term inside the trace become
$$
    \begin{align}
        &\hspace{10pt}
        \left\{
            (
                \sqrt{2}\bar{\partial _ {\bar{i}}}
                +
                \bar{\phi} _ {\bar{i}}
            )
            e^{-V}
        \right\}
        \left\{
            (
                \sqrt{2}\partial _ {j}
                +
                \phi _ {j}
            )
            e^{V}
            \right\}
            +
            (
                \bar{\partial} _ {\bar{i}}e^{-V}
            )
            (
                \partial _ {j}e^{V}
            )
        \nonumber
        \\
        &=
        \left\{
            (
                \sqrt{2}\bar{\partial _ {\bar{i}}}
                +
                \bar{\phi} _ {\bar{i}}
            )
            \left(
                1-V+\frac{1}{2}V^2
            \right)
        \right\}
        \left\{
            (
                \sqrt{2}\partial _ {j}
                +
                \phi _ {j}
            )
            \left(
                1+V+\frac{1}{2}V^2
            \right)
        \right\}
        \nonumber
        \\
        &\hspace{50pt}
        +
        \bar{\partial} _ {\bar{i}}
            \left(
                1-V+\frac{1}{2}V^2
            \right)
        \partial _ {j}
            \left(
                1+V+\frac{1}{2}V^2
            \right)
        \nonumber
        \\
        &=
        \bar{\phi} _ {\bar{i}}\phi _ {j}
        -
        \sqrt{2}\bar{\phi} _ {\bar{i}}(\partial _ {j}V)
        +
        \bar{\phi} _ {\bar{i}}\phi _ {j}V
        -
        \frac{1}{\sqrt{2}}\bar{\phi} _ {\bar{i}}(\partial _ {j}V)V
        -
        \frac{1}{\sqrt{2}}\bar{\phi} _ {\bar{i}}V(\partial _ {j}V)+\frac{1}{2}\bar{\phi} _ {\bar{i}}\phi _ {j}V^2
        \nonumber
        \\
        &\quad
        -
        \sqrt{2}(\bar{\partial} _ {\bar{i}}V)\phi _ {j}
        +
        (\bar{\partial} _ {\bar{i}}V)(\partial _ {j}V)
        -
        \sqrt{2}(\bar{\partial} _ {\bar{i}}V)\phi _ {j}V
        -
        \bar{\phi} _ {\bar{i}}V\phi _ {j}
        +
        \sqrt{2}\bar{\phi} _ {\bar{i}}
        V
        \partial _ {j}V
        \nonumber
        \\
        &\quad
        -
        \bar{\phi} _ {\bar{i}}
        V
        \phi _ {j}
        V
        +
        \frac{1}{\sqrt{2}}
        (\bar{\partial} _ {\bar{i}}V)V\phi _ {j}
        +
        \frac{1}{\sqrt{2}}V(\bar{\partial} _ {\bar{i}}V)\phi _ {j}
        +
        \frac{1}{2}\bar{\phi} _ {\bar{i}}V^2\phi _ {j}
        .
    \end{align}
$$
This is the only term that contains the auxiliary $D$. Note that the action $S$ contains only the highest term $\theta^4$ from the Kähler potential $\mathcal{K}$. Thus when we take the derivative to the $D$, the term which has only one $V$ will remain[^1]. After integrating by parts, for removing the factor the derivative of vector superfield, for instance, the term $\bar{\phi} _ {\bar{i}}\partial _ {j}V$, we find
$$
    \begin{align}
        \frac{\delta \mathcal{S}}{\delta D}
        &=        
        \sqrt{-G}      
        \frac{2}{g^2}
        h^{\bar{i}j}
        \left[
            \partial _ {j}\bar{A} _ {\bar{i}}
            +
            \frac{1}{2}\bar{A} _ {\bar{i}}A _ {j}
            +
            \bar{\partial} _ {\bar{i}}A _ {j}
            -
            \frac{1}{2}A _ {j}\bar{A} _ {\bar{i}}
        \right]
        \nonumber
        \\
        &\hspace{20pt}+
        \frac{1}{4g^2}
        \frac{\delta}{\delta D}
        \int\text{d}^{10}X\sqrt{-G}
        \left[
            \int\text{d}^{2}\theta\ \text{Tr}\ \mathcal{W}^{\alpha}\mathcal{W} _ {\alpha}
            +  
            \int\text{d}^{2}\bar{\theta}\ \text{Tr}\ \overline{\mathcal{W} _ {\dot{\alpha}}\mathcal{W}^{\dot{\alpha}}}
        \right]
        .
    \end{align}
$$
Note that we should be careful about the derivatives of the term like $\bar{\phi} _ {\bar{i}}V\phi _ {j}$. We derivate with respect to the auxiliary $D$, but it actually has the indices of the gauge group, $D _ {AB}$. Therefore we obtain
$$
    \begin{align}    
        \left.
        \frac{\delta}{\delta D _ {AB}}
        \text{Tr}
        \left[\bar{\phi} _ {\bar{i}}V\phi _ {j}\right]
        \right| _ {\theta^4}
        &=
        \frac{1}{2}
        \frac{\delta}{\delta D _ {AB}} 
        (\bar{A} _ {\bar{i}}) _ {CD}    
        (D) _ {DE} 
        (A _ {j}) _ {EC}
        \nonumber
        \\
        &=
        \frac{1}{2}
        (\bar{A} _ {\bar{i}}) _ {CA}    
        (A _ {j}) _ {BC}
        =
        \frac{1}{2}
        (A _ {j}\bar{A} _ {\bar{i}}) _ {AB}
        .
    \end{align}
$$
The term including $\text{Tr}\ \mathcal{W}^{\alpha}\mathcal{W} _ {\alpha}$ and its hermitian conjugate is well-known[^2]. That is
$$
    \begin{equation}
        \text{Tr}\ 
        \mathcal{W}^{\alpha}
        \mathcal{W} _ {\alpha}
        =
        2
        \text{Tr}
        \left[
            D^2
            +
            \cdots
        \right]
    \end{equation}
$$
and the variation of the action is
$$
    \begin{align}
        \frac{\delta S}{\delta D}
        =
        \sqrt{-G}\frac{2}{g^2}
        \left[
            D
            +
            h^{\bar{i}j}
            \left(
                \partial _ {j}\bar{A} _ {\bar{i}}
                +
                \bar{\partial} _ {\bar{i}}A _ {j}   
                +
                \frac{1}{2}[\bar{A} _ {\bar{i}},A _ {j}]
            \right)
        \right]
        =
        0
        .
    \end{align}
$$
Finally we get
$$
    \begin{equation}
        D
        =
        -h^{\bar{i}j}
        \left(
            \partial _ {j}\bar{A} _ {\bar{i}}
            +
            \bar{\partial} _ {\bar{i}}A _ {j}   
            +
            \frac{1}{2}[\bar{A} _ {\bar{i}},A _ {j}]
        \right)
    \end{equation}
$$
for the equation of motion with respect to the auxiliary $D$. Let us move on to the computation for the auxiliary $F _ i$. $F _ {i}$ is included by the superfield $\phi _ {i}$ that appears only in Kähler potential $\mathcal{K}$ and super potential $\mathcal{W}$, not in field strength $\mathcal{W}^{\alpha}$. The highest component containing the auxiliary $F _ {i}$ comes from the term $\bar{\phi} _ {\bar{i}}\phi _ {j}$ in Kähler potential. Thus the Kähler potential including $F$ is
$$
    \begin{equation}
        \mathcal{K}
        \rightarrow
        \frac{2}{g^2} h^{\bar{i}j}
        \text{Tr}
        \left[
            \bar{F} _ {\bar{i}}F _ {j}
        \right]
        .
    \end{equation}
$$
From superpotential, we can get the term related auxiliary $F$ as
$$
    \begin{align}
        \mathcal{W}
        &=
        \frac{1}{g^2}
        \varepsilon^{\text{ijk}}
        e^{\ i} _ {\text{i}}e^{\ j} _ {\text{j}}e^{\ k} _ {\text{k}}
        \text{Tr}
        \left[
            \sqrt{2}\phi _ {i}
            \left(
                \partial _ {j}\phi _ {k}
                -
                \frac{1}{3\sqrt{2}}[\phi _ {j},\phi _ {k}]
            \right)
        \right]
        \nonumber
        \\
        &\rightarrow
        \frac{1}{g^2}
        \varepsilon^{\text{ijk}}
        e^{\ i} _ {\text{i}}e^{\ j} _ {\text{j}}e^{\ k} _ {\text{k}}
        \text{Tr}
        \left[
            \vphantom{\frac{1}{6}}
            A _ {i}\partial _ {j}F _ {k}
            +
            F _ {i}\partial _ {j}A _ {k}
        \right.
        \nonumber
        \\
        &\hspace{50pt}
        \left.
            -
            \frac{1}{6}
            \left(
                F _ {i}[A _ {j},A _ {k}]
                +
                A _ {i}[F _ {j},A _ {k}]
                +
                A _ {i}[A _ {j},F _ {k}]
            \right)
        \right]
        ,
        \\
        \overline{\mathcal{W}}
        &\rightarrow
        \frac{1}{g^2}
        \varepsilon^{\bar{\text{i}}\bar{\text{j}}\bar{\text{k}}}
        e^{\ \bar{i}} _ {\bar{\text{i}}}e^{\ \bar{j}} _ {\bar{\text{j}}}e^{\ \bar{k}} _ {\bar{\text{k}}}
        \text{Tr}
        \left[
            \vphantom{\frac{1}{6}}
            \bar{A} _ {\bar{i}}\bar{\partial} _ {\bar{j}}\bar{F} _ {\bar{k}}
            +
            \bar{F} _ {\bar{i}}\bar{\partial} _ {\bar{j}}\bar{F} _ {\bar{k}}
        \right.
        \nonumber
        \\
        &\hspace{50pt}
        \left.
            -
            \frac{1}{6}
            \left(
                \bar{F} _ {\bar{i}}[\bar{A} _ {\bar{j}},\bar{A} _ {\bar{k}}]
                +
                \bar{A} _ {\bar{i}}[\bar{F} _ {\bar{j}},\bar{A} _ {\bar{k}}]
                +
                \bar{A} _ {\bar{i}}[\bar{A} _ {\bar{j}},\bar{F} _ {\bar{k}}]
            \right)
        \right]
        .
    \end{align}
$$
By derivating to the $F _ {i}$, the term in the action become separately
$$
    \begin{align}
        \frac{\delta}{\delta F _ {i}}
        \int\text{d}^{10}X\sqrt{-G}\int\text{d}^{4}\theta\ \mathcal{K}
        &=
        \sqrt{-G}\frac{2}{g^2}
        \frac{\delta}{\delta F _ {i}}
        h^{\bar{a}b}\text{Tr}\ 
        \bar{F} _ {\bar{a}}F _ {b}    
        \nonumber    
        \\
        &=
        \sqrt{-G}\frac{2}{g^2}
        h^{\bar{j}i}
        \text{Tr}\ \bar{F} _ {\bar{j}}
        ,
        \\
        \frac{\delta}{\delta F _ {i}}
        \int\text{d}^{10}X\sqrt{-G}\int\text{d}^{2}\theta\ \mathcal{W}
        &=
        \sqrt{-G}\frac{1}{g^2}
        \varepsilon^{\text{ijk}}
        e^{\ i} _ {\text{i}}e^{\ j} _ {\text{j}}e^{\ k} _ {\text{k}}        
        \frac{\delta}{\delta F _ {i}}
        \text{Tr}\ 
        \left[
            \vphantom{\frac{1}{6}}
            A _ {i}\partial _ {j}F _ {k}
            +
            F _ {i}\partial _ {j}A _ {k}
        \right.
        \nonumber
        \\
        &\hspace{30pt}
        \left.
            -
            \frac{1}{6}
            \left(
                F _ {i}[A _ {j},A _ {k}]
                +
                A _ {i}[F _ {j},A _ {k}]
                +
                A _ {i}[A _ {j},F _ {k}]
            \right)
        \right]
        \nonumber
        \\
        &=
        \sqrt{-G}\frac{1}{g^2}
        \varepsilon^{\text{ijk}}
        e^{\ i} _ {\text{i}}e^{\ j} _ {\text{j}}e^{\ k} _ {\text{k}} 
        \text{Tr}\ 
        \left[
            2\partial _ {j}A _ {k}
            -
            \frac{1}{2}[A _ {j},A _ {k}]
        \right]
        .
    \end{align}
$$
Note that we have interchanged the dummy indices several times after derivating. At last, the equation of motion with respect to the $F _ {i}$
$$
    \begin{equation}
        h^{\bar{j}i}\bar{F} _ {\bar{j}}
        +        
        \varepsilon^{\text{ijk}}
        e^{\ i} _ {\text{i}}e^{\ j} _ {\text{j}}e^{\ k} _ {\text{k}} 
        \left[
            \partial _ {j}A _ {k}
            -
            \frac{1}{4}[A _ {j},A _ {k}]     
        \right]
        =
        0   
    \end{equation}
$$
or equivalently
$$
    \begin{equation}
        \bar{F} _ {\bar{i}}
        =
        -
        h _ {j\bar{i}}
        \varepsilon^{\text{jkl}}
        e^{\ j} _ {\text{j}}e^{\ k} _ {\text{k}}e^{\ l} _ {\text{l}}
        \left[
            \partial _ {k}A _ {l}
            -
            \frac{1}{4}[A _ {k},A _ {l}]     
        \right]
    \end{equation}
$$
holds.

### Lagrangian with the field fluctuations

We set VEV's for
$$
    \begin{equation}
        \braket{V}
        =
        0
        ,\quad
        \braket{\phi _ {i}}
        \neq 
        0
        .
    \end{equation}
$$
Thus the Kähler potential satisfies
$$
    \begin{align}
        \mathcal{K}
        &=
        \frac{2}{g^2}h^{\bar{i}j}
        \text{Tr}\left[\vphantom{\frac{1}{2}}\right.
            \underline{\bar{\phi} _ {\bar{i}}\phi _ {j}}
            +
            \braket{\bar{\phi} _ {\bar{i}}}\phi _ {j}
            +        
            \bar{\phi} _ {\bar{i}}\braket{\phi _ {j}}
            +
            \braket{\bar{\phi} _ {\bar{i}}}\braket{\phi _ {j}}
            -
            \underline{\sqrt{2}\bar{\phi} _ {\bar{i}}(\partial _ {j}V)}
            -
            \underline{\sqrt{2}\braket{\bar{\phi} _ {\bar{i}}}(\partial _ {j}V)}
        \nonumber
        \\
        &\qquad
            +
            \underline{\bar{\phi} _ {\bar{i}}\phi _ {j}V}
            +
            \underline{\braket{\bar{\phi} _ {\bar{i}}}\phi _ {j}V}
            +
            \underline{\bar{\phi} _ {\bar{i}}\braket{\phi _ {j}}V}
            +
            \braket{\bar{\phi} _ {\bar{i}}}\braket{\phi _ {j}}V
        \nonumber
        \\
        &\qquad
            -
            \underline{\frac{1}{\sqrt{2}}\bar{\phi} _ {\bar{i}}(\partial _ {j}V)V}
            -
            \underline{\frac{1}{\sqrt{2}}\braket{\bar{\phi} _ {\bar{i}}}(\partial _ {j}V)V}
            -
            \underline{\frac{1}{\sqrt{2}}\bar{\phi} _ {\bar{i}}V(\partial _ {j}V)}
            -
            \underline{\frac{1}{\sqrt{2}}\braket{\bar{\phi} _ {\bar{i}}}V(\partial _ {j}V)}
        \nonumber
        \\
        &\qquad
            +
            \underline{\frac{1}{2}\bar{\phi} _ {\bar{i}}\phi _ {j}V^2}
            +
            \underline{\frac{1}{2}\braket{\bar{\phi} _ {\bar{i}}}\phi _ {j}V^2}
            +
            \underline{\frac{1}{2}\bar{\phi} _ {\bar{i}}\braket{\phi _ {j}}V^2}
            +
            \underline{\frac{1}{2}\braket{\bar{\phi} _ {\bar{i}}}\braket{\phi _ {j}}V^2}
        \nonumber
        \\
        &\qquad
            -
            \underline{\sqrt{2}(\bar{\partial} _ {\bar{i}}V)\phi _ {j}}
            -
            \underline{\sqrt{2}(\bar{\partial} _ {\bar{i}}V)\braket{\phi _ {j}}}
            +
            \underline{(\bar{\partial} _ {\bar{i}}V)(\partial _ {j}V)}
        \nonumber
        \\
        &\qquad
            -
            \underline{\sqrt{2}(\bar{\partial} _ {\bar{i}}V)\phi _ {j}V}
            -
            \underline{\sqrt{2}(\bar{\partial} _ {\bar{i}}V)\braket{\phi _ {j}}V}
        \nonumber
        \\
        &\qquad
            -
            \underline{\bar{\phi} _ {\bar{i}}V\phi _ {j}}
            -
            \underline{\braket{\bar{\phi} _ {\bar{i}}}V\phi _ {j}}
            -
            \underline{\bar{\phi} _ {\bar{i}}V\braket{\phi _ {j}}}
            -
            \braket{\bar{\phi} _ {\bar{i}}}V\braket{\phi _ {j}}
            +
            \underline{\sqrt{2}\bar{\phi} _ {\bar{i}}
            V
            \partial _ {j}V}
            +
            \underline{\sqrt{2}\braket{\bar{\phi} _ {\bar{i}}}
            V
            \partial _ {j}V}
        \nonumber
        \\
        &\qquad
            -
            \underline{\bar{\phi} _ {\bar{i}}
            V
            \phi _ {j}
            V}
            -
            \underline{\braket{\bar{\phi} _ {\bar{i}}}
            V
            \phi _ {j}
            V}
            -
            \underline{\bar{\phi} _ {\bar{i}}
            V
            \braket{\phi _ {j}}
            V}
            -
            \underline{\braket{\bar{\phi} _ {\bar{i}}}
            V
            \braket{\phi _ {j}}}
            V
        \nonumber
        \\
        &\qquad
            +
            \underline{\frac{1}{\sqrt{2}}
            (\bar{\partial} _ {\bar{i}}V)V\phi _ {j}}
            +
            \underline{\frac{1}{\sqrt{2}}
            (\bar{\partial} _ {\bar{i}}V)V\braket{\phi _ {j}}}
            +
            \underline{\frac{1}{\sqrt{2}}V(\bar{\partial} _ {\bar{i}}V)\phi _ {j}}
            +
            \underline{\frac{1}{\sqrt{2}}V(\bar{\partial} _ {\bar{i}}V)\braket{\phi _ {j}}}
        \nonumber
        \\
        &\qquad
            +
            \underline{\frac{1}{2}\bar{\phi} _ {\bar{i}}V^2\phi _ {j}}
            +
            \underline{\frac{1}{2}\braket{\bar{\phi} _ {\bar{i}}}V^2\phi _ {j}}
            +
            \underline{\frac{1}{2}\bar{\phi} _ {\bar{i}}V^2\braket{\phi _ {j}}}
            +
            \underline{\frac{1}{2}\braket{\bar{\phi} _ {\bar{i}}}V^2\braket{\phi _ {j}}}
        \left.\vphantom{\frac{1}{2}}
        \right]
        \nonumber
        \\
        &=
        \frac{2}{g^2}h^{\bar{i}j}\text{Tr}\left[\vphantom{\frac{1}{2}}\right.
            \bar{\phi} _ {\bar{i}}\phi _ {j}
            +
            \sqrt{2}(\bar{\partial} _ {\bar{i}}\phi _ {j}+\partial _ {j}\bar{\phi} _ {\bar{i}})V
            +
            [\bar{\phi} _ {\bar{i}},\phi _ {j}]V
        \nonumber
        \\
        &\hspace{10pt}
            +
            \sqrt{2}
            \left\{
                \left(
                    \bar{\partial} _ {\bar{i}}\phi _ {j}
                    +
                    \frac{1}{\sqrt{2}}[\braket{\bar{\phi} _ {\bar{i}}},\phi _ {j}]
                \right)
                +
                \left(
                    \partial _ {j}\bar{\phi} _ {\bar{i}}
                    -
                    \frac{1}{\sqrt{2}}[\braket{\phi _ {j}},\bar{\phi} _ {\bar{i}}]
                \right)
            \right\}
            V
        \nonumber
        \\
        &\hspace{10pt}
            +
            \left(
                \bar{\partial} _ {\bar{i}}V
                +
                \frac{1}{\sqrt{2}}[\braket{\bar{\phi} _ {\bar{i}}},V]
                +
                \frac{1}{\sqrt{2}}[\bar{\phi} _ {\bar{i}},V]
            \right)
            \left(
                \partial _ {j}V
                -
                \frac{1}{\sqrt{2}}[\braket{\phi _ {j}},V]
                -
                \frac{1}{\sqrt{2}}[\phi _ {j},V]
            \right)
        \left.\vphantom{\frac{1}{2}}\right]
        \nonumber
        \\
        &\quad
        +
        \frac{2}{g^2}h^{\bar{i}j}\text{Tr}\ \left[\vphantom{\frac{1}{2}}\right.
            \braket{\bar{\phi} _ {\bar{i}}}\phi _ {j}
            +        
            \bar{\phi} _ {\bar{i}}\braket{\phi _ {j}}
            +
            \braket{\bar{\phi} _ {\bar{i}}}\braket{\phi _ {j}}
        \nonumber
        \\
        &\hspace{100pt}
            +
            \braket{\bar{\phi} _ {\bar{i}}}\braket{\phi _ {j}}V
            -
            \braket{\bar{\phi} _ {\bar{i}}}V\braket{\phi _ {j}}
        \left.\vphantom{\frac{1}{2}}\right]
        \\
        &\equiv
        \mathcal{K}^{(0)}+\mathcal{K}^{(D)}
        ,
        \nonumber
    \end{align}
$$
where
$$
    \begin{align}
        \mathcal{K}^{(0)}
        &=
        \frac{2}{g^2}h^{\bar{i}j}\text{Tr}\left[\vphantom{\frac{1}{2}}\right.
            \bar{\phi} _ {\bar{i}}\phi _ {j}
            +
            \sqrt{2}(\bar{\partial} _ {\bar{i}}\phi _ {j}+\partial _ {j}\bar{\phi} _ {\bar{i}})V
            +
            [\bar{\phi} _ {\bar{i}},\phi _ {j}]V
        \nonumber
        \\
        &\hspace{5pt}
            +
            \sqrt{2}
            \left\{
                \left(
                    \bar{\partial} _ {\bar{i}}\phi _ {j}
                    +
                    \frac{1}{\sqrt{2}}[\braket{\bar{\phi} _ {\bar{i}}},\phi _ {j}]
                \right)
                +
                \left(
                    \partial _ {j}\bar{\phi} _ {\bar{i}}
                    -
                    \frac{1}{\sqrt{2}}[\braket{\phi _ {j}},\bar{\phi} _ {\bar{i}}]
                \right)
            \right\}
            V
        \nonumber
        \\
        &\hspace{5pt}
            +
            \left(
                \bar{\partial} _ {\bar{i}}V
                +
                \frac{1}{\sqrt{2}}[\braket{\bar{\phi} _ {\bar{i}}},V]
                +
                \frac{1}{\sqrt{2}}[\bar{\phi} _ {\bar{i}},V]
            \right)
            \left(
                \partial _ {j}V
                -
                \frac{1}{\sqrt{2}}[\braket{\phi _ {j}},V]
                -
                \frac{1}{\sqrt{2}}[\phi _ {j},V]
            \right)
        \left.\vphantom{\frac{1}{2}}\right]
        \nonumber
        \\
        \mathcal{K}^{(D)}
        &=        
        \frac{2}{g^2}h^{\bar{i}j}\text{Tr}\ \left[\vphantom{\frac{1}{2}}\right.
            \braket{\bar{\phi} _ {\bar{i}}}\phi _ {j}
            +        
            \bar{\phi} _ {\bar{i}}\braket{\phi _ {j}}
            +
            \braket{\bar{\phi} _ {\bar{i}}}\braket{\phi _ {j}}
        \nonumber
        \\
        &\hspace{100pt}
            +
            \braket{\bar{\phi} _ {\bar{i}}}\braket{\phi _ {j}}V
            -
            \braket{\bar{\phi} _ {\bar{i}}}V\braket{\phi _ {j}}
        \left.\vphantom{\frac{1}{2}}\right]
    \end{align}
$$
Note that we have used the cyclic property of the trace $\text{Tr}AB=\text{Tr}BA$, and the underline $\underline{\cdots}$ at the first line is the non-zero term.

Let us focus on the superpotential $\mathcal{W}$.
$$
    \begin{align}
        \mathcal{W}
        &=
        \frac{1}{g^2}
        \varepsilon^{\text{ijk}}
        e^{\ i} _ {\text{i}}e^{\ j} _ {\text{j}}e^{\ k} _ {\text{k}}
        \text{Tr}
        \left[\vphantom{\frac{1}{2}}\right.
            \sqrt{2}(\phi _ {i}+\braket{\phi _ {i}})\partial _ {j}\phi _ {k}
        \\
        &\qquad
            -
            \frac{1}{3}(\phi _ {i}+\braket{\phi _ {i}})[\phi _ {j}+\braket{\phi _ {j}},\phi _ {k}+\braket{\phi _ {k}}]
        \left.\vphantom{\frac{1}{2}}\right] 
        \nonumber
        \\
        &=
        \frac{1}{g^2}
        \varepsilon^{\text{ijk}}
        e^{\ i} _ {\text{i}}e^{\ j} _ {\text{j}}e^{\ k} _ {\text{k}}
        \text{Tr}
        \left[\vphantom{\frac{1}{2}}\right.
            \underline{\sqrt{2}\phi _ {i}\partial _ {j}\phi _ {k}}
            +
            \sqrt{2}\braket{\phi _ {i}}\partial _ {j}\phi _ {k}
        \nonumber
        \\
        &\qquad
            -
            \underline{\frac{1}{3}\phi _ {i}[\phi _ {j},\phi _ {k}]}
            -
            \underline{\frac{1}{3}\phi _ {i}[\braket{\phi _ {j}},\phi _ {k}]}
            -
            \underline{\frac{1}{3}\phi _ {i}[\phi _ {j},\braket{\phi _ {k}}]}
            -
            \frac{1}{3}\phi _ {i}[\braket{\phi _ {j}},\braket{\phi _ {k}}]
        \nonumber
        \\
        &\qquad
            -
            \underline{\frac{1}{3}\braket{\phi _ {i}}[\phi _ {j},\phi _ {k}]}
            -
            \frac{1}{3}\braket{\phi _ {i}}[\braket{\phi _ {j}},\phi _ {k}]
            -
            \frac{1}{3}\braket{\phi _ {i}}[\phi _ {j},\braket{\phi _ {k}}]
            -
            \frac{1}{3}\braket{\phi _ {i}}[\braket{\phi _ {j}},\braket{\phi _ {k}}]
        \left.\vphantom{\frac{1}{2}}\right] 
        \nonumber
        \\
        &=
        \frac{1}{g^2}
        \varepsilon^{\text{ijk}}
        e^{\ i} _ {\text{i}}e^{\ j} _ {\text{j}}e^{\ k} _ {\text{k}}
        \text{Tr}
        \left[\vphantom{\frac{1}{2}}\right.
            \sqrt{2}
            \left(
                \partial _ {i}\phi _ {j}
                -
                \frac{1}{\sqrt{2}}[\braket{\phi _ {i}},\phi _ {j}]
            \right)
            \phi _ {k}
            -
            \frac{2}{3}\phi _ {i}\phi _ {j}\phi _ {k}        
        \left.\vphantom{\frac{1}{2}}\right]
        \nonumber
        \\
        &\qquad
        +
        \frac{1}{g^2}
        \varepsilon^{\text{ijk}}
        e^{\ i} _ {\text{i}}e^{\ j} _ {\text{j}}e^{\ k} _ {\text{k}}
        \text{Tr}
        \left[\vphantom{\frac{1}{2}}\right.
            \sqrt{2}\braket{\phi _ {i}}\partial _ {j}\phi _ {k}   
            -
            \frac{1}{3}\braket{\phi _ {i}}[\braket{\phi _ {j}},\phi _ {k}]
            -
            \frac{1}{3}\phi _ {i}[\braket{\phi _ {j}},\braket{\phi _ {k}}]
        \nonumber
        \\
        &\hspace{100pt}
            -
            \frac{1}{3}\braket{\phi _ {i}}[\braket{\phi _ {j}},\phi _ {k}]
            -
            \frac{1}{3}\braket{\phi _ {i}}[\braket{\phi _ {j}},\braket{\phi _ {k}}]
        \left.\vphantom{\frac{1}{2}}\right]
        \\
        &\equiv
        \mathcal{W}^{(0)}
        +
        \mathcal{W}^{(F)}
        \nonumber
    \end{align}
$$
where
$$
    \begin{align}
        \mathcal{W}^{(0)}
        &=
        \frac{1}{g^2}
        \varepsilon^{\text{ijk}}
        e^{\ i} _ {\text{i}}e^{\ j} _ {\text{j}}e^{\ k} _ {\text{k}}
        \text{Tr}
        \left[\vphantom{\frac{1}{2}}\right.
            \sqrt{2}
            \left(
                \partial _ {i}\phi _ {j}
                -
                \frac{1}{\sqrt{2}}[\braket{\phi _ {i}},\phi _ {j}]
            \right)
            \phi _ {k}
            -
            \frac{2}{3}\phi _ {i}\phi _ {j}\phi _ {k}        
        \left.\vphantom{\frac{1}{2}}\right]
        ,
        \\
        \mathcal{W}^{(F)}
        &=
        \frac{1}{g^2}
        \varepsilon^{\text{ijk}}
        e^{\ i} _ {\text{i}}e^{\ j} _ {\text{j}}e^{\ k} _ {\text{k}}
        \text{Tr}
        \left[\vphantom{\frac{1}{2}}\right.
            \sqrt{2}\braket{\phi _ {i}}\partial _ {j}\phi _ {k}
        \nonumber
        \\
        &\hspace{100pt}
            -
            2\phi _ {i}\braket{\phi _ {j}}\braket{\phi _ {k}}
            -
            \frac{2}{3}\braket{\phi _ {i}}\braket{\phi _ {j}}\braket{\phi _ {k}}
        \left.\vphantom{\frac{1}{2}}\right]
        .
    \end{align}
$$
We have used the property that the indices $i,j,k$ are totally antisymmetric because of the coefficient $\varepsilon^{\text{ijk}}$ and the cyclicity inside the trace.

### Do $\mathcal{K}^{(D)}$ and $\mathcal{W}^{(F)}$ really vanish?

We will check that $\mathcal{K}^{(D)}$ and $\mathcal{W}^{(F)}$ are vanished if we impose the SUSY condition. For the Kähler potential $\mathcal{K}^{(D)}$, only $\theta^4$ terms remains in the action $S$[^3]. Thus after taking VEV's it yields
$$
    \begin{align}
        \int\text{d}^4\theta\ \mathcal{K}^{(D)}
        &=
        \int\text{d}^4\theta\ \frac{2}{g^2}h^{\bar{i}j}\text{Tr}\ \left[\vphantom{\frac{1}{2}}\right.
            \braket{\bar{\phi} _ {\bar{i}}}\braket{\phi _ {j}}V
            -
            \braket{\bar{\phi} _ {\bar{i}}}V\braket{\phi _ {j}}
        \left.\vphantom{\frac{1}{2}}\right]
        \nonumber
        \\
        &=
        \frac{1}{g^2}h^{\bar{i}j}\text{Tr}\ \left[\vphantom{\frac{1}{2}}\right.
            \frac{1}{2}\braket{\bar{A} _ {\bar{i}}}\braket{A _ {j}}D
            -
            \frac{1}{2}\braket{A _ {j}}  \braket{A _ {\bar{i}}}D
        \left.\vphantom{\frac{1}{2}}\right]
        =
        0
    \end{align}
$$
The first term at the second line vanished because of the commutativity of the VEV's $\braket{\bar{A} _ {\bar{i}}}\braket{A _ {j}}=\braket{A _ {j}}\braket{\bar{A} _ {\bar{i}}}$. The second one also vanishes
$$
    \begin{align}
        \int\text{d}^2\theta\ 
        \mathcal{W}^{(F)}
        &=        
        \int\text{d}^2\theta\ 
        \frac{1}{g^2}
        \varepsilon^{\text{ijk}}
        e^{\ i} _ {\text{i}}e^{\ j} _ {\text{j}}e^{\ k} _ {\text{k}}
        \text{Tr}
        \left[\vphantom{\frac{1}{2}}\right.
            \sqrt{2}\braket{\phi _ {i}}\partial _ {j}\phi _ {k}
            -
            2\phi _ {i}\braket{\phi _ {j}}\braket{\phi _ {k}}
        \left.\vphantom{\frac{1}{2}}\right]
        \nonumber
        \\
        &=        
        \frac{1}{g^2}
        \varepsilon^{\text{ijk}}
        e^{\ i} _ {\text{i}}e^{\ j} _ {\text{j}}e^{\ k} _ {\text{k}}
        \text{Tr}
        \left[\vphantom{\frac{1}{2}}\right.
            \braket{A _ {i}}\partial _ {j}F _ {k}
            -
            \frac{1}{2}
            F _ {i}\braket{A _ {j}}\braket{A _ {k}}
        \left.\vphantom{\frac{1}{2}}\right]
        =
        0
        ,
    \end{align}
$$
because of the commutativity of the VEV too[^4].


## Effective SUGRA

The action for 4D $\mathcal{N}=1$ conformal supergravity is written as
$$
    \begin{align}
        S _ {\mathcal{N}=1}
        &=
        \int\text{d}^4x\ \sqrt{-g^{C}}
            \left[\vphantom{\frac{1}{2}}\right.
            -3\int\text{d}^4\theta\ 
            \bar{C}Ce^{-K/3}
        \nonumber
        \\
        &\qquad
            +
            \left\{
                \int\text{d}^2\theta\ 
                \left(
                    \frac{1}{4}
                    \sum _ {a}f _ {a}W^{a,\alpha}W^{a} _ {\alpha}
                    +
                    CW^3
                \right)
            +
            \text{h.c.}
            \right\}
        \left.\vphantom{\frac{1}{2}}\right]
        .
    \end{align}
$$
















## Reference

1. <a name="AbeKobayashiOhkiSumita2012"></a>H. Abe, T. Kobayashi, H. Ohki, and K. Sumita, “Superfield description of 10D SYM theory with magnetized extra dimensions,” Nuclear Physics B, vol. 863, no. 1, pp. 1–18, Oct. 2012, [doi: 10.1016/j.nuclphysb.2012.05.012](https://link.aps.org/doi/10.1103/PhysRevD.75.025019).

2. <a name="AbeHigakiKobayashiOmura2007"></a>H. Abe, T. Higaki, T. Kobayashi, and Y. Omura, “Moduli stabilization, F-term uplifting, and soft supersymmetry breaking terms,” Phys. Rev. D, vol. 75, no. 2, p. 025019, Jan. 2007, [doi: 10.1103/PhysRevD.75.025019](https://doi.org/10.1016/j.nuclphysb.2012.05.012).

3. <a name="WessBagger"></a>J. Wess and J. Bagger, *"Supersymmetry and Supergravity."* Princeton, N.J: Princeton University Press, 1992.

[^1]: If there are two $V$s, for instance $\bar{\phi} _ {\bar{i}}(\partial _ {j}V)V$ or $\bar{\phi} _ {\bar{i}}\phi _ {j}V^2$, the term must not have the $D$ for the highest components. The term higher than $V^3$ should vanish by WZ gauge fixing, and no $V$ term also does not have the contribution for the equation of motion.

[^2]: Refer the exercise 2 in Section 7 in the textbook[[2](#WessBagger)].

[^3]: For example, the term not including $\theta^4$ like $\braket{\bar{\phi} _ {\bar{i}}}\phi _ {j}$ vanishes.

[^4]: More accurately, the term $\braket{A _ {i}}\partial _ {j}F _ {k}$ vanishes because of the integration by parts and the fact that $\partial _ {j}\braket{A _ {i}}=0$. The last condition is derived from the Lorentz invariance of the flux.