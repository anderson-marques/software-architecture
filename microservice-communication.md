# Microservices Communication

## Challenges involved Microservices Communication Patterns

    - synchronous or asynchronous communication
        - MOM (Messanging)
    - message payloads encodings
        - XML
        - Json
        - Binary
        - Bson
    - message serialization
        - Registers
        - Apache Avro

    - Internet Communication Model - Channel properties:
        - Direction
        - Data format/Codec        
        - synchronicity
        - Deliver guarantees
        - Security
        - Performance/Latency
        - Overhead (Payload/Overall)

    - Message Receiver Cardinality
        - Unicast - 1:1
        - Multicast - 1:N
        - Broadcast - 1:*

    - Direction
        - Request/Response: ->;<-
        - Push: <-
        - Peer-to-Perr: <->

## Guarding synchronous calls by using a circuit breaker

- Detects failure and protects the system maintaining healthy
- Netflix Hystrix
- It is like the default behavior of Load Balancer that monitor
  errors, thresholds, timeouts and intervals

## Topic based async pub-sub using Apache Kafka
## RPC Communication
## async message work queues using RabbitMQ