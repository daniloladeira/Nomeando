# Documento de Visão e Escopo

## [NOME DO SISTEMA]

**Componentes:** - [Nome do Componente 1]

- [Nome do Componente 2]
- [Nome do Componente 3]
- [Nome do Componente 4]
- [Nome do Componente 5]

## Histórico de Revisões

|    Data    | Versão |              Descrição              |             Autores             |
| :--------: | :----: | :---------------------------------: | :-----------------------------: |
| 26/03/2026 |  1.0   |  Criação do esqueleto do documento  | Danilo Ladeira - @daniloladeira |
| 31/03/2026 |  1.1   | Definição dos requisitos funcionais |      Ana Maria - @namariaa      |

---

## 1. Requisitos de Negócio

### 1.1. Objetivo do Projeto

[Descreva aqui o objetivo geral do sistema, o que se pretende implantar e quais as metas principais da solução tecnológica.]

---

## 2. Descrição do Problema

|              |                                                                                                                                                                                                                     |
| ------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Problema** | Inexistência de uma plataforma digital que ofereça suporte à execução de uma técnica coletiva, desenvolvida no IFRN, para definição de nomes de marcas, produtos e sistemas.                                        |
| **Afeta**    | Designers, equipes de desenvolvimento e stakeholders envolvidos no processo de decisão de nomes.                                                                                                                    |
| **Impacta**  | Perda de tempo, dificuldade de organização das ideias e risco de escolha de nomes inadequados ao contexto, além da baixa participação da equipe na decisão.                                                         |
| **Solução**  | Criação de um sistema interativo, estruturado como um jogo em sessões colaborativas, onde os usuários possam gerar, avaliar e selecionar nomes por meio de categorias, estalos criativos e critérios pré-definidos. |

### 2.1. Oportunidade de Negócio

A definição de um nome para uma marca, produto ou sistema é uma etapa essencial, pois representa diretamente sua identidade e posicionamento. foi desenvolvida no IFRN uma técnica de criação de nomes baseada em dinâmica de grupo, que utiliza categorias, geração de ideias e critérios de avaliação para refinar opções até chegar ao nome ideal.
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
| RIS-1  | Interface não intuitiva, dificultando a compreensão da técnica pelos usuários                 |           6            |        9         |
| RIS-2  | A equipe não chegar em um resultado satisfatório                                              |           8            |        5         |
| RIS-3  | Falhas na contagem de votos ou regras de eliminação, comprometendo a credibilidade do sistema |           4            |        7         |

---

## 3. Usuários

### 3.1. Descrição dos Usuários

| NOME       | DESCRIÇÃO                   | RESPONSABILIDADE                      |
| ---------- | --------------------------- | ------------------------------------- |
| [Perfil 1] | [Quem é este usuário/cargo] | [O que ele faz no sistema/permissões] |
| [Perfil 2] | [Quem é este usuário/cargo] | [O que ele faz no sistema/permissões] |

### 3.2. Descrição do Ambiente dos Usuários

- **Número de pessoas envolvidas**: [Quantidade estimada de usuários]
- **Duração de tarefas**: [Tempo médio gasto nas funções principais do dia a dia]
- **Restrições ambientais**: [Onde será acessado? Ex: Web, Mobile, Servidor local, Nuvem?]
- **Plataformas utilizadas atualmente**: [Como o processo é feito hoje (planilhas, papel, outro software)?]
- **Princípios do ambiente**: [Ex: Padronização, Hierarquia, Acessibilidade, Simplicidade.]

### 3.3. Principais Necessidades dos Usuários

[O que os usuários esperam ganhar com o novo sistema?]

- [Necessidade 1]
- [Necessidade 2]
- [Necessidade 3]

---

## 4. Requisitos

### 4.1. Requisitos Funcionais (RF)

| CÓDIGO | NOME                           | DESCRIÇÃO                                                                                                                                                                                                                                     | GRAVIDADE |
| ------ | ------------------------------ | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------- |
| RF01   | Criar sessão                   | O sistema deve permitir que uma equipe configure uma sessão, definindo parâmetros como tempo das rodadas, quantidade de opções exibidas, número mínimo de palavras, quantidade de opções para a fase MEIA e regras de critérios de avaliação. | Alta      |
| RF02   | Adicionar estalos criativos    | O sistema deve permitir que participantes adicionem novas ideias espontaneamente durante as fases iniciais e intermediárias, integrando essas sugestões à nuvem de palavras.                                                                  | Média     |
| RF03   | Criar por categorias           | O sistema deve conduzir a fase de geração de nomes por categorias sorteadas, permitindo que cada participante insira sugestões de forma individual e oculta dentro do tempo definido.                                                         | Alta      |
| RF04   | Realizar exclusão coletiva     | O sistema deve apresentar quadros de palavras iguais para todos os participantes, permitindo votação individual (manter ou excluir), aplicando a regra de eliminação por maioria (50% + 1) e repondo automaticamente novas palavras da nuvem. | Alta      |
| RF05   | Aplicar critérios de avaliação | O sistema deve permitir a avaliação dos nomes com base em critérios definidos (sonoridade, escrita, disponibilidade, etc.), eliminando nomes conforme o limite de critérios violados estabelecido.                                            | Alta      |
| RF06   | Executar fase MEIA             | O sistema deve permitir a criação de variações dos nomes restantes por meio das etapas de manter, eliminar, incrementar e ajuntar, registrando todas as sugestões geradas.                                                                    | Média     |
| RF07   | Realizar votação final         | O sistema deve apresentar os nomes finais para votação, permitindo que os participantes escolham o nome vencedor por maioria.                                                                                                                 | Alta      |
| RF08   | Exibir nuvem de palavras       | O sistema deve consolidar e exibir todas as palavras sugeridas ao longo da dinâmica, garantindo sua utilização nas fases seguintes.                                                                                                           | Média     |
| RF09   | Controlar tempo das rodadas    | O sistema deve gerenciar automaticamente o tempo de cada fase, encerrando rodadas conforme definido na sessão.                                                                                                                                | Alta      |

### 4.2. Requisitos Não Funcionais (RNF)

| CÓDIGO | NOME              | DESCRIÇÃO                                           | GRAVIDADE          |
| ------ | ----------------- | --------------------------------------------------- | ------------------ |
| RNF 01 | [Ex: Segurança]   | [Restrição de acesso ou regra de proteção de dados] | [Alta/Média/Baixa] |
| RNF 02 | [Ex: Performance] | [Tempo de resposta ou capacidade do sistema]        | [Alta/Média/Baixa] |
| RNF 03 | [Ex: Usabilidade] | [Interface e facilidade de uso]                     | [Alta/Média/Baixa] |
