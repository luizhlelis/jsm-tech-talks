# JS+ TechTalks #15 - Padrão Trace Context W3C para rastreamento distribuído

## Glossário

- `tracing`: rastreamento / uma prática de baixo nível usada para criar o perfil e analisar códigos por meio de uma combinação de ferramentas de depuração especializadas (Linux dtrace ou Windows ETW).

- `distributed tracing`: uma aplicação das técnicas de rastreamento tradicionais citadas acima em arquiteturas distribuídas.

- `trace`: um rastro / representa a jornada de um única ação de usuário por uma pilha inteira de spans. Também pode ser definido como: dados contextuais sobre uma requisição ao longo de um sistema.

- `metrics`: informações quantitativas sobre processos.

- `log`: mensagens específicas emitidas por um processo ou serviço.

- `span`: representa uma operação individual do trace completo (um domínio ou escopo específico).

- `tracer`: responsável por criar os spans.

- `context`: também conhecido como contexto de rastreamento (trace context) contém várias informações que podem ser passadas entre funções dentro de um mesmo processo ou entre processos diferentes em um RPC. O contexto pode conter informações sobre o processo, sobre a requisição e também campos personalizados.

- `events`: responsável por dar contexto a um span. É estruturado em: nome, timestamp e zero ou mais atributos.

- `attributes`: lista de zero ou mais pares de chave-valor que compõe um evento.

- `observability`: capacidade de entender o desempenho de um aplicativo com base em dados de saída ou telemetria. O termo deriva da teoria de controle, uma engenharia que se preocupa em manter sistemas dinâmicos dentro de faixas desejadas e em inferir o estado interno de um sistema com base nas suas saídas externas.

- `telemetry`: dados emitidos por uma aplicação referentes ao seu comportamento. Em sistemas distribuídos, a telemetria pode ser dividida em três grandes categorias: metrics, logs, traces.

- `baggage`: adiciona contexto e informações às métricas, traces e logs. É um conjunto de pares nome/valor que descreve propriedades definidas pelo usuário.

- `instrumentation`: adicionar código a serviços para monitorar e rastrear seu sistema.

- `OpenTelemetry`: conjunto de APIs, SDKs, ferramentas e integrações que são projetadas para a criação e gerenciamento de dados de telemetria (métricas, traces e logs). O projeto fornece uma implementação independente de fornecedor que pode ser configurada para enviar dados de telemetria ao(s) backend(s) de sua escolha. Ele suporta uma variedade de projetos populares de código aberto, incluindo Jaeger, Prometheus e W3C TraceContext.

## Referências

[Dapper, a Large-Scale Distributed Systems Tracing Infrastructure](https://research.google/pubs/pub36356/)

[Using W3C Trace Context standard in distributed tracing](https://dev.to/luizhlelis/using-w3c-trace-context-standard-in-distributed-tracing-3743)

[[c#] Using W3C Trace Context standard in distributed tracing](https://dev.to/luizhlelis/c-using-w3c-trace-context-standard-in-distributed-tracing-1nm0)

[Why distributed tracing will replace (most) logging](https://www.youtube.com/watch?v=Hv98hU3nj0U)

[Context Propagation makes OpenTelemetry awesome](https://www.youtube.com/watch?v=gviWKCXwyvY)

[Opentelemetry explain like I'm five](https://go.lightstep.com/rs/260-KGM-472/images/opentelemetry-explain-like-im-five.pdf)

[OpenTelemetry 101: What is tracing?](https://lightstep.com/blog/opentelemetry-101-what-is-tracing/)

[What is OpenTelemetry?](https://opentelemetry.io/docs/concepts/what-is-opentelemetry/)

[Opentelemetry Glossary](https://opentelemetry.io/docs/concepts/glossary/)
