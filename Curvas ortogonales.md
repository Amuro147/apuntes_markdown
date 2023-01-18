Las [[funciones armónicas conjugadas]], son Curvas Ortogonales, es decir que se cortan ó intersectan perpendicularmente. Para demostrar esta propiedad se utilizan ECR. Sean u y v dos funciones armónicas conjugadas, si igualamos a una constante cada una de ellas, encontraremos las correspondientes curvas de nivel:
$$u(x,y)=c \qquad v(x,y)=k$$
Diferenciando, se puede despejar $\frac {dy}{dx}$, que representa la pendiente de la recta tangente en cada curva:
$$du=\frac{\partial u}{\partial x}+\frac{\partial u\ dy}{\partial y\ dx}=0 \to \frac{dy}{dx}=-\frac{\partial u/\partial x}{\partial u/\partial y}$$
$$dv=\frac{\partial v}{\partial x}+\frac{\partial v\ dy}{\partial y\ dx}=0 \to \frac{dy}{dx}=-\frac{\partial v/\partial x}{\partial v/\partial y}$$
Si se aplica [[ecuaciones de cauchy-riemann|ECR]] a $dv$:
$$\frac{dy}{dx}=-\frac{\partial v/\partial x}{\partial v/\partial y}=\frac{\partial u/\partial y}{\partial u/\partial x}$$
Las expresiones representan las pendientes de las rectas tangentes a las funciones $u$ y $v$, respectivamente, haciendo el producto comprobamos que son perpendiculares:
$$\left(-\frac{\partial u/\partial x}{\partial u/\partial y}\right)\left(-\frac{\partial v/\partial x}{\partial v/\partial y}\right)=\left(\frac{\partial v/\partial y}{\partial v/\partial x}\right)\left(-\frac{\partial v/\partial x}{\partial v/\partial y}\right)=-1$$