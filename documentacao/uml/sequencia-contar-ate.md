```mermaid
sequenceDiagram
    participant User as Usuário
    participant SmartWatch as SmartWatch
    participant UserInterface as UserInterface
    participant Timer as Timer
    participant CountdownTimer as CountdownTimer

    User ->> SmartWatch: Swipe para a esquerda
    SmartWatch ->> UserInterface: Mostrar opções de contador
    User ->> UserInterface: Selecionar "Contar Até"
    UserInterface ->> Timer: Criar instância de CountdownTimer
    Timer ->> CountdownTimer: Inicializar
    User ->> UserInterface: Inserir tempo alvo
    UserInterface ->> CountdownTimer: setTargetTime(tempo)
    CountdownTimer ->> UserInterface: Confirmar configuração
    UserInterface ->> User: Exibir confirmação
```
