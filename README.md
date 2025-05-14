# Algoritmia-y-programación-Proyecto-hotelero
##############################################
# PUNTO 1 Y 2: Integrantes, vinculos académicos y descripción..
**-Katheryn Yens Martinez Perez (Encargada del codigo).** 

Soy estudiante de ingenieria industrial con poca experiencia en programacion, pero tengo la capacidad de afianzar conceptos, definiciones y metodos con bastante practica.

-Espacio para otros integrantes..........



# PUNTO 3: Nombre del proyecto y detalles.
HOTEL CIELO AZUL  
![image](https://github.com/user-attachments/assets/481b5e6b-82f0-4924-86ba-f07ed1168141)

Hotel Cielo Azul es un alojamiento frente al mar en una zona costera ideal para el descanso. Ofrece habitaciones individuales y suites modernas, atención 24 horas y un ambiente tranquilo. Está pensado para brindar comodidad y una experiencia cálida a turistas, viajeros y ejecutivos.




# PUNTO 4: Licencia de sofware.
Hotel Cielo azul © 2025 por Katheryn Martínez está licenciado bajo CC BY-NC-SA 4.0

# PUNTO 5: Reporte de visión.
Este software fue desarrollado para el Hotel Cielo Azul con el fin de poder automatizar la gestión de huéspedes, reservas, ingresos y salidas. Este busca reemplazar los procesos manuales, reducir errores y mejorar el control de las operacion. Cuando funciona de forma correcta, facilita la atención al cliente y permite generar reportes confiables de manera rápida y organizada.

# PUNTO 6: Especificación de requisitos.

Este sistema debe permitir poder registrar huéspedes con sus datos personales, tambien realizar reservas según la disponibilidad, registrar ingresos (check-in) y salidas (check-out) con una generación de facturas.  
Acicionalmente el administrador podrá acceder mediante un metodo de autenticación a los reportes actualizados sobre ocupación, los ingresos e informacion de los huéspedes.

Se espera que el sistema:
- Registre y valide correctamente los datos ingresados.
- Calcule fechas, noches y costos.
- Importe y guarde la información sin errores.
- Genere reportes y gráficos que ayuden a la vizualización y gestionar.

El sistema no debe:
- Aceptar reservas de los huéspedes que no estan registrados.
- Permitir check-in o check-out fuera de las fechas válidas.
- Acceder a reportes sin autenticación de administrador.

**Librerías que se requieren:**
- `pandas`: Esta para el manejo de datos (huéspedes, reservas).
- `datetime`: para el manejo de las fechas y horas.
- `matplotlib`: con esta se generan los graficos en el reporte administrativo.
- `getpass`, `platform`, `time`: esta para registrar los eventos del sistema.

**Funciones principales que se esperan que haga el sistema:**
- `registrar_huesped()`
- `reservar_habitacion()`
- `check_in()`
- `registrar_salida()`
- `acceder_admin()`
- `mostrar_reportes()`
- `registrar_evento()`
- `menu_principal()`

**Estructuras de datos implementadas:**
- `DataFrames` de `pandas` para almacenar huéspedes y reservas.
- Diccionarios para habitaciones, tarifas y usuarios administradores.
- Funciones por medio de modulos para mantener el código organizado y que se pueda reutilizar.

# PUNTO 7: Plan proyecto:

**Actividades principales:**

1. Análisis del problema y requerimientos del sistema.
2. Definición de funciones y estructuras de datos.
3. Desarrollo del registro de huéspedes.
4. Implementación de reservas y validaciones.
5. Programación de check-in y check-out con facturación.
6. Desarrollo del módulo de administración y reportes.
7. Implementación del log de eventos del sistema.
8. Construcción del menú general y pruebas funcionales.
9. Documentación técnica y manual de usuario.
10. Entrega en GitHub y preparación para sustentación.

**Cronograma (aqui se resume por semanas):**

| Semana | Actividad principal |
|--------|---------------------|
| 1      | Análisis y diseño del sistema |
| 2      | Registro de huéspedes y estructura base |
| 3      | Reservas y validaciones |
| 4      | Check-in y check-out |
| 5      | Administración y reportes |
| 6      | Registro de eventos (log) |
| 7      | Integración del menú principal |
| 8      | Pruebas, documentación y entrega |

**Presupuesto (en tiempo):**

- El grupo lo conformamos 3 estudiantes.
- Tiempo total invertido: **50 horas**.
- Equivalente al valor de una práctica profesional (1 SMLV).
- Distribución estimada para cada integrante: **~17 horas cada uno**.

