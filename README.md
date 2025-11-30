# Método de Euler vs solución exacta para una ecuación separable

## Problema
Resolver y comparar la ecuación diferencial separable:


\[
\frac{dy}{dt} = t \cdot y, \quad y(0) = 1
\]


- Solución exacta por separación de variables: \(y(t) = e^{t^2/2}\).
- Aproximación numérica con el método de Euler en el intervalo \(t \in [0, 1]\) con paso \(h = 0.2\).

## Derivación breve
Separando:


\[
\frac{1}{y}dy = t\,dt \Rightarrow \ln|y| = \frac{t^2}{2} + C \Rightarrow y(t) = Ce^{t^2/2}
\]


Con \(y(0)=1\) se obtiene \(C=1\), por lo que \(y(t)=e^{t^2/2}\).

## Método de Euler
La iteración es:


\[
y_{n+1} = y_n + h \cdot f(t_n, y_n), \quad f(t,y) = t \cdot y
\]


Se evalúa en los puntos \(t = 0.0, 0.2, 0.4, 0.6, 0.8, 1.0\).

## Cómo ejecutar
1. Clona el repo o descarga los archivos.
2. Ejecuta:
   ```bash
   python3 main.py
3. Para ver la gráfica, instala:
pip install matplotlib
