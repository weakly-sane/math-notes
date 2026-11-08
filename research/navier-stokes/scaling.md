# Scaling of the Navier–Stokes Equations

**Status:** Verified elementary calculation  
**Scope:** Incompressible Navier–Stokes equations on $\mathbb{R}^3$; sufficiently regular solutions for the formal computations below.

## 1. Equations

For a velocity field $u:\mathbb{R}^3\times I\to\mathbb{R}^3$ and pressure $p:\mathbb{R}^3\times I\to\mathbb{R}$,

$$
\begin{cases}
\partial_t u+(u\cdot\nabla)u-\nu\Delta u+\nabla p=0,\\
\nabla\cdot u=0,
\end{cases}
$$

where $\nu>0$ is the viscosity.

## 2. Natural scaling

For $\lambda>0$, define

$$
u_\lambda(x,t)=\lambda u(\lambda x,\lambda^2t),
\qquad
p_\lambda(x,t)=\lambda^2p(\lambda x,\lambda^2t).
$$

The time interval of the rescaled solution is $I_\lambda=\{t:\lambda^2t\in I\}$.

By the chain rule,

$$
\begin{aligned}
\partial_tu_\lambda(x,t)
  &=\lambda^3(\partial_tu)(\lambda x,\lambda^2t),\\
(u_\lambda\cdot\nabla)u_\lambda(x,t)
  &=\lambda^3((u\cdot\nabla)u)(\lambda x,\lambda^2t),\\
\Delta u_\lambda(x,t)
  &=\lambda^3(\Delta u)(\lambda x,\lambda^2t),\\
\nabla p_\lambda(x,t)
  &=\lambda^3(\nabla p)(\lambda x,\lambda^2t).
\end{aligned}
$$

Also, $\nabla\cdot u_\lambda=\lambda^2(\nabla\cdot u)(\lambda x,\lambda^2t)=0$. Thus $(u_\lambda,p_\lambda)$ solves the same equations, with the same viscosity.

## 3. Spatial Lebesgue norms

At any corresponding times $t$ and $\lambda^2t$, change variables $y=\lambda x$ to obtain, for $1\le q<\infty$,

$$
\begin{aligned}
\|u_\lambda(\cdot,t)\|_{L^q(\mathbb{R}^3)}^q
&=\int_{\mathbb{R}^3}|\lambda u(\lambda x,\lambda^2t)|^q\,dx\\
&=\lambda^{q-3}\int_{\mathbb{R}^3}|u(y,\lambda^2t)|^q\,dy.
\end{aligned}
$$

Consequently,

$$
\boxed{\|u_\lambda(\cdot,t)\|_{L^q}
=\lambda^{1-3/q}\|u(\cdot,\lambda^2t)\|_{L^q}.}
$$

The same formula holds for $q=\infty$ if $1-3/q$ is interpreted as $1$. In particular, $L^3(\mathbb{R}^3)$ is **scaling invariant** for the velocity.

## 4. A stationary comparison

For the stationary equations, $u_\lambda(x)=\lambda u(\lambda x)$ and $p_\lambda(x)=\lambda^2p(\lambda x)$.

For a smooth stationary velocity field with $\nabla u\in L^2(\mathbb{R}^3)$,

$$
\int_{\mathbb{R}^3}|\nabla u_\lambda(x)|^2\,dx
=\lambda\int_{\mathbb{R}^3}|\nabla u(y)|^2\,dy.
$$

Thus the Dirichlet integral is **not scaling invariant** in three dimensions.

## Remark

A scale-invariant norm is often called *critical* relative to the natural scaling, but criticality alone does not imply a regularity or Liouville theorem. Such results require additional arguments and precise hypotheses.

## References

This note records standard scaling calculations, not a new research result. Specific background references may be added as reading progresses.
