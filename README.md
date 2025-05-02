MODELO DE PREDICCIÓN DE IMÁGENES 
Para este proyecto se utilizó el dataset de Moda (similar a MNIST), el cual es un conjunto de 70,000 imágnes 
de ropa etiquetadas, cada una de tamaño de 28x28 píxeles.
El dataset está compuesto por 60,000 imágenes de prueba en escala de grises, cada una asociada a
una de las 10 etiquetas.
El escalado de grises corresponde a un número entero entre 0 y 255.
Las etiquetas del dataset son:
0 Camiseta/top
1 pantalón
2 jerseys
3 Vestido
4 capas
5 Sandalia
6 Camisa
7 zapatillas
8 Bolsa
9 Botín

Para la elaboración del modelo se procedió similarmente al dataset MNIST: primero se normalizaron
los datos, posteriormente se separó en datos de entrenamiento (los 60,000) para de ahí ir a la 
creación del modelo, por medio de keras con la función sequential, además de usar "Adam" como
optimizador.

Para entrenar al modelo se utilizaorn 5 épocas, además de graficar la función de pérdida para 
observar que efectivamente esas 5 épocas coincidieran con la frontera, como se observó en clase.

Finalmente se elaboró la impresión de las predicciones mediante un array, el cual mostraba 25
imágenes de prueba, acertando en 22 de los 25 casos, lo que corresponde a un 88% de acierto, lo 
cual nos indica la buena eficiencia del modelo.
