# Repositorio de Resultados de Pruebas de Software

Este repositorio está diseñado para almacenar los resultados de las pruebas realizadas en el proyecto de análisis de resultados de pruebas de software. Proporciona una estructura organizada para diferentes tipos de pruebas y documentos relacionados, permitiendo un seguimiento efectivo y detallado de las pruebas.

## Objetivo del Proyecto

El objetivo de este proyecto es asegurar la calidad y confiabilidad del sistema de gestión de proyectos y contratos a través de pruebas exhaustivas. Se incluyen pruebas de caja negra, caja de estado y caja clara, así como informes detallados de los resultados y un perfil de uso del sistema.

## Estructura del Repositorio

La estructura del repositorio se divide en varias carpetas, cada una dedicada a un tipo específico de prueba o documento.

### Caja_Negra

Contiene las pruebas de caja negra, las cuales se centran en la funcionalidad externa del sistema sin considerar la estructura interna del código. Cada subcarpeta representa un caso de uso específico y contiene los casos de prueba correspondientes.


```
Caja_Negra/
├── Crear_Proyecto/
│ ├── Prueba1_CrearProyecto_Valido.md
│ ├── Prueba2_CrearProyecto_SinFechaTermino.md
│ ├── Prueba3_CrearProyecto_CodigoDuplicado.md
├── Supervisar_Proyecto/
│ ├── Prueba1_SupervisarProyecto_Valido.md
│ ├── Prueba2_SupervisarProyecto_FechaIncorrecta.md
│ ├── Prueba3_SupervisarProyecto_Inexistente.md
├── Generar_Informes_Progreso/
│ ├── Prueba1_Informe_Proyecto_Valido.md
│ ├── Prueba2_Informe_Sin_Seleccionar_Proyecto.md
│ ├── Prueba3_Informe_Rango_Fechas_Invalido.md
├── Registrar_Cliente/
│ ├── Prueba1_Registrar_Cliente_Valido.md
│ ├── Prueba2_Registrar_Cliente_Sin_Direccion.md
│ ├── Prueba3_Registrar_Cliente_Rut_Duplicado.md
├── Actualizar_Cliente/
│ ├── Prueba1_Actualizar_Cliente_Valido.md
│ ├── Prueba2_Actualizar_Cliente_Datos_Invalidos.md
│ ├── Prueba3_Actualizar_Cliente_Inexistente.md
├── Visualizar_Comisiones/
│ ├── Prueba1_Visualizar_Comisiones_Periodo_Valido.md
│ ├── Prueba2_Visualizar_Comisiones_Sin_Periodo.md
│ ├── Prueba3_Visualizar_Comisiones_Sin_Comisiones.md
├── Consultar_Estado_Proyecto/
│ ├── Prueba1_Consultar_Proyecto_Existente.md
│ ├── Prueba2_Consultar_Proyecto_Inexistente.md
│ ├── Prueba3_Consultar_Proyecto_Sin_Permisos.md

```

### Caja_Estado

Incluye pruebas de caja de estado que verifican el comportamiento del sistema en función de sus estados. Cada prueba valida transiciones y estados específicos del sistema.

```
Caja_Estado/
└── Proyecto/
├── Prueba1_EstadoInicial.md
├── Prueba2_CambioEstado.md
├── Prueba3_ActualizarEstado.md
```

### Caja_Clara

Contiene pruebas de caja clara que se alinean con el diseño procedimental y de programación estructurada del sistema. Estas pruebas verifican la correcta ejecución de funciones y procedimientos detallados.

```
Caja_Clara/
└── Proyecto/
├── Prueba1_crearProyecto.md
├── Prueba2_actualizarProyecto.md
├── Prueba3_eliminarProyecto.md
```

### Informes

Esta carpeta almacena los informes generados a partir de las pruebas realizadas. Incluye informes específicos para cada tipo de prueba y un informe consolidado que resume todos los resultados.

```
Informes/
├── Informe_Pruebas_Caja_Negra.md
├── Informe_Pruebas_Caja_Estado.md
├── Informe_Pruebas_Caja_Clara.md
└── Informe_Consolidado_Pruebas.md
```


### Perfil_de_Uso.md

Este archivo documenta el perfil de uso del sistema, asignando probabilidades a diferentes escenarios de uso basados en la frecuencia esperada de cada escenario en el uso real del sistema.

## Cómo Utilizar el Repositorio

1. **Ejecutar Pruebas:** Siga los casos de prueba detallados en las carpetas de Caja_Negra, Caja_Estado y Caja_Clara para realizar las pruebas correspondientes.
2. **Registrar Resultados:** Documente los resultados de cada prueba en los archivos `.md` correspondientes.
3. **Generar Informes:** Compile los resultados en los informes ubicados en la carpeta Informes.
4. **Actualizar Perfil de Uso:** Mantenga actualizado el archivo Perfil_de_Uso.md para reflejar los cambios y las nuevas pruebas añadidas.

## Contribuciones

Las contribuciones al repositorio son bienvenidas. Por favor, siga las directrices de contribución y asegúrese de documentar claramente cualquier nueva prueba o informe añadido.

---

Este repositorio es una herramienta fundamental para garantizar la calidad y la confiabilidad del sistema de gestión de proyectos y contratos, facilitando una gestión efectiva de las pruebas y sus resultados.

