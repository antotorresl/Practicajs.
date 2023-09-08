# Practicajs.
function simularTiradaRuleta() {
    // Generar un número aleatorio entre 5 y 10 para las vueltas
    const vueltas = Math.floor(Math.random() * (10 - 5 + 1)) + 5;
  
    // Inicializar la posición en 0
    let posicion = 0;
  
    // Realizar las vueltas
    for (let i = 0; i < vueltas; i++) {
      // Generar un número aleatorio entre 0 y 36
      const numero = Math.floor(Math.random() * 37);
      // Actualizar la posición
      posicion = (posicion + numero) % 37;
    }
  
    return posicion;
  }
  
  // Simular 10 tiradas
  for (let juego = 1; juego <= 10; juego++) {
    const resultado = simularTiradaRuleta();
    console.log(`Nro de Juego: ${juego}`);
    console.log(`Valor Aleatorio Generado: ${resultado}`);
    console.log(`Nro que cayó en la ruleta: ${resultado}`);
    console.log();
  }
