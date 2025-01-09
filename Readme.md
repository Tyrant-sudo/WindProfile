# Log wind profile
The equation to estimate the mean wind speed ($u_z$) at height $z$ (meters) above the ground is:

$$u_z = \frac{u_*}{\kappa} \left[ \ln \left( \frac{z - d}{z_0} \right) + \psi(z, z_0, L) \right]$$

where $u_*$ is the *friction velocity* (m s$^{-1}$), $\kappa$ is the *Von Kármán constant* (~0.41), $d$ is the *zero plane displacement* (in meters), $z_0$ is the *surface roughness* (in meters), and $\psi$ is a *stability term* where $L$ is the *Obukhov length* from *Monin-Obukhov similarity theory*. Under *neutral stability* conditions, $z/L = 0$ and $\psi$ drops out and the equation is simplified to:

$$u_z = \frac{u_*}{\kappa} \ln \left( \frac{z - d}{z_0} \right).$$

$d$ is the height in meters above the ground at which zero mean wind speed is achieved as a result of flow obstacles such as trees or buildings. This displacement can be approximated as $2/3$ to $3/4$ of the average height of the obstacles. For example, if estimating winds over a forest canopy of height 30 m, the zero-plane displacement could be estimated as $d = 20$ m.


$z_0$ is a corrective measure to account for the effect of the roughness of a surface on wind flow. That is, the value of the roughness length depends on the terrain. The exact value is subjective and references indicate a range of values, making it difficult to give definitive values. In most cases, references present a tabular format with the value of $z_0$ given for certain terrain descriptions. For example:
- For very flat terrain (snow, desert), the roughness length may be in the range $0.001$ to $0.005$ m.
- For open terrain (grassland), the typical range is $0.01$ to $0.05$ m.
- For cropland, and brush/forest, the ranges are $0.1$ to $0.25$ m and $0.5$ to $1.0$ m, respectively.
- When estimating wind loads on structures, the terrains may be described as suburban or dense urban, for which the ranges are typically $0.1$ to $0.5$ m and $1.0$ to $5.0$ m, respectively.
In order to estimate the mean wind speed at one height ($z_2$) based on that at another ($z_1$), the formula would be rearranged:

$$u(z_2) = u(z_1) \frac{\ln \left( \frac{z_2 - d}{z_0} \right)}{\ln \left( \frac{z_1 - d}{z_0} \right)},$$

where $u(z_1)$ is the mean wind speed at height $z_1$.