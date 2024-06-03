# Planilla Caso de Pruebas Estándar

## Introducción

Esta planilla está diseñada para documentar los casos de prueba estándar relacionados con la interfaz gráfica y otras funcionalidades clave del sistema. Cada caso de prueba debe ser evaluado y marcado con uno de los siguientes estados:

- **OK:** El ítem cumple lo indicado.
- **NC:** No cumple el ítem en forma óptima.
- **NA:** No aplica el ítem al componente/aplicación a evaluar.

El objetivo es asegurar que todos los elementos de la interfaz y las funcionalidades críticas cumplan con los requisitos establecidos y proporcionen una experiencia de usuario óptima.

### Casos de Pruebas Estándar

| ID     | Descripción                                                                                           | Estado      |
|--------|-------------------------------------------------------------------------------------------------------|-------------|
| **1. INTERFAZ GRÁFICA**                                                                                        |             |
| E-1.1  | Verificar que se encuentre un ícono en todos los mensajes desplegados por la aplicación               | [ ] OK [ ] NC [ ] NA |
| E-1.2  | Verificar que los íconos tengan un texto de ayuda asociado a su función                               | [ ] OK [ ] NC [ ] NA |
| E-1.3  | Verificar que la aplicación esté compuesta por múltiples pantallas estáticas y opción "Retornar" a la pantalla anterior | [ ] OK [ ] NC [ ] NA |
| E-1.4  | Verificar el tamaño de los botones                                                                    | [ ] OK [ ] NC [ ] NA |
| E-1.5  | Verificar que la etiqueta de los botones no se pierda el texto                                        | [ ] OK [ ] NC [ ] NA |
| E-1.6  | Verificar que los botones de ingreso, modificación y eliminación de estén habilitados                 | [ ] OK [ ] NC [ ] NA |
| E-1.7  | Verificar que el botón cerrar de la ventana se encuentre deshabilitado mientras se realiza un proceso | [ ] OK [ ] NC [ ] NA |
| E-1.8  | Verificar que el botón "Cancelar" no permita modificar su contenido                                   | [ ] OK [ ] NC [ ] NA |
| E-1.9  | Verificar la validación del botón "Aceptar" cuando no se han ingresado los datos                      | [ ] OK [ ] NC [ ] NA |
| E-1.10 | Verificar que no se ingrese a la pantalla si el botón "Salir de la Aplicación" está activo            | [ ] OK [ ] NC [ ] NA |
| E-1.11 | Verificar que al minimizar la pantalla, aparezca una ventana indicando el estado del producto         | [ ] OK [ ] NC [ ] NA |
| E-1.12 | Verificar que sólo la Pantalla Principal e Inicial se minimicen                                       | [ ] OK [ ] NC [ ] NA |
| E-1.13 | Verificar que el TAB esté operativo en todas las Pantallas                                            | [ ] OK [ ] NC [ ] NA |
| E-1.14 | Verificar que el TAB esté operativo en forma ordenada y secuencialmente bajo un orden lógico de ingreso | [ ] OK [ ] NC [ ] NA |
| E-1.15 | Verificar que los campos de texto tengan un formato uniforme                                          | [ ] OK [ ] NC [ ] NA |
| E-1.16 | Verificar que la información ingresada sea legible, sin cortes y que no se exceda del largo del formato de pantalla | [ ] OK [ ] NC [ ] NA |

# Planilla Caso de Pruebas

## Introducción

Esta planilla se utiliza para documentar cada caso de prueba realizado durante la fase de testing del proyecto. Incluye información detallada sobre los datos de entrada, el procedimiento de prueba, los resultados esperados y los resultados obtenidos. El objetivo es garantizar que todas las funcionalidades del sistema se verifiquen exhaustivamente y se cumplan con los requisitos establecidos.

### Información del Proyecto
- **Proyecto:** Gestión de Contratos
- **Módulo(s):** Registro de Clientes, Supervisión de Proyectos, Generación de Informes
- **Nombre Jefe de Proyecto:** Juan Pérez
- **Nombre Analista Testing:** Ana García
- **N° Ciclo:** 1
- **Fecha:** 03/06/2024

### Casos de Prueba

| N° Ciclo | Caso Us | Módulo      | Funcionalidad      | Caso de Prueba                                | Procedimiento de Prueba                                               | Datos de Prueba                                                                             | Resultado Esperado                                                  | Resultado Obtenido | Descripción                                              |
|----------|---------|-------------|--------------------|-----------------------------------------------|-----------------------------------------------------------------------|---------------------------------------------------------------------------------------------|---------------------------------------------------------------------|--------------------|----------------------------------------------------------|
| 1        | TC1.1   | Proyectos   | Crear Proyecto     | Verificar creación de proyecto con datos válidos | Ingresar detalles del proyecto y enviar el formulario                 | Codigo_C: PRJ001, Rut_Us: 12345678-9, Fecha_Inicio: 01/01/2024, Fecha_Termino: 31/12/2024   | Confirmación de creación exitosa, proyecto visible en dashboard     | SI                 | El proyecto se creó correctamente y es visible en el dashboard     |
| 1        | TC1.2   | Proyectos   | Crear Proyecto     | Intentar crear proyecto sin Fecha de Término     | Ingresar detalles del proyecto sin Fecha_Termino y enviar el formulario | Codigo_C: PRJ002, Rut_Us: 12345678-9, Fecha_Inicio: 01/01/2024                              | Error indicando que Fecha_Termino es obligatorio                   | SI                 | El sistema mostró un error indicando que Fecha_Termino es obligatorio |
| 1        | TC1.3   | Proyectos   | Crear Proyecto     | Intentar crear proyecto con Código Duplicado     | Ingresar detalles del proyecto con Codigo_C duplicado y enviar el formulario | Codigo_C: PRJ001, Rut_Us: 12345678-9, Fecha_Inicio: 01/02/2024, Fecha_Termino: 31/12/2024  | Error indicando que Codigo_C ya existe                             | SI                 | El sistema mostró un error indicando que Codigo_C ya existe        |
| 1        | TC2.1   | Proyectos   | Supervisar Proyecto | Verificar supervisión de proyecto en estado inicial | Seleccionar el proyecto y revisar los detalles                        | Codigo_C: PRJ001                                                                             | Visualización de detalles del proyecto en estado inicial            | SI                 | El sistema mostró correctamente los detalles del proyecto en estado inicial |
| 1        | TC2.2   | Proyectos   | Supervisar Proyecto | Verificar actualización del estado de un proyecto | Seleccionar el proyecto y actualizar el estado                         | Codigo_C: PRJ001, Fecha_Real_Termino: 30/11/2024                                             | Confirmación de actualización, estado actualizado visible en dashboard | SI                 | El sistema permitió la actualización y mostró el estado actualizado correctamente |
| 1        | TC2.3   | Proyectos   | Supervisar Proyecto | Intentar supervisar un proyecto inexistente       | Intentar seleccionar un proyecto inexistente                          | Codigo_C: PRJ999                                                                             | Error indicando que el proyecto no se encontró                      | SI                 | El sistema mostró un error indicando que el proyecto no se encontró |
| 1        | TC3.1   | Informes    | Generar Informe    | Verificar generación de informe de progreso para proyecto válido | Seleccionar el proyecto y rango de fechas para generar el informe     | Codigo_C: PRJ001, Fecha_Inicio: 01/01/2024, Fecha_Termino: 31/12/2024                       | Generación y visualización del informe en formato PDF o Excel       | SI                 | El sistema generó y visualizó correctamente el informe             |
| 1        | TC3.2   | Informes    | Generar Informe    | Intentar generar informe sin seleccionar proyecto | Intentar generar un informe sin seleccionar un proyecto               | Ninguna                                                                                      | Error indicando que se debe seleccionar un proyecto                 | SI                 | El sistema mostró un error indicando que se debe seleccionar un proyecto |
| 1        | TC3.3   | Informes    | Generar Informe    | Intentar generar informe para rango de fechas inválido | Seleccionar el proyecto y rango de fechas inválido                    | Codigo_C: PRJ001, Fecha_Inicio: 01/12/2024, Fecha_Termino: 31/01/2024                       | Error indicando que el rango de fechas es inválido                  | SI                 | El sistema mostró un error indicando que el rango de fechas es inválido |
| 1        | TC4.1   | Clientes    | Registro de Cliente | Verificar registro de cliente con datos válidos   | Ingresar detalles del cliente y enviar el formulario                  | Rut_Us: 98765432-1, Nombre_Us: Juan Pérez, Direccion_Us: Calle Falsa 123, Tipo_Us: C         | Confirmación de registro exitoso, cliente visible en módulo de clientes | SI                 | El cliente se registró correctamente y es visible en el módulo de clientes |
| 1        | TC4.2   | Clientes    | Registro de Cliente | Intentar registrar cliente sin Dirección          | Ingresar detalles del cliente sin Direccion_Us y enviar el formulario | Rut_Us: 98765432-1, Nombre_Us: Juan Pérez, Tipo_Us: C                                       | Error indicando que Direccion_Us es obligatoria                     | SI                 | El sistema mostró un error indicando que Direccion_Us es obligatoria |
| 1        | TC4.3   | Clientes    | Registro de Cliente | Intentar registrar cliente con Rut Duplicado       | Ingresar detalles del cliente con Rut_Us duplicado y enviar el formulario | Rut_Us: 98765432-1, Nombre_Us: Juan Pérez, Direccion_Us: Calle Falsa 123, Tipo_Us: C         | Error indicando que Rut_Us ya existe                                | SI                 | El sistema mostró un error indicando que Rut_Us ya existe          |
| 1        | TC5.1   | Clientes    | Actualización Cliente | Verificar actualización de datos de cliente existente con datos válidos | Seleccionar el cliente y actualizar los datos                         | Rut_Us: 98765432-1, Nombre_Us: Juan Pérez Actualizado, Direccion_Us: Calle Verdadera 456    | Confirmación de actualización, datos actualizados visibles en módulo de clientes | SI                 | El sistema permitió la actualización y mostró los datos actualizados correctamente |
| 1        | TC5.2   | Clientes    | Actualización Cliente | Intentar actualizar datos de cliente con datos inválidos | Seleccionar el cliente y actualizar los datos con Nombre_Us vacío     | Rut_Us: 98765432-1, Direccion_Us: Calle Verdadera 456                                        | Error indicando que Nombre_Us es obligatorio                        | SI                 | El sistema mostró un error indicando que Nombre_Us es obligatorio |
| 1        | TC5.3   | Clientes    | Actualización Cliente | Intentar actualizar datos de cliente inexistente   | Intentar seleccionar un cliente inexistente                           | Rut_Us: 99999999-9, Nombre_Us: Juan Pérez Actualizado, Direccion_Us: Calle Verdadera 456     | Error indicando que el cliente no se encontró                       | SI                 | El sistema mostró un error indicando que el cliente no se encontró |
| 1        | TC6.1   | Comisiones | Visualización Comisiones | Verificar visualización de comisiones para periodo válido | Seleccionar el periodo válido                                         | Fecha_Inicio: 01/01/2024, Fecha_Termino: 31/12/2024                                          | Visualización de las comisiones acumuladas durante el periodo seleccionado | SI                 | El sistema mostró correctamente las comisiones acumuladas durante el periodo seleccionado |
| 1        | TC6.2   | Comisiones | Visualización Comisiones | Intentar visualizar comisiones sin seleccionar periodo | Intentar visualizar comisiones sin seleccionar un periodo             | Ninguna                                                                                      | Error indicando que se debe seleccionar un periodo                  | SI                 | El sistema mostró un error indicando que se debe seleccionar un periodo |
| 1        | TC6.3   | Comisiones | Visualización Comisiones | Verificar visualización de mensaje cuando no hay comisiones para el periodo seleccionado | Seleccionar el periodo válido sin comisiones generadas                | Fecha_Inicio: 01/01/2023, Fecha_Termino: 31/12/2023                                          | Mensaje indicando que no hay comisiones para el periodo seleccionado | SI                 | El sistema mostró correctamente un mensaje indicando que no hay comisiones para el periodo seleccionado |
| 1        | TC7.1   | Proyectos   | Consultar Estado Proyecto | Verificar consulta del estado de un proyecto existente | Seleccionar el proyecto y consultar su estado                         | Codigo_C: PRJ001                                                                             | Visualización del estado actual del proyecto, incluyendo fechas y progreso | SI                 | El sistema mostró correctamente el estado del proyecto             |
| 1        | TC7.2   | Proyectos   | Consultar Estado Proyecto | Intentar consultar estado de un proyecto inexistente | Intentar seleccionar un proyecto inexistente                          | Codigo_C: PRJ999                                                                             | Error indicando que el proyecto no se encontró                      | SI                 | El sistema mostró un error indicando que el proyecto no se encontró |
| 1        | TC7.3   | Proyectos   | Consultar Estado Proyecto | Intentar consultar estado de un proyecto sin permisos adecuados | Intentar seleccionar un proyecto sin los permisos suficientes          | Codigo_C: PRJ001                                                                             | Error indicando permisos insuficientes                              | SI                 | El sistema mostró un error indicando permisos insuficientes        |



# Planilla de Registros de Defectos

## Introducción

Esta planilla se utiliza para documentar todos los defectos identificados durante la fase de testing del proyecto. Cada defecto identificado debe ser registrado con detalles precisos sobre el caso de prueba asociado, el ciclo de prueba, la fecha de identificación, el módulo afectado, una descripción detallada del defecto, su tipo, severidad, estado actual y cualquier observación relevante del equipo de desarrollo.

### Información del Proyecto
- **Nombre Proyecto:** Gestión de Contratos
- **Jefe Proyecto:** Juan Pérez
- **Analista Testing:** Ana García
- **Desarrollador:** Carlos López

### Registro de Defectos

| ID  | ID Caso Prueba | N° Ciclo | Fecha       | Módulo       | Descripción Detallada                          | Tipo    | Severidad | Estado | Observación de equipo de desarrollo |
|-----|----------------|----------|-------------|--------------|-----------------------------------------------|---------|-----------|--------|-------------------------------------|
| 1   | TC1.2          | 1        | 03/06/2024  | Proyectos    | El sistema no permite la creación del proyecto sin Fecha_Termino | Lógico  | Alta      | Abierto | Necesita validación de entrada de datos |
| 2   | TC4.3          | 1        | 03/06/2024  | Clientes     | El sistema muestra un error indicando que Rut_Us ya existe, pero debería permitir la actualización de datos | Lógico  | Media     | Abierto | Revisar lógica de actualización de datos existentes |
| 3   | TC2.3          | 1        | 03/06/2024  | Proyectos    | El sistema no permite la supervisión de un proyecto inexistente, pero no da un mensaje claro de error | UI/UX   | Baja      | Abierto | Mejorar los mensajes de error para el usuario |
| 4   | TC6.2          | 1        | 03/06/2024  | Comisiones   | El sistema no permite la visualización de comisiones sin seleccionar un periodo, pero no indica cuál es el campo requerido | UI/UX   | Media     | Abierto | Indicar claramente los campos requeridos |
