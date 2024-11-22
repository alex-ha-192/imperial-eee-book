# Complex numbers
Complex numbers are numbers that do not have to be real. This can be useful in solving quadratic equations, and especially with regards to engineering, where they can be used in wave equations and the like.
## Imaginary numbers
Numbers of the form \\( a \sqrt{-1} \\) can be represented using the construction \\( i = \sqrt{-1} \\).

\\( i \\) is an **imaginary number**, as opposed to the real numbers (\\( 1, 5, -10, \sqrt{2}, \frac{\pi}{4} \\) etc.). The set of imaginary numbers is much like the set of real numbers, except with the base unit switched from units of 1 to units of \\( i \\). For example, the imaginary numbers include \\( i, -i, 2.5i, e^2 i, \sqrt{43}i \\) and so on.

Imaginary numbers follow all the usual rules of arithmetic.

## Complex numbers
The set of complex numbers is the set of all numbers of the form \\( x+iy \\). The set of numbers such that \\( x = 0 \\) is the set of imaginary numbers, and the set of numbers such that \\( y = 0 \\) is the set of real numbers. Therefore, all purely real and purely imaginary numbers can also be considered complex.

## Argand diagrams
We can use a number line to show the relationships between real numbers graphically. When we also need to consider a second category (the set of imaginary numbers), we add another axis to the number line to create a 2D graph. Because this graph contains axes in terms of the real and imaginary units, we can show any complex number on this graph.

We call this graph an Argand diagram. In order to display a number on an Argand diagram, we can either plot numbers in Cartesian form (e.g. plot \\( 2 - i \\) as 2 units along the positive real axis and 1 unit along the negative imaginary axis) or in modulus-argument (mod-arg) form. In mod-arg form, we plot numbers by the angle they make anti-clockwise with the positive real axis (to find the line the number lies on) and the number's distance from the origin (to find where on this line the number lies).

The angle a number makes with the positive real axis (its argument) is measured in radians and fits within the range \\( 0 \le  \theta < 2\pi \\) or within the range \\( -\pi < \theta \le \pi \\). By convention, we will use the latter. Note that we find negative arguments by going clockwise from the positive real axis instead of by going anti-clockwise.

We can either add complex numbers by summing their real and imaginary components, or by treating the line between the origin and each number as a vector and summing these.

When multiplying complex numbers together, note that the \\( i^2 \\) term is equal to \\( -1 \\) by definition.

For some complex number \\( z \\), \\( |z| \\) is the magnitude of \\( z \\) or (assuming that \\( z = x + iy \\)) \\( |z| = \sqrt{x^2+y^2} \\). We can show that for two complex numbers \\( z, w \\): \\( |zw| = |z||w| \\), \\( \overline{zw}=\bar{z}\bar{w} \\), \\( \overline{z+w}=\bar{z}+\bar{w} \\).

## Complex exponential form
From the Maclaurin series (see [Derivatives](derivatives.md)) of \\( e^x \\), we can find that \\( e^{ix} = \cos x + i \sin x \\).

We can use this to show that \\( \cos (a+b) = \cos a \cos b - \sin a \sin b \\) and \\( \sin (a+b) = \sin a \cos b + \cos a \sin b \\) by taking \\( e^{ai}e^{ib} = e^{i(a+b)} \\), applying Euler's formula, and equating real and imaginary parts.

We can also show that for some \\( z = x + iy \\), \\( e^z = e^x(\cos y + i \sin y) \\), and (by taking \\( r \\) as the magnitude of \\( z \\)), find that \\( z = re^{i\theta} \\) for any \\( z \\), as long as we use the correct \\( r \\) (magnitude) and \\( \theta \\) (argument). 

We now know that changing the argument \\( \theta \\) of a complex number \\( z = re^{i\theta} \\) only changes the angle with the origin, not the magnitude. Therefore, any complex number in the form \\( re^{i\theta} \\) lies on the circle centred at the origin with radius \\( r \\).

We can use this knowledge to determine the value of some important complex numbers. For example, \\( e^{i\pi} \\) is the number 1 unit away from the origin and makes an angle \\( \pi \\) radians or 180 degrees with the positive real axis, that is, the number lies on the negative real axis. As we know, a number 1 unit away from the origin on the negative real axis is simply -1. Therefore, \\( e^{i\pi} = -1 \\).

If we replace \\( \theta \\) with \\( -\theta \\) in Euler's formula, we find that \\( e^{-i\theta} = \cos \theta - i \sin \theta \\). Adding this with \\( e^{i\theta} \\) and rearranging, we can find that \\( \cos \theta = \frac{ e^{i\theta} + e^{-i\theta}}{2} \\) and that \\( \sin \theta = \frac{e^{i\theta}-e^{-i\theta}}{2i} \\). These results can be used to switch between terms of \\( \cos (n\theta) \\) and \\( \cos^n(\theta) \\).

The complex exponential form can be used in the analysis and design of circuits to model a phasor.

## De Moivre's Theorem