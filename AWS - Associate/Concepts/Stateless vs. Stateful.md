![[Pasted image 20261029082248.png]]


## Stateful

_O programa tem uma memória (estado)._

Já o Stateful mantém o controle do estado de interação da aplicação e permite que os dados possam ser mantido entre diferentes requisições.

Exemplo: Java — HttpSession, C# APS.net — Session, JavaScript — SessionStorage.

Imagine uma solicitação web onde você tem um navegador cliente para se comunicar a um processo do servidor.

## Stateless

Não há memória (estado) que é mantido pelo programa.

No conceito de Stateless nenhum registro ou estado de todas as interações anteriores na aplicação são salvos e cada interação é tratada com base nas informações disponíveis para a interação.

Exemplo: Protocolos de Internet (IP), Protocolo de transferência de Hyper Texto (HTTP).

No exemplo do HTTP, cada requisição que é feita pelo navegador é de forma independente. Assim que o navegador fecha a conexão _TCP_, toda a informação é perdida. Mesmo que várias requisições sejam enviadas pela mesma conexão _TCP_, uma requisição não sabe da outra.