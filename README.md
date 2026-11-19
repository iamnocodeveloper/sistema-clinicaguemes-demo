# sistema-clinicaguemes-demo

Demo navegable del **sistema de gestión** de Clínica Güemes — Medicina Integral (San Juan, Argentina).

Es el complemento de la web pública: la landing atrae y da turnos; este panel es lo que la clínica usa todos los días.

## Qué incluye

Aplicación de una sola página (`index.html`, CSS y JS inline, sin backend ni dependencias externas salvo Google Fonts):

- **Entrada simulada**: usuario demo precargado y botón «Entrar en modo demostración».
- **Escritorio**: turnos de hoy, profesionales en consulta, estudios pendientes de informar, pacientes sin volver, cobros del día y avisos.
- **Agenda**: vista de día con carriles por profesional (turnos ubicados por hora y con su duración) y vista semanal; filtros por especialidad y profesional; detalle de cada turno y alta real de turnos desde el formulario, con aviso si se superpone el horario del profesional.
- **Pacientes**: buscador y listado; ficha con contacto, obra social, historial de consultas agrupado por especialidad, estudios, recetas y observaciones.
- **Mensajes**: bandeja tipo WhatsApp con recordatorios de turno, confirmaciones, avisos de resultados listos y reagendamientos.
- **Pagos**: cobros del mes con fecha, paciente, práctica, obra social, medio de pago y estado; totales, ticket promedio y desglose por obra social.
- **Informes**: turnos por semana, especialidades más pedidas, ingresos por mes, ausentismo y confirmados vs. cancelados, todo con SVG y CSS sin librerías.
- **Ajustes**: catálogo de prácticas editable en memoria (valor y duración), profesionales y especialidades, horarios de atención y configuración de recordatorios.
- Menú de usuario con acceso a la web pública y pie con la nota de demo.

Los datos son de ejemplo y se generan en el navegador, relativos a la fecha en que se abre el demo: 25 profesionales de 9 especialidades, 120 pacientes, alrededor de 100 turnos en el mes, 8 estudios pendientes de informar, obras sociales argentinas como texto (Particular, PAMI, OSDE, Swiss Medical, Obra Social Provincial, OMINT) y montos en pesos.

## Despliegue

`Dockerfile` de dos líneas (`nginx:alpine` + copia de los archivos) publicado desde este repositorio en EasyPanel:

- Sistema: https://clientes-sistema-clinicaguemes.rddxeh.easypanel.host/

## Nota

Demo de referencia hecho por Nocodeveloper. No envía mensajes, no guarda datos y no incluye información real de terceros; en el sistema real se cargan los datos de la clínica.