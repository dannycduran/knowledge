
podemos crear graficas usando mathplotlib
Aqui hay un ejemplo de como podemos usarlo
```python

from mathplotlib import pyplot as plt
# el primer arg para el eje x y el segundopara el eje y
plt.plot([1,2,4], [6, 8, 9])

# para poder visualizar la grafica tenemos que llamar .show
plt.show()
```

Para graficas que involucre mostrar una evolucion del tiempo en el eje x podemos usar el ejemplo de arriba.

Para poder visualizar una correlacion entre dos variables es mejor usar scatter:
```python
import mathplotlib.pyplot as plt

plt.scatter(x, y)
plt.show()

```

para explorar explorar el dataset y poder una idea de la distribucion poder usar histogram:
```python
# bins are the number the categories to divide the dataset, by default 10
plt.hist(dataset, bins=5)
plt.show()

```

# Customization

para cambiar el nombre los ejes:
```python
plt.xlabel('hello world')
plt.ylabel('yyy')
```

para cambiar se visualiza en los ejes:
```python
plt.yticks(values, name_of_points)
```

para cambiar el tamaño de los puntos podemos usar:
```python
plt.scatter(gdp_cap, life_exp, s = np_pop)
```

para agregar el color de los puntos podemos usar c y alpha
```python
plt.scatter(x = gdp_cap, y = life_exp, s = np.array(pop) * 2, c = col, alpha=0.8)
```