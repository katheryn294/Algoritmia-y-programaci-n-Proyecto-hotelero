# Manual de Usuario – Hotel Cielo Azul

## Introducción

Este manual tiene como propósito orientar al usuario en el uso correcto del sistema de consola desarrollado para el Hotel Cielo Azul.  
El programa permite registrar huéspedes, realizar reservas, controlar ingresos y salidas, generar facturas, acceder a reportes administrativos y registrar eventos del sistema.

##Requisitos para ejecutar el programa

- Python 3.x instalado o uso de Google Colab.
- Librerías necesarias:
  - `pandas`
  - `datetime`
  - `matplotlib` (para reportes gráficos)
  - `re`, `time`, `platform`, `getpass`
- Archivos generados automáticamente:
  - `log_eventos.txt` (registro de acciones del sistema)

---

## 🏁 Inicio del programa

Al ejecutar el programa, se mostrará un menú principal con las siguientes opciones:

1-Registrar Huésped

2-Realizar Reserva

3-Registrar Ingreso (Check-In)

4-Registrar Salida (Check-Out)

5-Administración (Acceso restringido)

6-Salir




## 1. Registrar Huésped

Permite ingresar los datos de un nuevo huésped. El sistema solicitará:

- Nombre (mínimo 3 letras, solo letras)
- Apellido (mínimo 3 letras, solo letras)
- Documento de identidad (3 a 15 dígitos)
- Correo electrónico válido
- Teléfono de contacto (7 a 15 dígitos)

Si los datos son válidos, se almacenan en el sistema.  
En caso de error, el sistema mostrará los campos que deben corregirse.

---

## 2. Realizar Reserva

Permite reservar una habitación para un huésped previamente registrado.

Se solicita:

- Documento del huésped
- Tipo de habitación (estándar o suite)
- Fecha de ingreso (YYYY-MM-DD)
- Número de noches de estancia

El sistema verifica disponibilidad y, si hay habitaciones libres, muestra un comprobante de reserva con:

- Tipo y número de habitación
- Fechas de ingreso y salida
- Número de noches
- Costo estimado

---

## 3. Registrar Ingreso (Check-In)

Permite registrar el ingreso del huésped. El sistema:

- Verifica si existe una reserva activa para la fecha actual
- Marca la reserva como activa (`CheckIn = True`)
- No permite check-in si la fecha no coincide con la programada

---

## 4. Registrar Salida (Check-Out)

Se usa cuando el huésped finaliza su estancia. El sistema:

- Calcula el número de noches
- Aplica la tarifa por tipo de habitación:
  - Estándar: $120,000 por noche
  - Suite: $250,000 por noche
- Cobra al menos una noche
- Muestra una factura detallada:
  - Datos del huésped
  - Fechas de ingreso y salida
  - Total a pagar
- Elimina la reserva del sistema

---

## 5. Administración

Requiere ingresar un **usuario y contraseña válidos**.

Una vez autenticado, el administrador accede a los siguientes reportes:

### Reportes Administrativos (en consola):

- Total de huéspedes registrados
- Total de habitaciones ocupadas
- Total de habitaciones disponibles
- Total de ingresos generados
- Tiempo promedio de estancia por huésped
- Lista de huéspedes con historial de reservas
- Huésped con mayor número de noches
- Huésped con menor número de noches

### Visualización de Reportes Gráficos

Después de mostrar los reportes en texto, el sistema preguntará:


¿Deseas ver los gráficos administrativos? (s/n):

Si se responde "s", se mostrarán **8 gráficos** distribuidos en dos ventanas para facilitar su lectura:


#### gráficos:

1. **Gráfica de barras**  
   Habitaciones ocupadas por tipo.

2. **Gráfica circular (pie chart)**  
   Ocupadas vs. disponibles.

3. **Gráfica de líneas**  
   Check-outs por día.

4. **Barras horizontales (Top 10)**  
   Huéspedes con más noches hospedadas.

5. **Gráfica de dispersión (scatter plot)**  
   Noches vs. costo total.

6. **Gráfica circular (pastel)**  
   Ingresos por tipo de habitación.

7. **Histograma**  
   Distribución de duración de estancias.

8. **Gráfico combinado (barras + líneas)**  
   Ingresos diarios y cantidad de huéspedes.

---

## Registro de Eventos (Log)

El sistema guarda automáticamente en el archivo `log_eventos.txt` los eventos más importantes.  
Cada registro incluye:

- Fecha y hora (hasta milisegundos)
- Acción ejecutada (ej. “Registrar huésped”, “Check-out”)
- Duración de la operación
- Usuario del sistema, sistema operativo y plataforma


---

## 6. Salir

Finaliza la ejecución del sistema y guarda el evento en el archivo de log.

---

