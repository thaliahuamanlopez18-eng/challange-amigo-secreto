# challenge-amigo-secreto
// Lista (array) para guardar las tareas
let tareas = [];

// Función para agregar una tarea
function agregarTarea(nombreTarea) {
  if (nombreTarea) { // condicional: revisa si no está vacío
    tareas.push(nombreTarea); // agrega la tarea al array
    console.log(`Tarea "${nombreTarea}" agregada con éxito `);
  } else {
    console.log(" No puedes agregar una tarea vacía");
  }
}

// Función para mostrar todas las tareas
function mostrarTareas() {
  if (tareas.length === 0) {
    console.log("No tienes tareas pendientes ");
  } else {
    console.log("Tus tareas son:");
    // Bucle para recorrer la lista
    for (let i = 0; i < tareas.length; i++) {
      console.log(`${i + 1}. ${tareas[i]}`);
    }
  }
}

// Ejemplo de uso
agregarTarea("Estudiar JavaScript");
agregarTarea("Practicar ejercicios de lógica");
agregarTarea("Preparar presentación de la universidad");

mostrarTareas();
