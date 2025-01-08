# Descrição Técnica do Projeto de Portal Interno

## Visão Geral

O objetivo deste projeto é desenvolver um portal de atendimento interno para os funcionários de nossa empresa utilizando C# com Blazor. O portal permitirá a comunicação eficiente e organizada com diversas funcionalidades, incluindo uma central de notícias, cadastro de funcionários, registro e acompanhamento de chamados, quadro de aniversariantes, controle de ponto, atividades e status de transição, e chat em tempo real com log de mensagens. O sistema também incluirá autenticação segura para acesso autorizado, bem como uma ferramenta de logs para monitoramento de erros e eventos adversos.

## Funcionalidades Pretendidas

### 1. Autenticação

- **Objetivo:** Garantir que apenas usuários autorizados tenham acesso ao portal.
- **Requisitos Funcionais:**
  - Login seguro, recuperação de senha via e-mail, Single Sign-On (SSO), autenticação de dois fatores (2FA).
  - Criação de novos usuários, gerenciamento de perfis de acesso e autorização baseada em papéis (roles).

### 2. Portal de Notícias da Empresa

- **Objetivo:** Informar os funcionários sobre acontecimentos, novidades e comunicados importantes da empresa.
- **Requisitos Funcionais:**
  - Publicação de notícias com imagens, vídeos e anexos.
  - Categorização de notícias e sistema de busca e filtros.

### 3. Cadastro de Funcionários

- **Objetivo:** Manter um registro atualizado de todos os funcionários da empresa.
- **Requisitos Funcionais:**
  - Formulário de cadastro completo, função de edição e exclusão de cadastros.
  - Sistema de importação/exportação de dados.

### 4. Cadastro de Chamados Diversos

- **Objetivo:** Permitir que os funcionários registrem e acompanhem seus chamados.
- **Requisitos Funcionais:**
  - Registro de chamados com categoria, descrição detalhada.
  - Gerenciamento de chamados com atualização de status.
  - Notificações automáticas sobre mudança de status.

### 5. Quadro de Aniversariantes

- **Objetivo:** Manter um quadro atualizado com os aniversariantes do mês.
- **Requisitos Funcionais:**
  - Tela exibindo aniversariantes do mês.
  - Função de lembrança e envio automático de parabéns via e-mail.

### 6. Controle de Ponto

- **Objetivo:** Registrar e monitorar o horário de entrada e saída dos funcionários.
- **Requisitos Funcionais:**
  - Registro de ponto eletrônico, relatórios de frequência e pontualidade.
  - Relatório de ponto mensal, total de horas no banco de horas.
  - Recurso para justificativa de marcação sujeita a aprovação de um superior.

### 7. Atividades e Status de Transição

- **Objetivo:** Gerenciar e acompanhar o progresso das atividades dos funcionários.
- **Requisitos Funcionais:**
  - Interface para registro e acompanhamento de atividades.
  - Sistema de transição de status para atividades e relatório de progresso e produtividade.

### 8. Chat em Tempo Real

- **Objetivo:** Facilitar a comunicação interna entre os funcionários em tempo real.
- **Requisitos Funcionais:**
  - Interface de chat em tempo real, log de mensagens.
  - Notificações de novas mensagens, suporte a mensagens privadas e em grupo.

### 9. Ferramenta de Logs

- **Objetivo:** Monitorar erros e eventos adversos que ocorram no servidor.
- **Requisitos Funcionais:**
  - Log de todos os eventos e erros significativos.
  - Configuração para envio de e-mails de notificação de erros para a equipe de desenvolvimento e diretoria.

## Arquitetura do Sistema

O sistema será desenvolvido utilizando uma arquitetura em camadas, garantindo modularidade, manutenibilidade e escalabilidade. As camadas incluirão:

1. **Camada de Apresentação:** Interface de usuário responsiva e interativa desenvolvida com Blazor.
2. **Camada de Negócio:** Implementação das regras de negócio do sistema, utilizando C#.
3. **Camada de Dados:** Gerenciamento da persistência de dados utilizando PostgreSQL como sistema de banco de dados relacional, com acesso mediado por Entity Framework Core.
4. **Camada de Autenticação e Autorização:** Implementação segura de autenticação e autorização usando ASP.NET Identity.
5. **Camada de Comunicação em Tempo Real:** Implementação de SignalR para suporte a comunicação em tempo real.
6. **Camada de Monitoramento e Logs:** Implementação de uma ferramenta de logs para monitoramento de erros e eventos, configurada para enviar notificações por e-mail.

## Fluxo de Desenvolvimento

1. **Planejamento e Análise de Requisitos:** Coleta de requisitos e planejamento detalhado do sistema, envolvendo stakeholders para garantir a compreensão completa das necessidades.
2. **Design:** Criação de wireframes e protótipos de alta fidelidade para a interface do usuário, juntamente com o design da arquitetura do sistema.
3. **Desenvolvimento:** Implementação incremental das funcionalidades, seguindo metodologias ágeis como Scrum ou Kanban.
4. **Testes e Validação:** Testes de unidade, integração e sistema para garantir a qualidade do software.
5. **Implantação:** Implementação do sistema no ambiente de produção, com acompanhamento e suporte inicial.
6. **Manutenção e Suporte:** Monitoramento contínuo e fornecimento de suporte técnico para resolver quaisquer problemas que surgirem.
