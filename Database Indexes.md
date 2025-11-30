Un index en bases de datos es una data structure que permite mejorar el tiempo de obtener datos en una tabla.

Clustered-index:
- Ordena la tabla fisicamente, se recomienda usarlo en columna que no cambien constantemente.
- Una tabla solo puede tener un solo clustered index, o sea es unique.
- Normalmente es el primary key de la tabla.
- es mas rapido al momento de obtener información pero no al momento de insertar.

Non-clustered index:
- No afecta como se almacena las rows fisicamente.
- se usa una estructura de datos adicional
- se puede tener multiple indexes en una tabla
- se recomienda en usar en columnas de frecuente acceso en joins y search conditions.
- exact match queries

Como crear un index en SQL
![[Pasted image 20251127094832.png]]

leftmost prefix rule
en un index compuesto, solo funcionara si se inicia con la primera columna declarada en los filtros. El orden importa.

fuente:
[# SQL Indexes (Visually Explained) | Clustered vs Nonclustered](https://www.youtube.com/watch?v=BxAj3bl00-o)
