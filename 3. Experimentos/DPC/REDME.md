# DFIG DPC using MPC-WM 

*27/03/2024*

## Análise do comportamento do DFIG com controle DPC utilizando Modulador quando submetido a variação dos horizontes e dos ajustes das matrizes de peso

### Modelo em Espaço de Estados da dinâmica do rotor

$$
\begin{bmatrix}
Q_s(k+1)\\ 
P_s(k+1)
\end{bmatrix}=
\begin{bmatrix}
1 & \omega_{sl}T \\
-\omega_{sl}T & 1 
\end{bmatrix}
\begin{bmatrix}
Q_s(k) \\
P_s(k)
\end{bmatrix}+
\begin{bmatrix}
\frac{T}{A_m} & 0 \\
0 & \frac{T}{A_m} 
\end{bmatrix}
\begin{bmatrix}
v_{r,d}(k) \\
v_{r,q}(k)
\end{bmatrix}+
\begin{bmatrix}
1 & 0 \\
0 & 1 
\end{bmatrix}
\begin{bmatrix}0 \\
\frac{-\omega_{sl}L_rT}{L_m A_m}\lambda_s(k)
\end{bmatrix}
$$

### Variação dos Horizontes

Para uma primera análise serão estudados a variação dos horizontes ($n_y, n_u$) para os seguintes intervalos:

$n_y = 1:20$

$n_u = 1:10$



### Variação dos Ajustes das Matrizes de Ganho

<center>
<figure>
  <img src="https://github.com/cotabr/Mestrado/blob/299be38beff96f7d1a35d659046d43e1ab340fb7/3.%20Experimentos/DPC/Imagens/THD%20(200%20-%20VH).png" width="300" height="auto"  />
  <figcaption>An elephant at sunset</figcaption>
</figure>
</center>


