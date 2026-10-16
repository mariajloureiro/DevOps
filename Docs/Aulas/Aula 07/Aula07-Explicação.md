# Aula 7: Monitoramento, Observabilidade e Feedback

## 1. Monitoramento vs. Observabilidade

* **Monitoramento:** Focado no que é conhecido (*"Known-Unknowns"*). Informa quando algo deu errado (ex: Alerta se o uso de CPU passar de 90%).
* **Observabilidade:** Focado no desconhecido (*"Unknown-Unknowns"*). Permite entender a causa raiz de problemas complexos analisando os dados emitidos pelo sistema.

---

## 2. Os Três Pilares da Observabilidade

```
                  ┌─────────────────┐
                  │ Observabilidade │
                  └────────┬────────┘
        ┌──────────────────┼──────────────────┐
        ▼                  ▼                  ▼
  1. Métricas          2. Logs            3. Traces
(Dados Agregados)   (Eventos Discretos)  (Jornada da Requisição)
```

1. **Métricas:** Dados numéricos agregados ao longo do tempo (ex: Taxa de erros 5xx, latência média).
2. **Logs:** Registro textual de eventos específicos com contexto e timestamp.
3. **Traces (Rastreamento Distribuído):** Acompanha uma requisição à medida que ela passa por múltiplos microserviços.

---

## 3. Stack Tecnológica Popular
* **Métricas:** Prometheus + Grafana.
* **Logs:** ELK / PLG Stack (Promtail + Loki + Grafana / Elasticsearch + Logstash + Kibana).
* **Tracing:** OpenTelemetry + Jaeger.