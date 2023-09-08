# Practicajs.
import random
#  la posición inicial
posicion_inicial = random.randint(0, 359)
#las vueltas al círculo
vueltas = random.randint(5, 10)
# Calcular el ángulo final
angulo_final = (posicion_inicial + vueltas * 360) % 360
print(f"Posición o ángulo Inicial G.A.: {posicion_inicial}")
print(f"Valor Aleatorio Generado en Grados: {vueltas * 360}")
print(f"Ángulo Final: {angulo_final}")
