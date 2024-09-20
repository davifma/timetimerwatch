```mermaid
usecaseDiagram
    actor User as "Usuário"
    actor SmartWatch as "Smart Watch"

    User --> (Iniciar Contagem)
    User --> (Pausar Contagem)
    User --> (Zerar Contagem)
    User --> (Configurar Contador)
    User --> (Selecionar Tipo de Contador)

    (Configurar Contador) --> (Contar Até)
    (Configurar Contador) --> (Regredir Até Hora)

    SmartWatch --> (Iniciar Contagem)
    SmartWatch --> (Pausar Contagem)
    SmartWatch --> (Zerar Contagem)
    SmartWatch --> (Configurar Contador)
    SmartWatch --> (Selecionar Tipo de Contador)
```
