## Campos vectoriales

### Funciones analiticas
![[Funciones analiticas]]

### Funciones enteras
Una funcion que es analitica en todo punto z del plano complejo se dice que es una **funcion entera**.
**Puntos singulares**: Un punto $z$ en el que una funcion compleja $w=f(z)$ no es analitica se llama **punto singular** de $f$.

### Ecuaciones de Cauchy-Riemann

> Supongamos que $f(z)=u(x,y)+iv(x,y)$ es derivable en un punto $z=x+iy$. Entonces en $z$ las derivadas parciales de primer orden de $u$ y $v$ existen y satisfacen las **ecuaciones de Cauchy-Riemann**.$$\frac{\partial u}{\partial x}=\frac{\partial v}{\partial y}\ \ \ \ \text{y} \ \ \ \ \frac{\partial u}{\partial y}=-\frac{\partial v}{\partial x} $$

##### **Demostracion**
La derivada de $f$ en $z$ esta dada por:
$$f'(z)=\lim_{\Delta z \to 0} \frac {f(z+\Delta z)-f(z)}{\Delta z}$$
Al escribir $f(z)=u(x,y)+iv(x,y)$ y $\Delta z = \Delta x + i\Delta y$, la ecuacion anterior se convierte en:
$$
f^{\prime}(z)=\lim _{\Delta z \rightarrow 0} \frac{u(x+\Delta x, y+\Delta y)+i v(x+\Delta x, y+\Delta y)-u(x, y)-i v(x, y)}{\Delta x+i \Delta y}
$$
Ya que se supone que existe el limite, $\Delta z$ puede aproximarse a cero desde cualquier direccion conveniente. En particularm si elegimos hacer que $\Delta z \to 0$ a lo largo de una recta horizontal, entonces $\Delta y =0$ y $\Delta z = \Delta x$. Entonces podemos escribir a la ecuacion anterior como:
$$
\begin{aligned}
f^{\prime}(z) & =\lim _{\Delta x \rightarrow 0} \frac{u(x+\Delta x, y)-u(x, y)+i[v(x+\Delta x, y)-v(x, y)]}{\Delta x} \\
& =\lim _{\Delta x \rightarrow 0} \frac{u(x+\Delta x, y)-u(x, y)}{\Delta x}+i \lim _{\Delta x \rightarrow 0} \frac{v(x+\Delta x, y)-v(x, y)}{\Delta x}
\end{aligned}
$$
La existencia de $f'(z)$ implica que cada limite existe. Estos limites son definiciones de las derivadas parciales de primer orden respecto a $x$ de $u$ y de $v$, respectivamente. Se han demostrado dos cosas: que $\frac {\partial u}{\partial x}$ y $\frac{\partial v}{\partial x}$ existen en el punto $z$, y que la derivada de $f$ es:
$$f'(z)=\frac{\partial u}{\partial x} + i \frac{\partial v}{\partial x}$$
Ahora hacemos que $\Delta z \to 0$ a lo largo de una recta vertical. Con $\Delta x = 0$ y $\Delta z = i\Delta y$, los limites se convierte en:
$$
\begin{aligned}
f^{\prime}(z)&=\lim _{\Delta y \rightarrow 0} \frac{u(x, y+\Delta y)-u(x, y)}{i\Delta y}+i \lim _{\Delta y \rightarrow 0} \frac{v(x, y+\Delta y)-v(x, y)}{i\Delta y}
\end{aligned}
$$
En este caso se demuestra que $\frac{\partial u}{\partial y}$ y $\frac{\partial v}{\partial y}$ existen en $z$ y que:
$$f'(z) = -i\frac{\partial u}{\partial y}+\frac{\partial v}{\partial y}$$
Igualando las partes real e imaginaria de las derivadas, se obtiene el sistema de ecuaciones mostrado al principio del tema.

##### Criterio para la analiticidad
Supongamos que las funciones reales $u(x,y)$ y $v(x,y)$ son continuas y tiene derivadas parciales de primer orden continuas en un dominio $D$. Si $u \text{ y } v$ satisfacen las ecuaciones de Cauchy-Riemann en todos los puntos de $D$, entonces la funcion compleja $f(z)=u(x, y) + iv(x, y)$ es analitica  en $D$.

### Conclusion
**Si las funciones $u(x,y), v(x,y)$ y sus cuatro derivadas parciales de primer orden son continuas en determinada región o dominio del Plano Complejo y satisfacen las Condiciones de Cauchy–Riemann, estas condiciones son necesarias y suficientes para asegurar la derivabilidad de la función: $f(x,y) = u(x,y) + i v(x,y)$ , en dicha región del Plano Complejo.**
De esta manera las ECR no solamente determinan si la funcion es derivable sino tambien indican en que region del plano existe la derivada. Cuando hablamos de region/dominio, puede ser todo el plano o solamente parte de el. Las ECR forman un sistema, es decir, deben cumplirse ambas simultaneamente.

### Funciones armonicas
Una funcion de valores reales $\phi$ de dos variables reales $x$ e $y$ que tiene primeras y segundas derivadas parciales continuas en un dominio $D$, y satisface la ecuacion de Laplace, se dice que es **armonica** en $D$.
Suponga que la funcion compleja $f(z)=u(x,y)+iv(x,y)$ es analitica en un dominio $D$. Entonces las funciones $u(x,y)$ y $v(x,y)$ son armonicas en $D$.

#### Funciones armonicas conjugadas
![[funciones armónicas conjugadas]]