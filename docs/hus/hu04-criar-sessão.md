## HU04 - Criar Sessão
**ID:** HU04 
**Prioridade:** Alta  
**Requisito Relacionado:** RF01 (Criação de uma sessão)

### Descrição
Como **Mestre da Sessão**, desejo **criar uma sessão de jogo**, para **personalizar uma partida de nomeação**.

### Especificações Técnicas

#### Campos do Formulário de criar sessão:

| Campo             | Descrição                  | Tipo de Campo | Tipo de Dado | Tamanho | Máscara            | Obrigatório |
|-------------------|----------------------------|---------------|--------------|---------|--------------------|-------------|
| `Tempo da rodada` | Quantidade de tempo, em segundos, que durará uma rodada de seleção de nome por categoria. | Texto | Alfanumérico |  5 digítos  | N/A | Sim |
| `Conceito` | Nomes que estão relacionados ao conceito do projeto. | Texto | Alfanumérico |  10 opções  | N/A | Sim |

### Critérios de Aceite
1. As configurações das partidas devem ser ocultadas para outros jogadores, ou seja, devem ser exibidas apenas para o mestre da sessão.
2. O sistema deve permitir apenas o usuário que criou a partida, mestre da essão, acesse as informações.
