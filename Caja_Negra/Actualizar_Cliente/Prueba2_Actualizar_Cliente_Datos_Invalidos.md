# Prueba 2: Actualizar Cliente con Datos Inválidos

## Objetivo
Verificar que el sistema no permite la actualización de datos de un cliente con datos inválidos.

## Entrada
- Rut_Us: 98765432-1
- Nuevos datos del cliente:
  - Nombre_Us:
  - Direccion_Us: Calle Verdadera 456

## Proceso
El usuario selecciona el cliente y actualiza los datos con Nombre_Us vacío.

## Salida Esperada
- Error indicando que Nombre_Us es obligatorio.

## Resultado Obtenido
- [X] Éxito
- [ ] Fallo

## Observaciones
El sistema mostró un error indicando que Nombre_Us es obligatorio.
