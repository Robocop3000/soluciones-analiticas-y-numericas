# soluciones-analiticas-y-numericas
soluciones analiticas y numericas
Aquí está el contenido del archivo README en texto plano, sin formato Markdown, tablas ni caracteres especiales, manteniendo la estructura lógica.

COMPARACION SOLUCION EXACTA VS METODO DE EULER

Este repositorio contiene un script de Python (main.py o ecuacion_euler.py) que resuelve una Ecuacion Diferencial Ordinaria (EDO) separable utilizando dos metodos la solucion analitica exacta (Separacion de Variables) y la solucion numerica aproximada (Metodo de Euler).

El objetivo es comparar la precision de la aproximacion de Euler frente al valor real de la solucion en un intervalo dado.

ECUACION DIFERENCIAL ORDINARIA EDO

La EDO seleccionada para este ejercicio es el modelo de crecimiento exponencial simple:

dy dt = 2y

Condicion Inicial: y(0) = 1

Solucion Analitica Exacta Mediante la separacion de variables e integracion, la solucion exacta es: y(t) = e elevado a la 2t

EJECUCION Y PARAMETROS

Requisitos Para ejecutar el script, solo se necesita tener Python instalado junto con las siguientes librerias: numpy matplotlib

Puedes instalar las dependencias con el siguiente comando: pip install numpy matplotlib

Parametros de la Simulacion

Parametro | Valor | Descripcion Intervalo | t pertenece a 0, 1 | El rango de tiempo para la simulacion. Paso (h) | 0.2 | El tamano del paso utilizado por el Metodo de Euler. Condicion Inicial | y0 = 1 | El valor inicial de la funcion y(t) en t=0.

Ejecucion Ejecuta el script de Python directamente: python nombre_del_archivo.py (Asume que nombraste el archivo como quieras, por ejemplo, simulacion_edo.py)

RESULTADOS Y CONCLUSION

Reporte de la Simulacion

El script mostrara una tabla similar a esta, donde el error absoluto se calcula como y_Exacta - y_Euler en valor absoluto:

t | y_Euler | y_Exacta | Error Abs. 0.0 | 1.0000 | 1.0000 | 0.0000 0.2 | 1.2000 | 1.4918 | 0.2918 0.4 | 1.4400 | 2.2255 | 0.7855 0.6 | 1.7280 | 3.3201 | 1.5921 0.8 | 2.0736 | 4.9530 | 2.8794 1.0 | 2.4883 | 7.3891 | 4.9008

Conclusion

Debido a que el Metodo de Euler es un metodo de primer orden y la solucion exacta (e elevado a la 2t) crece exponencialmente, el error de truncamiento se acumula y magnifica rapidamente a medida que avanza el tiempo.
