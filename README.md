# otlp-forwarding
forwarding opentelemetry with fluentbit

> Disclaimer: Current setup doens't seem to work

# How to reproduce

1. docker-compose up -d
2. curl  http://localhost:8080/WeatherForecast
3. find activity id in the logs, e.g. docker-compose logs webapp
4. open grafana/tempo on http://localhost:3000 and search for the previous found activity id (= trace id)

