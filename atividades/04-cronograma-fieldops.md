# Aula 04 - Cronograma do Projeto FieldOps

## 1. Identificação

| Campo | Informação |
|---|---|
| Projeto | FieldOps - Gestão de Operações em Campo |
| Gerente do projeto | Gerente de Projetos |
| Versão | 1.0 |
| Início de referência | Semana 1 após autorização |
| Término de referência | Semana 20 |
| Unidade de planejamento | Dias úteis e semanas do projeto |

As semanas são relativas à autorização do projeto para não vincular a atividade acadêmica a um calendário corporativo específico. O cronograma considera trabalho paralelo quando os predecessores permitem.

## 2. Lista de atividades

| ID | Atividade / entrega | Período | Duração | Responsável | Dependência |
|---|---|---:|---:|---|---|
| A01 | Confirmar patrocinador e caso de negócio | S1 | 2 d | Sponsor | - |
| A02 | Designar gerente do projeto | S1 | 1 d | Sponsor | A01 |
| A03 | Realizar kickoff | S1 | 1 d | Gerente do projeto | A02 |
| A04 | Identificar partes interessadas | S1 | 3 d | Gerente do projeto | A03 |
| A05 | Aprovar termo de abertura | S2 | 2 d | Sponsor | A04 |
| A06 | Consolidar baseline de planejamento | S2 | 5 d | Gerente do projeto | A05 |
| A07 | Conduzir entrevistas de descoberta | S2-S3 | 5 d | Analista de negócio | A03 |
| A08 | Mapear processo atual e futuro | S3 | 4 d | Analista de negócio | A07 |
| A09 | Especificar requisitos funcionais | S3-S4 | 5 d | Analista de negócio | A07 |
| A10 | Especificar requisitos não funcionais | S4 | 3 d | Tech lead | A09 |
| A11 | Levantar fontes e integrações | S4 | 4 d | Arquiteto / TI | A08 |
| A12 | Priorizar backlog do MVP | S5 | 3 d | Product owner | A09, A10, A11 |
| A13 | Validar requisitos com Operações | S5 | 2 d | Product owner | A12 |
| A14 | Aprovar baseline de requisitos | S5 | 1 d | Coordenação de Operações | A13 |
| A15 | Definir arquitetura de experiência | S6 | 4 d | UX designer | A14 |
| A16 | Produzir wireframes web e móvel | S6-S7 | 5 d | UX designer | A15 |
| A17 | Conduzir revisão de usabilidade | S8 | 3 d | UX designer | A16 |
| A18 | Definir arquitetura técnica | S6-S7 | 5 d | Tech lead | A14 |
| A19 | Modelar dados do produto | S8 | 4 d | Tech lead | A18 |
| A20 | Definir contratos de API | S8 | 4 d | Tech lead | A18 |
| A21 | Definir segurança e privacidade | S8 | 4 d | Segurança | A18 |
| A22 | Aprovar pacote de design e arquitetura | S9 | 1 d | Tech lead / Operações | A17, A19, A20, A21 |
| A23 | Configurar repositório e CI | S9 | 2 d | DevOps | A22 |
| A24 | Configurar ambientes de desenvolvimento e testes | S10 | 3 d | DevOps | A23 |
| A25 | Implementar autenticação e perfis | S10-S11 | 5 d | Backend | A20, A24 |
| A26 | Implementar ordens de serviço | S11-S12 | 8 d | Backend / Frontend | A25 |
| A27 | Implementar agenda e despacho | S13-S14 | 8 d | Frontend | A26 |
| A28 | Implementar aplicativo móvel base | S11-S13 | 10 d | Mobile | A25 |
| A29 | Implementar sincronização offline | S14 | 7 d | Mobile / Backend | A28 |
| A30 | Implementar inventário e ativos | S13-S14 | 7 d | Backend / Frontend | A26 |
| A31 | Implementar evidências e assinatura | S14 | 5 d | Mobile | A28 |
| A32 | Implementar notificações | S14 | 4 d | Backend | A26 |
| A33 | Implementar dashboard e indicadores | S14-S15 | 6 d | Frontend / Dados | A26, A30 |
| A34 | Implementar configurações administrativas | S13 | 4 d | Frontend | A25 |
| A35 | Desenvolver integrações autorizadas | S13-S15 | 8 d | Backend / TI | A20, A26 |
| A36 | Ajustar acessibilidade e responsividade | S15 | 4 d | UX / Frontend | A28, A33 |
| A37 | Consolidar versão integrada | S16 | 2 d | Tech lead | A27, A29, A31, A32, A33, A34, A35, A36 |
| A38 | Elaborar plano e casos de teste | S10 | 4 d | QA | A22 |
| A39 | Executar testes unitários | S11-S12 | 8 d | Desenvolvimento | A25 |
| A40 | Executar testes de integração | S16 | 5 d | QA | A37, A38 |
| A41 | Executar testes de segurança | S16 | 4 d | Segurança | A37, A38 |
| A42 | Executar testes de desempenho | S16 | 4 d | QA / DevOps | A37, A38 |
| A43 | Executar testes de usabilidade e aceite | S16 | 4 d | QA / Operações | A37 |
| A44 | Corrigir defeitos do ciclo integrado | S17 | 7 d | Desenvolvimento | A40, A41, A42, A43 |
| A45 | Executar regressão | S18 | 4 d | QA | A44 |
| A46 | Aprovar release candidate | S18 | 1 d | QA / Operações | A45 |
| A47 | Produzir materiais de treinamento | S16-S17 | 4 d | Analista de negócio | A37 |
| A48 | Preparar usuários e ambiente-piloto | S18 | 2 d | Operações / Suporte | A46, A47 |
| A49 | Executar piloto controlado | S19 | 5 d | Operações | A48 |
| A50 | Coletar feedback do piloto | S19 | 2 d | Product owner | A49 |
| A51 | Implementar ajustes do piloto | S19 | 5 d | Desenvolvimento | A50 |
| A52 | Realizar decisão go/no-go | S19 | 1 d | Sponsor / Operações | A51 |
| A53 | Publicar em produção | S20 | 2 d | DevOps | A52 |
| A54 | Realizar handover e hiper cuidado | S20 | 3 d | Suporte / Tech lead | A53 |
| A55 | Consolidar lições aprendidas | S20 | 2 d | Gerente do projeto | A54 |
| A56 | Obter aceite final e encerrar | S20 | 1 d | Sponsor / Gerente | A55 |

## 3. Marcos

| Marco | ID de referência | Semana | Critério |
|---|---|---:|---|
| TAP aprovado | A05 | S2 | Objetivo, escopo inicial, premissas e autoridade aceitos |
| Requisitos aprovados | A14 | S5 | Backlog e requisitos não funcionais validados |
| Design e arquitetura aprovados | A22 | S9 | Fluxos, modelo, APIs e segurança revisados |
| Versão integrada pronta | A37 | S16 | Módulos do MVP integrados em ambiente de testes |
| Release candidate aprovado | A46 | S18 | Testes concluídos e defeitos críticos zerados |
| Go/no-go do piloto | A52 | S19 | Feedback analisado e decisão registrada |
| Aceite final | A56 | S20 | Entrega aceita e transição concluída |

## 4. Dependências críticas

```text
A05 TAP aprovado
  -> A14 Requisitos aprovados
    -> A22 Design e arquitetura aprovados
      -> A37 Versão integrada
        -> A46 Release candidate
          -> A52 Go/no-go
            -> A53 Publicação
              -> A56 Aceite final
```

As frentes de desenvolvimento web, móvel, integrações e testes unitários podem ocorrer em paralelo após suas entradas. A versão integrada é o ponto de convergência para os testes sistêmicos.

## 5. Responsáveis por frente

| Frente | IDs principais | Responsável |
|---|---|---|
| Integração e governança | A01-A06, A55-A56 | Gerente do projeto |
| Requisitos e produto | A07-A14, A47, A50 | Analista de negócio / Product owner |
| Experiência e arquitetura | A15-A22 | UX designer / Tech lead |
| Construção | A23-A37, A51, A53 | Desenvolvimento / DevOps |
| Qualidade | A38-A46 | QA / Segurança |
| Piloto e operação | A48-A54 | Operações / Suporte |

## 6. Acompanhamento

O gerente atualizará semanalmente o percentual concluído, as datas reais, o caminho crítico, os bloqueios e a previsão de término. Qualquer desvio superior a cinco dias úteis ou que afete A37, A46 ou A52 deverá ser registrado como questão e submetido à avaliação de mudança.

| Indicador | Meta |
|---|---:|
| Atividades concluídas no período | >= 90% do planejado |
| Marcos sem atraso | 100% |
| Ações bloqueadas por mais de dois dias | 0 |
| Mudanças sem análise de impacto | 0 |
