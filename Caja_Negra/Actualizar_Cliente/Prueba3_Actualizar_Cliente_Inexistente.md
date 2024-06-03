# Prueba 3: Actualizar Cliente Inexistente

## Objetivo
Verificar que el sistema no permite la actualización de datos de un cliente inexistente.

## Entrada
- Rut_Us: 99999999-9
- Nuevos datos del cliente:
  - Nombre_Us: Juan Pérez Actualizado
  - Direccion_Us: Calle Verdadera 456

## Proceso
El usuario intenta seleccionar un cliente inexistente.

## Salida Esperada
- Error indicando que el cliente no se encontró.

## Resultado Obtenido
- [X] Éxito
- [ ] Fallo

## Observaciones
El sistema mostró un error indicando que el cliente no se encontró.
