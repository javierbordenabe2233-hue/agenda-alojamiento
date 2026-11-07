# Agenda de alojamientos

App para gestionar las reservas, pagos, comisiones, gastos e ingresos de:

- **Casita del Bosque** (alojamiento)
- **Casa Calandria** (alojamiento)
- **Fiammata del Fuego** (salón de eventos)

Funciona en el celular como una app instalada, **sin internet** y **sin cuenta**. Los datos se guardan **en la memoria del teléfono**.

## Qué hace

- **Calendario** con la ocupación de cada lugar (solo para ver).
- **Reservas**: valor por noche × noches (o valor total del evento), en pesos o dólares con conversión al dólar oficial, seña y saldo (fijo o actualizable al dólar del día de pago), comisiones (Airbnb, Booking, inmobiliaria, recepción de huéspedes u otra) que se suman, y cancelación de reservas.
- **Movimientos**: gastos e ingresos por lugar o generales, con **PDF** para enviar.
- **Resumen** mensual por lugar: ingresos, comisiones, gastos, resultado, ocupación y lo que falta cobrar.
- **Copia de seguridad**: guardar y restaurar todos los datos en un archivo.
- Dos diseños: "libreta fueguina" y clásico (botón de la paleta, arriba a la derecha).

## Publicarla (una sola vez)

1. En GitHub, entrá a **Settings → Pages** de este repositorio.
2. En **Source** elegí **Deploy from a branch**, rama **main** y carpeta **/ (root)**. Guardá.
3. En uno o dos minutos la app queda en:
   `https://javierbordenabe2233-hue.github.io/agenda-alojamiento/`

## Instalarla en el celular

- **Android (Chrome):** abrí el link → menú ⋮ → **Instalar app** (o "Agregar a pantalla principal").
- **iPhone (Safari):** abrí el link → botón **Compartir** → **Agregar a inicio**.

Después se abre desde el ícono como cualquier app, y funciona sin conexión. (El PDF necesita internet la primera vez que se usa, para descargar el generador; después queda guardado.)

## Importante sobre los datos

- Cada teléfono tiene **sus propios datos**. Lo que se carga en un celular no aparece en otro.
- Si se borran los datos del navegador, se desinstala la app o se pierde el teléfono, **se pierden los datos**. Por eso conviene usar **Resumen → Copia de seguridad → Guardar copia** seguido, y guardar el archivo en Drive, mail o WhatsApp.
- Para pasar los datos a otro teléfono: guardá una copia en uno y usá **Restaurar copia** en el otro (reemplaza todo lo que haya en el segundo).
- En iPhone, abrí siempre la app desde el ícono de inicio (no desde Safari), así usa siempre el mismo espacio de datos.

## Cotización del dólar

La app no consulta internet para la cotización: se carga a mano el dólar oficial (venta, Banco Nación) tocando el recuadro de arriba a la derecha. Se guarda un historial por fecha.

## Archivos

- `index.html` — la app completa.
- `manifest.json`, `icons/` — para instalarla como app.
- `sw.js` — permite usarla sin internet.
