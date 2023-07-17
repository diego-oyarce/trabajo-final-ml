# Prueba de ciencia de datos de Empresa SoftWorld

# Antecedentes Generales

SoftWorld tiene operaciones en varias ciudades y países, entregando miles de pedidos todos los días. Para entregar estos pedidos a tiempo, dependemos de buenas estimaciones de cuánto tiempo necesita el comprador para completar el pedido.

En esta prueba técnica, creará un modelo de aprendizaje automático para realizar estas estimaciones. Dado que construimos internamente nuestras soluciones de aprendizaje automático con python, le pedimos que haga lo mismo en esta prueba técnica. Sin embargo, puede utilizar las bibliotecas con las que se sienta más cómodo.

# Entrega y grupos

Los grupos para este trabajo deben ser de 4 personas cada uno (2 personas por grupo deben presentar,  uds internamente lo eligen), en total son 21 alumnos asi que si hay un grupo de 5 personas no hay problema

*Los códigos propuestos tienen un 70% de la evaluación final y la presentación un 30% restante* 

El trabajo final corresponde a un 50% de la evaluación final.

***El formato de entrega es el habitual de Jupyter Notebook, Todas las celdas deben ser ejecutadas*** 

Sé Descontará un punto a cada grupo cor cada día de atraso en la entrega.

**El Plazo de entrega de este trabajo es el 17 de Julio (las presentaciones PPT de cada grupo se realizaran 20 de Julio en el horario habitual de clases**

## Datos

En este repositorio, hemos incluido datos que representan el pedido, el comprador y la sucursal de la tienda.

### Descripción del archivo y campos de datos

***pedir_productos.csv:***

- order_id: ID del pedido
- product_id: ID del producto
- cantidad: La cantidad pedida de este producto
- buy_unit: La unidad del producto (KG/UN)

***pedidos.csv:***

- order_id: ID del pedido
- lat: La latitud del lugar de entrega
-lng: La longitud de la ubicación de entrega
- prometido_tiempo: El tiempo de entrega prometido al usuario
- on_demand: si es verdadero, se prometió que el pedido se entregaría en menos de X minutos
- shopper_id: ID que representa al shopper que completó el pedido.
- store_branch_id: ID de la sucursal de la tienda
- total_minutes: el total de minutos que tomó completar el pedido (etiqueta)

***comprador.csv***

- shopper_id: ID del comprador
- antigüedad: El nivel de experiencia del comprador.
- tasa_encontrada: Porcentaje de productos encontrados por histórico de compradores.
- picking_speed: Histórico de velocidad de picking, productos por minutos.
- tasa_aceptada: Porcentaje de pedidos históricamente aceptados por el comprador
- calificación: calificación del cliente del comprador

***sucursal.csv:***

- store_branch_id: ID de la sucursal de la tienda
- tienda: ID que representa la tienda
-lat: Latitud de la ubicación de la sucursal
-lng: Longitud de la ubicación de la sucursal

*Todos los datos han sido anonimizados*

### Objetivo de la investigación

El objetivo es predecir los `total_minutes` que tarda en completarse un pedido, donde las filas que no contienen un valor de `total_minutes` deben reservarse como parte del archivo de envío, que contiene el `order_id` con los valores predichos.

Como estamos interesados en ver cómo abordó el problema, también le pedimos que incluya su código junto con el archivo de envío. 

El código debe estar bien documentado, explicando las decisiones tomadas. Con estas explicaciones, veremos todo, desde cómo se procesaron los datos, las características utilizadas hasta el modelo completo y las predicciones.

### Presentación PPT

Se necesita que cada grupo realice una presentación mediante formato PPT entre 6 y 10 slides con los aspectos relevantes tales como (no más de 30 minutos por presentación):

1. Objetivo de la investigación
2. Problema detectado
3. Fases del modelamiento predictivo
4. Propuesta de mejor modelo y justificación
5. Recomendaciones

[https://www.notion.so/Prueba-de-ciencia-de-datos-de-Empresa-SoftWorld-0a41e5a2496b493599230a283e81c4b2](https://www.notion.so/Prueba-de-ciencia-de-datos-de-Empresa-SoftWorld-0a41e5a2496b493599230a283e81c4b2?pvs=21)
