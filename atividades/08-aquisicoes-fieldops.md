# Aula 08 - Gerenciamento das Aquisições do Projeto FieldOps

## 1. Premissas de contratação

- itens de nuvem, APIs e licenças serão contratados de provedores homologados;
- serviços de segurança e acessibilidade devem apresentar escopo, evidências e confidencialidade;
- equipamentos precisam ser compatíveis com o aplicativo e ter garantia durante o piloto;
- a contratação será iniciada somente após validação técnica e disponibilidade orçamentária;
- os valores são estimativas e devem ser confirmados por cotação antes do pedido.

## 2. Plano de aquisições

Escala de urgência: 1 = pode aguardar; 5 = bloqueia a próxima fase.

| ID | Item / serviço | Urgência | Motivo | Fornecedor provável | Qtd. | Valor unitário | Total | Responsável | Momento |
|---:|---|---:|---|---|---:|---:|---:|---|---|
| AQ01 | Ambiente de nuvem de desenvolvimento e testes | 5 | Necessário para começar a construção | Provedor de nuvem homologado | 5 mês | R$ 1.500,00 | R$ 7.500,00 | DevOps | S9 |
| AQ02 | Ambiente de nuvem de produção e piloto | 5 | Necessário para piloto e implantação | Provedor de nuvem homologado | 5 mês | R$ 3.500,00 | R$ 17.500,00 | DevOps | S16 |
| AQ03 | Banco de dados gerenciado | 5 | Persistência e backup dos registros | Provedor de nuvem homologado | 5 mês | R$ 1.000,00 | R$ 5.000,00 | DevOps | S10 |
| AQ04 | Monitoramento, logs e alertas | 4 | Rastreabilidade e resposta a incidentes | Provedor de observabilidade | 5 mês | R$ 600,00 | R$ 3.000,00 | DevOps | S10 |
| AQ05 | API de mapas e rotas | 3 | Apoiar localização e deslocamento | Provedor de mapas homologado | 20.000 chamadas | R$ 0,25 | R$ 5.000,00 | TI | S13 |
| AQ06 | Serviço de mensagens e notificações | 3 | Avisar mudanças de agenda e status | Provedor de mensagens | 5.000 un. | R$ 0,30 | R$ 1.500,00 | Product owner | S14 |
| AQ07 | Smartphones robustos para o piloto | 4 | Garantir aparelhos compatíveis em campo | Revenda homologada | 6 un. | R$ 2.500,00 | R$ 15.000,00 | Operações | S18 |
| AQ08 | Leitores de código de barras | 3 | Apoiar identificação de materiais e ativos | Revenda homologada | 4 un. | R$ 1.200,00 | R$ 4.800,00 | Operações | S18 |
| AQ09 | Licenças de gerenciamento de dispositivos | 4 | Controlar acesso e configuração dos aparelhos | Fornecedor de MDM | 30 mês-un. | R$ 100,00 | R$ 3.000,00 | Segurança | S18 |
| AQ10 | Consultoria de segurança | 4 | Revisar ameaças e apoiar conformidade | Consultoria especializada | 1 serviço | R$ 18.000,00 | R$ 18.000,00 | Segurança | S8 |
| AQ11 | Teste de intrusão externo | 4 | Evidenciar vulnerabilidades antes do release | Empresa de segurança independente | 1 serviço | R$ 15.000,00 | R$ 15.000,00 | Segurança | S16 |
| AQ12 | Auditoria de acessibilidade | 3 | Validar critérios de inclusão e uso | Consultoria de acessibilidade | 1 serviço | R$ 8.000,00 | R$ 8.000,00 | QA | S16 |
| AQ13 | Migração e saneamento de dados | 4 | Preparar dados para o piloto | Empresa de dados ou equipe interna | 1 serviço | R$ 12.000,00 | R$ 12.000,00 | Dados / TI | S13 |
| AQ14 | Workshops de treinamento | 4 | Preparar técnicos, despachantes e suporte | Instrutor / equipe interna | 4 turma | R$ 1.500,00 | R$ 6.000,00 | Operações | S18 |
| AQ15 | Hiper cuidado e suporte inicial | 3 | Reduzir risco na transição para operação | Equipe de suporte ou fornecedor | 1 pacote | R$ 30.000,00 | R$ 30.000,00 | Suporte | S20 |
|  | **Subtotal estimado de aquisições** |  |  |  |  |  | **R$ 151.300,00** |  |  |

## 3. Estratégia de aquisição

| Grupo | Estratégia | Critério de seleção |
|---|---|---|
| Nuvem, banco, observabilidade e APIs | Contrato com provedor homologado | Segurança, disponibilidade, preço por consumo e suporte |
| Equipamentos | Compra com garantia e teste de compatibilidade | Prazo, garantia, compatibilidade e custo total |
| Segurança e acessibilidade | Contratação por escopo fechado | Experiência, independência, evidências e confidencialidade |
| Dados e treinamento | Serviço ou execução interna comparada | Capacidade, prazo, conhecimento do processo e transferência |
| Hiper cuidado | Pacote com níveis de atendimento | Tempo de resposta, cobertura e documentação de transição |

## 4. Processo de contratação e controle

1. Confirmar necessidade, escopo e orçamento.
2. Elaborar especificação e critérios de aceite.
3. Solicitar cotações ou propostas a fornecedores elegíveis.
4. Avaliar técnica, segurança, prazo e custo total.
5. Registrar recomendação e aprovar a contratação.
6. Emitir pedido ou contrato e acompanhar entrega.
7. Inspecionar o item/serviço e registrar aceite.
8. Acompanhar consumo, desempenho, renovação e encerramento.

Nenhuma aquisição deverá usar dados pessoais ou acessos produtivos antes de contrato, autorização e controle de segurança. O responsável pelo item registra pedido, prazo, custo comprometido, aceite e pendências no controle financeiro do projeto.
