# Practicajs.
// Obtener la hora actual
const horaActual = new Date();
const horaActualEnMilisegundos = horaActual.getTime();

// Generar un número aleatorio de minutos entre 300 (5 horas) y 600 (10 horas)
const minutosAleatorios = Math.floor(Math.random() * (600 - 300 + 1)) + 300;

// Calcular la hora final en milisegundos sumando los minutos aleatorios
const horaFinalEnMilisegundos = horaActualEnMilisegundos + minutosAleatorios * 60000;

// Crear objetos de fecha para la hora final
const horaFinal = new Date(horaFinalEnMilisegundos);

// Formatear las horas y minutos para mostrarlos con dos dígitos
const formatoDosDigitos = (numero) => {
  return numero.toString().padStart(2, '0');
};

// Obtener las horas y minutos en formato HH:mm
const horaActualFormateada = `${formatoDosDigitos(horaActual.getHours())}:${formatoDosDigitos(horaActual.getMinutes())}`;
const horaFinalFormateada = `${formatoDosDigitos(horaFinal.getHours())}:${formatoDosDigitos(horaFinal.getMinutes())}`;

// Imprimir los resultados
console.log(`Hora Actual: ${horaActualFormateada}`);
console.log(`Valor Aleatorio Generado en Minutos: ${minutosAleatorios}`);
console.log(`Hora Final: ${horaFinalFormateada}`);
Este código hace lo siguiente:

Obtiene la hora actual usando new Date() y convierte esa hora en milisegundos.

Genera un número aleatorio de minutos entre 300 (5 horas) y 600 (10 horas) utilizando Math.random().

Calcula la hora final en milisegundos sumando los minutos aleatorios a la hora actual.

Crea objetos de fecha para la hora final.

Formatea las horas y minutos para que se muestren con dos dígitos utilizando la función formatoDosDigitos().

Imprime la hora actual, el valor aleatorio en minutos y la hora final en el formato deseado.





