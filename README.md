# mwo_app_profile

Interfaccia utente per la gestione profili (modulo `mwo_ui`): frontend Java EE che consuma le API di `api-mwo-profile`.

## Stack tecnologico

- Java EE (JAX-RS / RESTEasy)
- Maven
- JSON (json-simple)

## Build

```bash
mvn clean package
```

L'artefatto prodotto va rilasciato su un application server compatibile Java EE (es. WildFly / JBoss).

## Contesto

Coppia backend/frontend:

- `api-mwo-profile` — API / controller
- `mwo_app_profile` — questo modulo: interfaccia utente

## Contatti

Andrei Alexandru Dabija — [LinkedIn](https://www.linkedin.com/in/andrei-alexandru-dabija/) — [github.com/XtremeAlex](https://github.com/XtremeAlex)
