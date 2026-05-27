# Histórias de Usuário - Sistema Nomeando

Este documento detalha as Histórias de Usuário (HUs) para as funcionalidades de criação por categorias, aplicação de critérios de avaliação e exibição da nuvem de palavras.

---

## HU01 - Criar Nome por Categoria
**ID:** HU01  
**Prioridade:** Alta  
**Requisito Relacionado:** RF03 (Criação por categorias)

### Descrição
Como **Jogador**, desejo inserir sugestões de nomes baseadas em categorias sorteadas de forma individual e oculta, para que eu possa contribuir com ideias sem ser influenciado pelas sugestões dos outros participantes.

### Critérios de Aceite
1. O sistema deve exibir claramente a categoria sorteada para a rodada (ex: natureza, gírias, tecnologia).
2. O sistema deve fornecer um campo de entrada de texto para que o jogador insira sua sugestão.
3. As sugestões enviadas por outros jogadores devem permanecer ocultas (ex: exibidas como cadeados ou borrões) até o encerramento do tempo da rodada.
4. O sistema deve exibir um cronômetro regressivo com alerta visual nos últimos 10 segundos.
5. O sistema deve permitir que o jogador envie múltiplas palavras dentro do tempo definido.

---

## HU02 - Aplicação de Critério de Avaliação
**ID:** HU02  
**Prioridade:** Alta  
**Requisito Relacionado:** RF05 (Aplicação de critérios de avaliação)

### Descrição
Como **Participante (Mestre ou Jogador)**, desejo avaliar os nomes finalistas com base em critérios técnicos pré-definidos, para que possamos filtrar e eliminar opções que não atendam aos requisitos de marca (sonoridade, escrita, disponibilidade).

### Critérios de Aceite
1. O sistema deve listar os nomes que sobreviveram às fases de exclusão anteriores.
2. Para cada nome, o sistema deve permitir marcar o atendimento ou violação de critérios como: Sonoridade, Escrita, Disponibilidade de Domínio/Redes Sociais e Originalidade.
3. O sistema deve exibir a descrição de cada critério ao passar o mouse ou clicar em um ícone de ajuda.
4. O sistema deve eliminar automaticamente os nomes que ultrapassarem o limite de violações configurado pelo Mestre no início da sessão.
5. O progresso da avaliação deve ser visível para todos os participantes em tempo real.

---

## HU03 - Exibição de Nuvem de Palavras
**ID:** HU03  
**Prioridade:** Média  
**Requisito Relacionado:** RF08 (Exibição de nuvem de palavras)

### Descrição
Como **Participante**, desejo visualizar uma nuvem de palavras consolidada que reúna todas as sugestões feitas, incluindo estalos criativos, para que tenhamos um painel visual rico de todas as ideias geradas durante a dinâmica.

### Critérios de Aceite
1. A nuvem de palavras deve agrupar nomes vindos da fase de categorias e os "estalos criativos" adicionados espontaneamente.
2. A nuvem deve ser atualizada dinamicamente sempre que uma nova palavra for adicionada ao sistema.
3. O tamanho das palavras na nuvem deve ser proporcional à frequência com que foram sugeridas (se aplicável) ou destaque visual para termos recentes.
4. O sistema deve permitir que o Mestre da Sessão exporte a nuvem de palavras ou a utilize como base de reposição em fases de exclusão futuras.
5. A interface da nuvem deve ser responsiva e visualmente atraente, reforçando o caráter gamificado do sistema.
