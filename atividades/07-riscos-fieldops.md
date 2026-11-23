# Aula 07 - Análise de Riscos do Projeto FieldOps

## 1. Método

O risco é descrito por causa, evento e consequência. A probabilidade e o impacto recebem notas de 1 a 5. A exposição é calculada por `P x I`.

| Faixa | Interpretação | Tratamento |
|---:|---|---|
| 1 a 4 | Baixa | Monitorar no ciclo regular |
| 5 a 9 | Média | Definir responsável e ação preventiva |
| 10 a 15 | Alta | Acompanhar semanalmente e preparar contingência |
| 16 a 25 | Crítica | Tratar como prioridade de gestão e escalar |

## 2. Registro e análise qualitativa

| ID | Causa | Risco (evento) | Consequência | P | I | Exposição | Nível | Dono |
|---|---|---|---|---:|---:|---:|---|---|
| R01 | Sinal instável e fila local incompleta | Registros offline podem não sincronizar | Perda de evidência e retrabalho no atendimento | 4 | 5 | 20 | Crítico | Tech lead |
| R02 | Usuários têm rotinas diferentes por região | Requisitos podem ficar incompletos ou ambíguos | Retrabalho, baixa adoção e atraso | 4 | 4 | 16 | Crítico | Product owner |
| R03 | Dependência de API externa | API pode ficar indisponível durante integração | Bloqueio de cadastro, mapas ou notificações | 3 | 4 | 12 | Alto | TI |
| R04 | Perfis e dados sensíveis mal configurados | Usuário pode acessar informação indevida | Incidente de segurança e impacto legal | 3 | 5 | 15 | Alto | Segurança |
| R05 | Usuários não participam do desenho | Equipe pode rejeitar o novo processo | Uso paralelo de planilhas e perda de benefício | 3 | 4 | 12 | Alto | Operações |
| R06 | Especialistas são compartilhados | Recurso-chave pode ficar sobrecarregado | Atraso em arquitetura, testes ou decisões | 4 | 4 | 16 | Crítico | Gerente |
| R07 | Cadastros legados incompletos | Dados podem ser importados com erro | Ordens, ativos ou indicadores incorretos | 3 | 4 | 12 | Alto | Dados / TI |
| R08 | Volume real maior que a carga testada | P95 pode superar 2 segundos | Baixa produtividade e rejeição do sistema | 3 | 4 | 12 | Alto | DevOps |
| R09 | Novas funções são solicitadas no piloto | Escopo pode crescer sem análise | Aumento de custo e atraso no release | 4 | 3 | 12 | Alto | Gerente |
| R10 | Diversidade de versões de dispositivos | Aplicativo pode falhar em aparelhos do piloto | Interrupção de atendimento em campo | 3 | 3 | 9 | Médio | Mobile |
| R11 | Agenda operacional muda no período do piloto | Usuários podem não estar disponíveis | Dados insuficientes para validar a solução | 3 | 3 | 9 | Médio | Operações |
| R12 | Treinamento é concentrado no fim | Usuários podem operar com erros | Mais chamados e registros inconsistentes | 3 | 3 | 9 | Médio | Product owner |
| R13 | Preço ou franquia de serviço externo varia | Custo de mapas, mensagens ou nuvem pode subir | Pressão sobre o orçamento | 2 | 3 | 6 | Médio | Gerente |
| R14 | Upload de evidência falha sem alerta | Fotos ou assinaturas podem não ser armazenadas | Ordem encerrada sem comprovação | 2 | 5 | 10 | Alto | QA |
| R15 | Revisão de segurança ocorre tarde | Achados podem exigir mudanças estruturais | Atraso na aprovação do release | 2 | 4 | 8 | Médio | Segurança |

## 3. Respostas planejadas

| ID | Estratégia | Ação preventiva | Gatilho | Contingência |
|---|---|---|---|---|
| R01 | Mitigar | Fila persistente, idempotência, conflitos e testes em campo | Taxa de sincronização < 95% | Bloquear encerramento offline sem confirmação e acionar procedimento manual |
| R02 | Mitigar | Entrevistas por perfil, protótipo e aceite de requisitos | Mais de 10% dos requisitos reabertos | Repriorizar MVP e reservar ciclo de ajuste |
| R03 | Mitigar | Mocks, timeout, retentativa e contrato versionado | Indisponibilidade > 30 min | Usar fila e processo manual até a API retornar |
| R04 | Evitar / mitigar | Menor privilégio, revisão de perfis, criptografia e pentest | Vulnerabilidade alta ou acesso indevido | Desativar integração afetada, corrigir e comunicar incidente |
| R05 | Mitigar | Usuários no desenho, demonstrações e treinamento no processo real | Participação < 80% | Replanejar piloto com representantes e ajustar fluxos |
| R06 | Mitigar | Planejamento de capacidade e decisões com prazo | Ocupação de especialista > 90% por duas semanas | Reordenar atividades e contratar apoio pontual |
| R07 | Mitigar | Perfilamento, validação e carga incremental | Mais de 2% de registros rejeitados | Suspender carga, corrigir origem e importar lote controlado |
| R08 | Mitigar | Teste de carga desde a versão integrada | P95 > 2 s | Otimizar consultas, aumentar capacidade ou reduzir escopo de indicadores |
| R09 | Controlar | Comitê de mudanças, critérios de aceite e backlog | Solicitação fora do baseline | Adiar para versão posterior ou aprovar impacto formalmente |
| R10 | Mitigar | Matriz de dispositivos e testes de compatibilidade | Falha em mais de 1 modelo crítico | Restringir dispositivos do piloto e publicar correção |
| R11 | Mitigar | Reservar janela de piloto e suplentes | Menos de 70% da escala prevista | Estender piloto ou substituir usuários mantendo rastreabilidade |
| R12 | Mitigar | Treinar em ondas, guias rápidos e simulações | Mais de 20% de erros repetidos | Reforço presencial e acompanhamento individual |
| R13 | Aceitar / controlar | Cotar consumo, alertas de franquia e contratos | Projeção > 90% da verba | Reduzir chamadas, negociar plano ou usar alternativa aprovada |
| R14 | Mitigar | Upload com confirmação, checksum e teste de reconexão | Evidência ausente em ordem encerrada | Reabrir ordem e executar procedimento de recuperação |
| R15 | Mitigar | Revisão de ameaças na arquitetura e segurança desde S8 | Revisão não concluída antes de S16 | Escalar decisão e postergar implantação até aceite mínimo |

## 4. Matriz probabilidade x impacto

| P \ I | 1 | 2 | 3 | 4 | 5 |
|---:|---:|---:|---:|---:|---:|
| 5 |  |  |  |  |  |
| 4 |  |  |  | R02, R06 | R01 |
| 3 |  |  | R10, R11, R12 | R03, R05, R07, R08 | R04 |
| 2 |  |  | R13 | R15 | R14 |
| 1 |  |  |  |  |  |

## 5. Monitoramento e comunicação

- revisão semanal no encontro do projeto;
- revisão extraordinária quando um gatilho ocorrer ou houver mudança de escopo;
- o dono do risco atualiza probabilidade, impacto, resposta, prazo e status;
- riscos críticos são comunicados ao patrocinador em até um dia útil;
- riscos encerrados permanecem no histórico para alimentar as lições aprendidas;
- riscos residuais do piloto são transferidos para o plano de operação e suporte.

## 6. Conclusão

Os riscos prioritários são sincronização offline, requisitos incompletos, sobrecarga de recursos, segurança de acesso e disponibilidade das integrações. A estratégia é tratar esses pontos antes do piloto e usar critérios objetivos de go/no-go, evitando que a primeira exposição aos problemas ocorra em produção.
