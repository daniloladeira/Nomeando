## HU05 - Adicionar estalo criativo
**ID:** HU04 
**Prioridade:** Baixa  
**Requisito Relacionado:** RF02 (Adição de estalos criativos)

### Descrição
Como **Mestre da Sessão ou Jogador**, desejo **inserir a sugestão de um nome**, para **adicionar um estalo criativo**.

### Especificações Técnicas

#### Campos do Formulário de criar sessão:

| Campo             | Descrição                  | Tipo de Campo | Tipo de Dado | Tamanho | Máscara            | Obrigatório |
|-------------------|----------------------------|---------------|--------------|---------|--------------------|-------------|
| `Nome` | Nome pensado no estalo criativo. | Texto | Alfanumérico |  N/A  | N/A | Sim |
| `Categoria` |Categoria associada ao nome. | Seleção | Alfanumérico | N/A  | N/A | Sim |

### Critérios de Aceite
1. O sistema deve permitir que a sugestão de estalo criativo seja feita durante qualquer momento do jogo.
2. O sistema deve permitir a seleção de apenas uma categoria por estalo criativo.
