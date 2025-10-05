---
name: "NFR"
about: "Definir un requisito no funcional medible"
title: "NFR-<ID>: <nombre corto>"
labels: ["type:NFR","priority:P?","tier:T?","area:?"]
assignees: []
---

## Descripción breve
<!-- ¿Qué atributo de calidad cubre y por qué importa para negocio/usuario? -->

## Alcance (servicios / rutas / contexto)
- Servicios: <!-- e.g., auth-iam, dir-interop, doc-meta, doc-content -->
- Entornos: <!-- dev/stg/prod -->
- Horario aplicable: <!-- 24x7 / horario pico -->

## SLI (qué medimos)
<!-- Latencia p95/p99, tasa de error, disponibilidad, throughput, etc. -->

## SLO (objetivo/umbral)
<!-- p.ej., p95 < 800 ms; disponibilidad 99.95% mensual -->

## Medición / Instrumentación
- Cómo: <!-- APM, OpenTelemetry, synthetic checks, logs -->
- Dónde: <!-- dashboard, alerta, panel -->
- Frecuencia: <!-- continua / cada deploy / mensual -->

## Datos de referencia / hipótesis de carga
<!-- DAU, QPS esperado, tamaño de payload, concurrencia, picos -->

## Criterios de aceptación (DoR/DoD)
- [ ] Dashboard con SLI visible en tiempo real
- [ ] Alarmas configuradas (umbral + canal)
- [ ] Pruebas (carga/sintéticas) demuestran el SLO
- [ ] Documentación/Runbook actualizados
- [ ] No rompe compatibilidad (si aplica)

## Riesgos / Dependencias
<!-- CNI/red, storage, PKI, terceros, colas, etc. -->

## Notas de granularidad (cohesión/volatilidad)
<!-- ¿Este RNF fuerza separar o mantener juntos sub-módulos? Reglas/umbrales -->
