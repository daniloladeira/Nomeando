# Documento de Visão e Escopo

## [NOME DO SISTEMA]

**Componentes:**
- Ana Maria
- Danilo Ladeira

## Histórico de Revisões

|    Data    | Versão |             Descrição             |             Autores             |
| :--------: | :----: | :---------------------------------: | :-----------------------------: |
| 26/03/2026 |  1.0   |  Criação do esqueleto do documento  | Danilo Ladeira - @daniloladeira |
| 31/03/2026 |  1.1   | Definição dos requisitos funcionais |      Ana Maria - @namariaa      |
| 31/03/2026 |  1.2   | Definição do objetivo do projeto, descrição dos usuários e requisitos não funcionais |      Danilo Ladeira - @daniloladeira      |

---

## 1. Requisitos de Negócio

### 1.1. Objetivo do Projeto

Desenvolver uma plataforma digital colaborativa e gamificada que automatize e estruture a técnica de criação de nomes de marcas elaborada no IFRN. O sistema tem como meta guiar equipes através de sessões interativas de ideação, votação, avaliação de critérios e transformação de palavras (utilizando o método MEIA). A solução visa substituir o processo manual por um ambiente virtual organizado e em tempo real, garantindo maior engajamento dos participantes, registro seguro de todas as ideias e eficiência na tomada de decisão para a escolha do nome final.

---

## 2. Descrição do Problema

|              |                                                                                                                                                                                     |
| ------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Problema** | Inexistência de uma plataforma digital que ofereça suporte à execução de uma técnica coletiva, desenvolvida no IFRN, para definição de nomes de marcas, produtos e sistemas.        |
| **Afeta** | Designers, equipes de desenvolvimento e stakeholders envolvidos no processo de decisão de nomes.                                                                                    |
| **Impacta** | Perda de tempo, dificuldade de organização das ideias e risco de escolha de nomes inadequados ao contexto, além da baixa participação da equipe na decisão.                         |
| **Solução** | Criação de um sistema interativo, estruturado como um jogo em sessões colaborativas, onde os usuários possam gerar, avaliar e selecionar nomes por meio de categorias, estalos criativos e critérios pré-definidos. |

### 2.1. Oportunidade de Negócio

A definição de um nome para uma marca, produto ou sistema é uma etapa essencial, pois representa diretamente sua identidade e posicionamento. Foi desenvolvida no IFRN uma técnica de criação de nomes baseada em dinâmica de grupo, que utiliza categorias, geração de ideias e critérios de avaliação para refinar opções até chegar ao nome ideal.
No entanto, o processo atualmente é manual, o que pode gerar desorganização, perda de ideias, dificuldade de controle das etapas e menor engajamento dos participantes.
Dessa forma, surge a oportunidade de desenvolver um sistema que estruture e automatize a aplicação da técnica, torne o processo mais dinâmico e permita a execução simultânea por diferentes equipes.

### 2.2. Objetivos de Negócio

| NÚMERO | DESCRIÇÃO                                                                                                                |
| ------ | ------------------------------------------------------------------------------------------------------------------------ |
| ON-1   | Disponibilizar um sistema em formato de jogo para criação de nomes, seguindo fielmente as etapas definidas pela técnica. |
| ON-2   | Permitir a personalização das sessões (tempo, quantidade de opções e regras de eliminação).                              |
| ON-3   | Apresentar de forma clara e guiada todas as etapas da dinâmica para os participantes.                                    |

### 2.3. Riscos de Negócio

| NÚMERO | DESCRIÇÃO                                                                                     | PROBABILIDADE (0 a 10) | IMPACTO (1 a 10) |
| ------ | --------------------------------------------------------------------------------------------- | :--------------------: | :--------------: |
| RIS-1  | Interface não intuitiva, dificultando a compreensão da técnica pelos usuários                 |            6           |        9         |
| RIS-2  | A equipe não chegar em um resultado satisfatório                                              |            8           |        5         |
| RIS-3  | Falhas na contagem de votos ou regras de eliminação, comprometendo a credibilidade do sistema |            4           |        7         |

---

## 3. Usuários

### 3.1. Descrição dos Usuários

| NOME | DESCRIÇÃO | RESPONSABILIDADE |
| :--- | :--- | :--- |
| **Mestre da Sessão (Facilitador)** | Usuário responsável por organizar e conduzir a dinâmica, assumindo o papel de liderança na plataforma digital. | Criar a sessão; configurar os parâmetros iniciais (tempo das rodadas, quantidade de opções, limites de exclusão e critérios); iniciar as fases do jogo e conduzir a equipe até a votação final. |
| **Jogador (Participante)** | Membros da equipe (designers, desenvolvedores, stakeholders) que colaboram na criação do nome. | Sugerir nomes ocultos por categoria; registrar "estalos criativos"; votar individualmente para manter ou excluir palavras; propor variações na fase MEIA e realizar a votação do nome vencedor. |

### 3.2. Descrição do Ambiente dos Usuários

- **Número de pessoas envolvidas**: Variável, mas idealmente planejado para equipes pequenas a médias (estimativa de 3 a 15 participantes por sessão) para garantir o dinamismo.
- **Duração de tarefas**: Sessões completas podem durar entre 1 e 2 horas, dependendo do tempo configurado pelo Mestre para cada rodada e do volume de palavras geradas.
- **Restrições ambientais**: Acesso via Web (navegadores de internet em desktops, notebooks ou dispositivos móveis) com necessidade de conexão à internet estável para sincronização do jogo em tempo real.
- **Plataformas utilizadas atualmente**: Processo manual com anotações em papel, quadros físicos, ou adaptações em ferramentas genéricas de texto e planilhas.
- **Princípios do ambiente**: Colaboração em tempo real, transparência (todos veem o mesmo quadro de votação), imparcialidade (sugestões ocultas na fase inicial), gamificação e interface limpa (foco nas palavras e no cronômetro).

### 3.3. Principais Necessidades dos Usuários

- **Automatização do fluxo**: Necessidade de um sistema que controle automaticamente o cronômetro, faça a contagem da regra de "50% + 1" nas votações e reponha palavras no quadro sem intervenção manual.
- **Organização e histórico de ideias**: Garantir que nenhuma ideia se perca, centralizando todas as sugestões (incluindo os "estalos criativos") em uma nuvem de palavras acessível pelo sistema.
- **Estruturação visual do método MEIA**: Facilidade para visualizar as transformações dos nomes (Manter, Eliminar, Incrementar e Ajuntar) de forma intuitiva antes da decisão final.
- **Imparcialidade na ideação**: Necessidade de que as sugestões da fase de categorias sejam ocultas no momento da criação, evitando que a ideia de um participante influencie a do outro.

---

## 4. Requisitos

### 4.1. Requisitos Funcionais (RF)

| CÓDIGO | NOME                           | DESCRIÇÃO                                                                                                                                                                                                     | GRAVIDADE |
| ------ | ------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------- |
| RF01   | Criar sessão                   | O sistema deve permitir que uma equipe configure uma sessão, definindo parâmetros como tempo das rodadas, quantidade de opções exibidas, número mínimo de palavras, quantidade de opções para a fase MEIA e regras de critérios de avaliação. | Alta      |
| RF02   | Adicionar estalos criativos    | O sistema deve permitir que participantes adicionem novas ideias espontaneamente durante as fases iniciais e intermediárias, integrando essas sugestões à nuvem de palavras.                                | Média     |
| RF03   | Criar por categorias           | O sistema deve conduzir a fase de geração de nomes por categorias sorteadas, permitindo que cada participante insira sugestões de forma individual e oculta dentro do tempo definido.                         | Alta      |
| RF04   | Realizar exclusão coletiva     | O sistema deve apresentar quadros de palavras iguais para todos os participantes, permitindo votação individual (manter ou excluir), aplicando a regra de eliminação por maioria (50% + 1) e repondo automaticamente novas palavras da nuvem. | Alta      |
| RF05   | Aplicar critérios de avaliação | O sistema deve permitir a avaliação dos nomes com base em critérios definidos (sonoridade, escrita, disponibilidade, etc.), eliminando nomes conforme o limite de critérios violados estabelecido.            | Alta      |
| RF06   | Executar fase MEIA             | O sistema deve permitir a criação de variações dos nomes restantes por meio das etapas de manter, eliminar, incrementar e ajuntar, registrando todas as sugestões geradas.                                  | Média     |
| RF07   | Realizar votação final         | O sistema deve apresentar os nomes finais para votação, permitindo que os participantes escolham o nome vencedor por maioria.                                                                                 | Alta      |
| RF08   | Exibir nuvem de palavras       | O sistema deve consolidar e exibir todas as palavras sugeridas ao longo da dinâmica, garantindo sua utilização nas fases seguintes.                                                                           | Média     |
| RF09   | Controlar tempo das rodadas    | O sistema deve gerenciar automaticamente o tempo de cada fase, encerrando rodadas conforme definido na sessão.                                                                                                | Alta      |

### 4.2. Requisitos Não Funcionais (RNF)

| CÓDIGO | NOME              | DESCRIÇÃO                                                                                                                                                             | GRAVIDADE |
| ------ | ----------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------- |
| RNF 01 | Desempenho e Sincronização | O sistema deve suportar a sincronização em tempo real das interações (votos, cronômetro e reposição de palavras) entre todos os usuários de uma sessão, sem atrasos perceptíveis. | Alta      |
| RNF 02 | Usabilidade e Responsividade | A interface do sistema deve ser responsiva, garantindo legibilidade e facilidade de interação tanto em navegadores desktop quanto em dispositivos móveis (smartphones e tablets). | Alta      |
| RNF 03 | Segurança e Controle de Acesso | O acesso às sessões colaborativas deve ser restrito a participantes autorizados mediante link de convite único ou código da sala, prevenindo interações não autorizadas. | Alta      |
| RNF 04 | Disponibilidade e Persistência | O sistema deve salvar automaticamente o estado da sessão (palavras sugeridas, resultados parciais e configurações) para evitar perda de dados em caso de queda de conexão. | Alta      |
| RNF 05 | Escalabilidade | A arquitetura deve permitir múltiplas sessões (salas) ocorrendo simultaneamente sem degradação do desempenho do servidor. | Média |
