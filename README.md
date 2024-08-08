# Sistema de Reservas de Habitaciones de Hotel

Este proyecto es una aplicación de consola en C# para gestionar un sistema de reservas de habitaciones en un hotel, utilizando el concepto de herencia en Programación Orientada a Objetos (POO). La aplicación permite la gestión de diferentes tipos de habitaciones y la asignación de habitaciones a clientes.

## Características

La aplicación permite gestionar los siguientes tipos de habitaciones:
- Habitación Simple
- Habitación Doble
- Suite
- Habitación Deluxe

Cada tipo de habitación tiene atributos y métodos específicos, y hereda de una clase base `Habitacion`.

### Atributos Comunes

- `Numero` (int): Número de la habitación.
- `PrecioPorNoche` (double): Precio por noche de la habitación.
- `Disponible` (bool): Indica si la habitación está disponible.
- `ClienteAsignado` (string): Nombre del cliente asignado a la habitación (si está ocupada).

### Métodos Comunes

- `MostrarInformacion()`: Método virtual que muestra la información básica de la habitación.
- `CambiarDisponibilidad(bool disponible)`: Método que cambia el estado de disponibilidad de la habitación.
- `AsignarCliente(string nombreCliente)`: Método que asigna un cliente a la habitación.
- `LiberarHabitacion()`: Método que libera la habitación y quita el cliente asignado.

### Atributos Específicos

- **Habitación Simple**: `NumeroDeCamas` (int)
- **Habitación Doble**: `VistaAlMar` (bool)
- **Suite**: `NumeroDeHabitaciones` (int), `TieneJacuzzi` (bool)
- **Habitación Deluxe**: `ServiciosExtras` (string)

## Funcionalidades del Menú

1. **Agregar Habitación**: Permite agregar una nueva habitación a la lista.
2. **Eliminar Habitación**: Permite eliminar una habitación existente de la lista.
3. **Mostrar Habitaciones**: Muestra la información de todas las habitaciones en la lista.
4. **Asignar Habitación a Cliente**: Asigna una habitación disponible a un cliente.
5. **Liberar Habitación**: Libera una habitación ocupada.

## Ejemplo de Uso

1. El usuario selecciona "Agregar Habitación" y elige "Suite".
2. El programa solicita el número de la habitación, el precio por noche, el número de habitaciones y si tiene jacuzzi.
3. La suite se agrega a la lista de habitaciones.
4. El usuario selecciona "Asignar Habitación a Cliente", ingresa el número de la habitación y el nombre del cliente.
5. El programa asigna la habitación al cliente y cambia la disponibilidad.
6. El usuario selecciona "Mostrar Habitaciones" y el programa muestra la información de todas las habitaciones en la lista, incluyendo el nombre del cliente asignado si la habitación está ocupada.
### Nota sobre las funciones del menú

Al iniciar la aplicacion utilizar primero el apartado de agregar habitación para que el resto de apartados funcionen de la manera esperada.

## Cómo Ejecutar

1. Clona el repositorio.
2. Abre una terminal en el directorio del proyecto.
3. Ejecuta el comando `dotnet run` para iniciar la aplicación.

