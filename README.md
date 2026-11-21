# Mesero Virtual – Prueba de Concepto de Machine Learning

## 1. Descripción del proyecto

Este proyecto presenta una prueba de concepto de Machine Learning aplicada al sistema **Mesero Virtual**, cuyo propósito es estimar los tiempos de preparación de productos gastronómicos mediante un modelo de aprendizaje automático.

El modelo analiza diferentes variables, como el producto solicitado, el día de la semana, la hora del pedido, la cantidad de productos, los pedidos pendientes, el nivel de ocupación y el personal disponible en cocina.

Con esta información genera una estimación del tiempo de preparación, contribuyendo a mejorar la planificación y gestión de los pedidos en establecimientos gastronómicos.

## 2. Objetivo

Implementar y evaluar un modelo de Machine Learning capaz de predecir el tiempo estimado de preparación de productos gastronómicos, como propuesta de mejora tecnológica para el proyecto Mesero Virtual.

## 3. Tecnologías utilizadas

- **Python:** lenguaje de programación.
- **Google Colab:** entorno de desarrollo y ejecución.
- **Pandas:** manipulación y análisis de datos.
- **NumPy:** operaciones numéricas.
- **Scikit-learn:** entrenamiento y evaluación del modelo.
- **Random Forest Regressor:** algoritmo de aprendizaje automático.
- **Joblib:** almacenamiento del modelo entrenado.

## 4. Descripción del modelo

Se implementó un modelo de aprendizaje supervisado mediante el algoritmo Random Forest Regressor, orientado a resolver un problema de regresión.

El modelo utiliza un conjunto de datos de 400 registros simulados para aprender la relación entre las condiciones de operación de la cocina y el tiempo de preparación de los productos.

### Variables utilizadas

| Variable | Descripción |
|---|---|
| Producto | Nombre del producto gastronómico |
| Categoría | Tipo de comida |
| Día de la semana | Día en que se realiza el pedido |
| Hora del pedido | Hora de ingreso del pedido |
| Cantidad | Número de unidades solicitadas |
| Pedidos pendientes | Pedidos en espera |
| Nivel de ocupación | Baja, media o alta |
| Personal de cocina | Número de personas disponibles |
| Tiempo de preparación | Tiempo estimado en minutos (variable objetivo) |

## 5. Resultados de evaluación

El modelo fue evaluado mediante las métricas MAE y R².

- **MAE:** 2.44 minutos.
- **R²:** 0.91.

Estos resultados corresponden a la evaluación realizada sobre los datos de prueba del conjunto simulado.

## 6. Pruebas de predicción

Se realizaron pruebas con diferentes condiciones de operación para comprobar el funcionamiento del modelo.

| Escenario | Tiempo estimado |
|---|---:|
| Sábado, 20:00, ocupación alta, 10 pedidos pendientes y 2 personas en cocina | 21.21 minutos |
| Lunes, 10:00, ocupación baja, 1 pedido pendiente y 3 personas en cocina | 16.52 minutos |

También se implementó un formulario interactivo en Python que permite ingresar manualmente las características de un pedido y obtener una predicción.

## 7. Estructura del repositorio

- `prueba_concepto_machine_learning_mesero_virtual.ipynb`: cuaderno de Google Colab con el desarrollo, entrenamiento, evaluación y pruebas del modelo.
- `base_datos_machine_learning_mesero_virtual.csv`: conjunto de datos utilizado para entrenar y evaluar el modelo.
- `modelo_mesero_virtual.joblib`: archivo del modelo entrenado y su preprocesamiento.

## 8. Limitaciones y mejoras futuras

Los datos utilizados son simulados y no representan mediciones reales de restaurantes. Por esta razón, los resultados corresponden a una demostración académica del funcionamiento de Machine Learning.

Como mejoras futuras se propone:

- Recopilar datos reales de preparación de productos.
- Ampliar y actualizar periódicamente el conjunto de datos.
- Comparar diferentes algoritmos de Machine Learning.
- Integrar el modelo con el backend y frontend de Mesero Virtual.
- Generar estimaciones basadas en las condiciones reales de cada restaurante.

## 9. Autoría y contexto académico

Proyecto: **Mesero Virtual**

Desarrollo: Prueba de concepto de Machine Learning para la predicción de tiempos de preparación de productos gastronómicos.

Formación: Tecnólogo en Análisis y Desarrollo de Software – SENA.

## 10. Conclusión

Esta prueba de concepto demuestra cómo el Machine Learning puede incorporarse como una herramienta de apoyo al sistema Mesero Virtual, permitiendo estimar tiempos de preparación según las características de los pedidos y las condiciones de operación de la cocina.

El desarrollo constituye una primera aproximación para implementar funcionalidades inteligentes que contribuyan a optimizar la gestión de pedidos en establecimientos gastronómicos.
