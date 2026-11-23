# Aula 02 - Termo de Abertura do Projeto (TAP)

## Projeto FieldOps

> **Nota de premissa:** como o PDF apresenta o nome FieldOps, mas não descreve o produto, este TAP usa o contexto documentado em [contexto/fieldops.md](../contexto/fieldops.md).

## 1. Identificação

| Campo | Definição |
|---|---|
| Projeto | FieldOps - Gestão de Operações em Campo |
| Patrocinador | Diretoria de Operações |
| Gerente do projeto | Gerente de Projetos |
| Cliente principal | Coordenação de Operações |
| Data-base | 23/11/2026 |
| Duração estimada | 20 semanas |
| Orçamento preliminar | R$ 742.000,00 |
| Versão | 1.0 |

## 2. Contexto e justificativa

Ordens de serviço são recebidas e distribuídas por canais diferentes. Técnicos e coordenadores possuem pouca visibilidade sobre prioridades, deslocamentos, materiais e evidências. O FieldOps centralizará o fluxo de atendimento e fornecerá dados para controlar prazo, produtividade e qualidade.

## 3. Objetivo do projeto

Entregar e colocar em piloto, em 20 semanas, uma solução web e móvel capaz de gerenciar ordens de serviço, agenda, equipes, evidências, inventário e indicadores, com operação offline e sincronização posterior.

## 4. Objetivos específicos

- reduzir o uso de planilhas e mensagens paralelas no despacho;
- permitir que técnicos atualizem atendimentos em campo;
- garantir rastreabilidade de status, usuário, horário e evidências;
- disponibilizar indicadores de backlog, prazo, produtividade e retrabalho;
- validar a solução com uma equipe-piloto antes da expansão.

## 5. Principais entregas

| Entrega | Critério de aceite |
|---|---|
| Plano e requisitos validados | Requisitos priorizados e aprovados por Operações |
| Protótipo de experiência | Fluxos principais revisados por usuários-piloto |
| Aplicação web | Ordens, agenda, usuários, inventário e indicadores funcionando |
| Aplicativo móvel | Consulta, atualização e registro de evidências online/offline |
| Integrações | APIs documentadas, autenticadas e testadas |
| Plano de qualidade | Casos, evidências, critérios e defeitos rastreados |
| Piloto e treinamento | Até 20 técnicos treinados e piloto executado |
| Implantação assistida | Versão aprovada, manual e transferência para suporte |

## 6. Requisitos iniciais

1. Autenticar usuários e aplicar perfis de acesso.
2. Criar, priorizar, atribuir e encerrar ordens de serviço.
3. Permitir agenda e acompanhamento do status.
4. Registrar fotos, assinatura, localização aproximada e observações.
5. Funcionar com conectividade intermitente e sincronizar alterações.
6. Controlar materiais e ativos utilizados no atendimento.
7. Disponibilizar indicadores de prazo, backlog, produtividade e retrabalho.
8. Registrar logs de auditoria para alterações críticas.
9. Atender aos critérios de qualidade definidos no plano do projeto.

## 7. Escopo e limites

O escopo inclui descoberta, desenho, desenvolvimento, testes, piloto, treinamento e implantação assistida de uma primeira versão. Ficam fora do escopo o faturamento, a substituição do ERP, a operação para todas as filiais, a roteirização avançada e o suporte 24x7 após o hiper cuidado.

## 8. Premissas

- Operações disponibilizará usuários para entrevistas e aceite;
- o piloto terá até 20 técnicos e duas áreas solicitantes;
- haverá cadastros mínimos de clientes, ativos, técnicos e serviços;
- a organização fornecerá ambientes de nuvem e acessos autorizados;
- os valores financeiros são estimativas acadêmicas de planejamento;
- mudanças relevantes serão analisadas pelo processo de controle integrado de mudanças.

## 9. Restrições

- prazo-base de 20 semanas;
- orçamento de linha de base de R$ 742.000,00;
- disponibilidade limitada de especialistas de Operações, Segurança e Qualidade;
- dependência de APIs externas e conectividade em campo;
- tratamento de dados sujeitos a requisitos de privacidade e segurança.

## 10. Riscos de alto nível

| Risco | Impacto inicial | Estratégia |
|---|---|---|
| Requisitos de campo incompletos | Retrabalho e baixa adoção | Entrevistas, protótipo e piloto antecipado |
| Conectividade insuficiente | Perda ou atraso de registros | Fila offline, sincronização e testes em campo |
| Integração indisponível | Bloqueio de fluxos | Contratos de API, mocks e plano manual temporário |
| Dados expostos | Impacto legal e reputacional | Menor privilégio, criptografia e testes de segurança |
| Sobrecarga de recursos-chave | Atrasos | Planejamento por capacidade e priorização do MVP |

## 11. Marcos principais

| Marco | Prazo relativo |
|---|---:|
| TAP aprovado | Semana 2 |
| Requisitos e escopo aprovados | Semana 5 |
| Design e arquitetura aprovados | Semana 8 |
| Versão integrada disponível | Semana 13 |
| Release candidate aprovado | Semana 17 |
| Piloto concluído | Semana 19 |
| Aceite final e encerramento | Semana 20 |

## 12. Partes interessadas principais

| Parte interessada | Papel / expectativa |
|---|---|
| Diretoria de Operações | Patrocínio, valor e decisões de prioridade |
| Coordenação de Operações | Cliente, processo e aceite funcional |
| Gerente de Projetos | Integração, planejamento e controle |
| Técnicos de campo | Uso diário, feedback e validação de usabilidade |
| Despachantes | Priorização e distribuição das ordens |
| TI e Segurança | Arquitetura, acessos, integração e conformidade |
| Qualidade | Critérios, testes e aceite técnico |
| Suporte | Operação assistida e sustentação |

## 13. Governança e autoridade

O gerente de projetos coordena o plano, o backlog, os riscos e as comunicações. A Coordenação de Operações aprova requisitos e aceite funcional. TI e Segurança aprovam arquitetura, acessos e integrações. Mudanças que afetem linha de base de prazo, custo ou escopo devem ser registradas e submetidas ao patrocinador.

## 14. Aprovação

Este TAP autoriza o planejamento detalhado do FieldOps e será considerado aprovado quando o patrocinador, o gerente do projeto e o cliente principal confirmarem os objetivos, entregas, restrições e premissas.
