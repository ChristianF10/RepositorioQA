# Repositorio_ACS

Este repositorio contiene todos los documentos y resultados de las pruebas realizadas para el proyecto de Gestión de Contratos. La estructura del repositorio está organizada en diferentes directorios para facilitar la navegación y el acceso a la información.

## Estructura del Repositorio


```
Repositorio_ACS/
├── README.md
├── Caja_Negra/
│ ├── Crear_Proyecto/
│ │ ├── Prueba1_CrearProyecto_Valido.md
│ │ ├── Prueba2_CrearProyecto_SinFechaTermino.md
│ │ ├── Prueba3_CrearProyecto_CodigoDuplicado.md
│ ├── Supervisar_Proyecto/
│ │ ├── Prueba1_SupervisarProyecto_Valido.md
│ │ ├── Prueba2_SupervisarProyecto_FechaIncorrecta.md
│ │ ├── Prueba3_SupervisarProyecto_Inexistente.md
│ ├── Generar_Informes_Progreso/
│ │ ├── Prueba1_InformeProyecto_Valido.md
│ │ ├── Prueba2_Informe_SinSeleccionar_Proyecto.md
│ │ ├── Prueba3_Informe_Rango_Fechas_Invalido.md
│ ├── Registrar_Cliente/
│ │ ├── Prueba1_Registrar_Cliente_Valido.md
│ │ ├── Prueba2_Registrar_Cliente_Sin_Direccion.md
│ │ ├── Prueba3_Registrar_Cliente_Rut_Duplicado.md
│ ├── Actualizar_Cliente/
│ │ ├── Prueba1_Actualizar_Cliente_Valido.md
│ │ ├── Prueba2_Actualizar_Cliente_Datos_Invalidos.md
│ │ ├── Prueba3_Actualizar_Cliente_Inexistente.md
│ ├── Visualizar_Comisiones/
│ │ ├── Prueba1_Visualizar_Comisiones_Periodo_Valido.md
│ │ ├── Prueba2_Visualizar_Comisiones_Sin_Periodo.md
│ │ ├── Prueba3_Visualizar_Comisiones_Sin_Comisiones.md
│ ├── Consultar_Estado_Proyecto/
│ │ ├── Prueba1_Consultar_Proyecto_Existente.md
│ │ ├── Prueba2_Consultar_Proyecto_Inexistente.md
│ │ ├── Prueba3_Consultar_Proyecto_Sin_Permisos.md
├── Caja_Estado/
│ ├── Proyecto/
│ │ ├── Prueba1_EstadoInicial.md
│ │ ├── Prueba2_CambioEstado.md
│ │ ├── Prueba3_ActualizarEstado.md
├── Caja_Clara/
│ ├── Proyecto/
│ │ ├── Prueba1_crearProyecto.md
│ │ ├── Prueba2_actualizarProyecto.md
│ │ ├── Prueba3_eliminarProyecto.md
├── Informes/
│ ├── Informe_Pruebas_Caja_Negra.md
│ ├── Informe_Pruebas_Caja_Estado.md
│ ├── Informe_Pruebas_Caja_Clara.md
│ ├── Informe_Consolidado_Pruebas.md
├── Documentos_Pruebas/
│ ├── Planilla_Caso_Pruebas_Estandar.xlsx
│ ├── Planilla_Caso_Pruebas.xlsx
│ ├── Planilla_Registros_Detectos.xlsx
├── Perfil_de_Uso.md

```

## Descripción de Directorios

- **Caja_Negra**: Contiene los casos de prueba realizados bajo la metodología de caja negra.
- **Caja_Estado**: Contiene los casos de prueba realizados bajo la metodología de caja estado.
- **Caja_Clara**: Contiene los casos de prueba realizados bajo la metodología de caja clara.
- **Informes**: Contiene los informes detallados de las pruebas realizadas y un informe consolidado.
- **Documentos_Pruebas**: Contiene las planillas de pruebas en formato Excel.
- **Perfil_de_Uso.md**: Documento que describe el perfil de uso del sistema basado en los escenarios de uso definidos.

## Cómo Usar Este Repositorio

1. **Navegar por los directorios**: Cada directorio está organizado por tipo de prueba y funcionalidad. Selecciona el directorio que corresponde a la prueba que deseas revisar.
2. **Revisar los documentos de prueba**: Cada archivo Markdown (.md) contiene los detalles de las pruebas realizadas, incluyendo objetivos, entradas, procesos, salidas esperadas, resultados obtenidos y observaciones.
3. **Consultar los informes**: Los informes detallan los resultados de las pruebas realizadas y proporcionan una visión general del estado del proyecto.
4. **Acceder a las planillas de pruebas**: Las planillas de pruebas en formato Excel están disponibles en el directorio `Documentos_Pruebas/` y pueden ser utilizadas para análisis y seguimiento de las pruebas y defectos.
