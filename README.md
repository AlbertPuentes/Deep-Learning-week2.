## Análisis de los Parámetros ejemplo credito bancario

La implementación de este perceptrón revela cómo los parámetros matemáticos se traducen directamente con ejemplo credito bancario:

1. El Puntaje z como "Credit Score": El valor z (z = w_1x_1 + w_2x_2 + b$) representa la calificación interna del cliente. Si z \ge 0, el cliente es sujeto de crédito. Observamos que el Cliente D obtuvo el puntaje máximo (z = 1.5$), siendo el perfil más seguro.
2. El Sesgo (Bias) como Aversión al Riesgo:** El sesgo ($-0.5$) representa la postura inicial del banco frente al riesgo. Un bias negativo significa que la respuesta por defecto del banco es "No" (0), a menos que el cliente presente evidencia positiva. Si el banco entrara en crisis y quisiera ser más estricto (exigiendo **ambas** condiciones, como una compuerta AND), bastaría con cambiar el bias a `-1.5`, aumentando la barrera de entrada sin tocar el código lógico.
3. Los Pesos como Ponderación de Factores:** En este ejemplo, w_1$ y $w_2$ valen `1.0`. Si el banco decidiera que el historial crediticio es el doble de importante que los ingresos, ajustaríamos los pesos a `[2.0, 1.0]`. La red neuronal nos permite modelar prioridades económicas exactas.
