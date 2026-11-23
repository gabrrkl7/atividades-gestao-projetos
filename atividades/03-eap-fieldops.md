# Aula 03 - EAP do Projeto FieldOps

## 1. Identificação

| Campo | Informação |
|---|---|
| Projeto | FieldOps - Gestão de Operações em Campo |
| Gerente do projeto | Gerente de Projetos |
| Data | 23/11/2026 |
| Versão | 1.0 |

## 2. Estrutura Analítica do Projeto

```text
0. FIELDOPS - GESTÃO DE OPERAÇÕES EM CAMPO
│
├── 1. Gestão e iniciação
│   ├── 1.1 Termo de abertura aprovado
│   ├── 1.2 Plano integrado do projeto
│   ├── 1.3 Registro de partes interessadas
│   └── 1.4 Governança e controle de mudanças
│
├── 2. Descoberta e requisitos
│   ├── 2.1 Mapa do processo de atendimento
│   ├── 2.2 Requisitos funcionais priorizados
│   ├── 2.3 Requisitos não funcionais
│   ├── 2.4 Regras de negócio e indicadores
│   └── 2.5 Baseline de requisitos aprovada
│
├── 3. Experiência e arquitetura
│   ├── 3.1 Arquitetura da solução
│   ├── 3.2 Protótipo web e móvel
│   ├── 3.3 Modelo de dados
│   ├── 3.4 Contratos de API
│   ├── 3.5 Projeto de segurança e privacidade
│   └── 3.6 Pacote de design aprovado
│
├── 4. Produto FieldOps
│   ├── 4.1 Ambientes e integração contínua
│   ├── 4.2 Autenticação e perfis
│   ├── 4.3 Ordens de serviço e agenda
│   ├── 4.4 Aplicativo móvel e modo offline
│   ├── 4.5 Evidências e assinatura
│   ├── 4.6 Inventário e ativos
│   ├── 4.7 Notificações e integrações
│   ├── 4.8 Dashboard e indicadores
│   └── 4.9 Versão integrada do produto
│
├── 5. Qualidade e validação
│   ├── 5.1 Plano e casos de teste
│   ├── 5.2 Testes unitários e de integração
│   ├── 5.3 Testes de segurança e desempenho
│   ├── 5.4 Testes de usabilidade e aceite
│   ├── 5.5 Correção e regressão
│   └── 5.6 Release candidate aprovado
│
├── 6. Piloto e implantação
│   ├── 6.1 Materiais de treinamento
│   ├── 6.2 Usuários e ambiente-piloto preparados
│   ├── 6.3 Piloto executado
│   ├── 6.4 Feedback e ajustes do piloto
│   ├── 6.5 Implantação assistida
│   └── 6.6 Aceite final e transição para suporte
│
└── 7. Encerramento
    ├── 7.1 Documentação final
    ├── 7.2 Lições aprendidas
    ├── 7.3 Relatório de resultados
    └── 7.4 Encerramento administrativo
```

## 3. Dicionário da EAP

| Código | Elemento | Descrição e critério de conclusão |
|---|---|---|
| 1.1 | Termo de abertura aprovado | TAP com objetivo, escopo inicial, patrocinador e premissas aceitos |
| 1.2 | Plano integrado | Planos de escopo, prazo, custo, qualidade, recursos, comunicação e riscos consolidados |
| 1.3 | Registro de partes interessadas | Pessoas e grupos identificados, com poder, interesse e estratégia |
| 1.4 | Governança e mudanças | Fluxo de decisão, reuniões, registros e formulário de mudança definidos |
| 2.1 | Mapa do processo | Fluxo atual e fluxo futuro de abertura, despacho e encerramento documentados |
| 2.2 | Requisitos funcionais | Funções priorizadas e rastreáveis ao objetivo do projeto |
| 2.3 | Requisitos não funcionais | Desempenho, segurança, disponibilidade, acessibilidade e usabilidade definidos |
| 2.4 | Regras e indicadores | Fórmulas, fontes, periodicidade e responsáveis documentados |
| 2.5 | Baseline de requisitos | Escopo validado pelo cliente e controlado para mudanças |
| 3.1 | Arquitetura | Componentes, integrações, ambientes e decisões técnicas registradas |
| 3.2 | Protótipo | Fluxos web e móvel principais demonstrados e revisados por usuários |
| 3.3 | Modelo de dados | Entidades, relacionamentos, regras e dicionário revisados |
| 3.4 | Contratos de API | Entradas, saídas, erros, autenticação e versionamento definidos |
| 3.5 | Segurança e privacidade | Perfis, logs, retenção, proteção e ameaças analisados |
| 3.6 | Design aprovado | Pacote de experiência e arquitetura aprovado para construção |
| 4.1 | Ambientes e CI | Repositório, automação de build, testes e ambientes configurados |
| 4.2 | Autenticação e perfis | Login, autorização por papel e auditoria de acesso funcionando |
| 4.3 | Ordens e agenda | Criar, priorizar, atribuir, reagendar e encerrar ordens funcionando |
| 4.4 | Móvel e offline | Aplicativo consulta e atualiza dados sem conexão e sincroniza depois |
| 4.5 | Evidências | Fotos, assinatura, observações e anexos validados e rastreáveis |
| 4.6 | Inventário e ativos | Materiais consumidos e ativos relacionados ao serviço controlados |
| 4.7 | Notificações e integrações | Eventos e integrações autorizadas testados e documentados |
| 4.8 | Dashboard | Indicadores de backlog, prazo, produtividade e retrabalho disponíveis |
| 4.9 | Produto integrado | Módulos integrados em uma versão candidata a testes sistêmicos |
| 5.1 | Plano de testes | Estratégia, casos, dados, critérios de entrada e saída definidos |
| 5.2 | Testes de software | Testes unitários e de integração executados com evidências |
| 5.3 | Segurança e desempenho | Vulnerabilidades críticas tratadas e metas de desempenho verificadas |
| 5.4 | Usabilidade e aceite | Usuários-piloto executam cenários e registram aceite ou pendências |
| 5.5 | Correção e regressão | Defeitos priorizados corrigidos e não regressivos |
| 5.6 | Release candidate | Versão atende aos critérios de qualidade e pode ir ao piloto |
| 6.1 | Treinamento | Manual, roteiro, vídeos ou guias rápidos produzidos |
| 6.2 | Preparação do piloto | Usuários, dados, acessos, dispositivos e suporte inicial preparados |
| 6.3 | Piloto | Operação real controlada executada e métricas coletadas |
| 6.4 | Feedback e ajustes | Feedback analisado, correções priorizadas e versão ajustada |
| 6.5 | Implantação assistida | Versão publicada no ambiente definido com plano de suporte |
| 6.6 | Aceite e transição | Cliente aceita a entrega e suporte recebe documentação e acessos |
| 7.1 | Documentação final | Manuais, arquitetura, operação, testes e decisões consolidados |
| 7.2 | Lições aprendidas | Resultados, problemas e recomendações registrados com o grupo |
| 7.3 | Relatório de resultados | Metas, indicadores do piloto e desvios comparados ao planejado |
| 7.4 | Encerramento | Pendências, contratos, acessos, repositório e aceite administrativo concluídos |

## 4. Requisitos rastreados na EAP

| Requisito | Pacote da EAP |
|---|---|
| Autenticação e perfis | 4.2 |
| Ordens e agenda | 4.3 |
| Operação offline | 4.4 |
| Evidências de atendimento | 4.5 |
| Inventário e ativos | 4.6 |
| Indicadores | 2.4 e 4.8 |
| Segurança e auditoria | 3.5, 4.2 e 5.3 |
| Treinamento e piloto | 6.1 a 6.4 |

## 5. Critério de completude

A EAP será considerada completa quando todas as entregas do TAP estiverem representadas, cada pacote tiver critério de aceite e não houver trabalho necessário para o objetivo do projeto fora da estrutura ou formalmente registrado como exclusão.
