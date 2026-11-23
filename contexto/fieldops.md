# Premissas do Projeto FieldOps

## Contexto adotado

O FieldOps é tratado neste trabalho como uma solução web e móvel para gestão de operações em campo. A solução apoia o ciclo de atendimento desde a abertura da ordem de serviço até o encerramento, permitindo distribuir atividades, acompanhar equipes, registrar evidências e consultar indicadores.

## Problema

As solicitações são distribuídas por canais diferentes, o acompanhamento das equipes depende de planilhas e mensagens e as evidências do atendimento ficam dispersas. Isso dificulta priorização, rastreabilidade, medição de prazo e tomada de decisão.

## Objetivo do projeto

Entregar e colocar em piloto, em 20 semanas, uma solução que permita:

- cadastrar e priorizar ordens de serviço;
- alocar técnicos e acompanhar o status dos atendimentos;
- operar com conectividade intermitente no aplicativo móvel;
- registrar fotos, assinatura e observações como evidências;
- controlar ativos e materiais utilizados;
- apresentar indicadores de prazo, produtividade e backlog.

## Escopo incluído

- descoberta e validação dos processos de atendimento;
- protótipo de experiência e arquitetura da solução;
- aplicação web para coordenação e gestão;
- aplicativo móvel para técnicos;
- autenticação e perfis de acesso;
- ordens de serviço, agenda, evidências, inventário e notificações;
- integração com cadastro de clientes e ativos por API;
- testes, piloto controlado, treinamento e implantação assistida.

## Fora do escopo

- substituição do ERP corporativo;
- faturamento e emissão fiscal;
- roteirização avançada com otimização matemática;
- operação para todas as filiais no primeiro lançamento;
- compra de hardware de telemetria;
- suporte 24x7 após o período de hiper cuidado.

## Premissas

1. A área de Operações disponibilizará usuários para entrevistas e validação.
2. Existe cadastro mínimo de clientes, técnicos, ativos e tipos de serviço para carga inicial.
3. A organização fornecerá ambiente de nuvem e credenciais das integrações autorizadas.
4. O piloto ocorrerá com uma equipe de até 20 técnicos e duas áreas solicitantes.
5. Os dados do projeto são fictícios para fins acadêmicos e os valores são estimativas de planejamento.

## Restrições

- prazo-base de 20 semanas;
- equipe compartilhada entre análise, desenvolvimento, qualidade e segurança;
- orçamento estimado limitado à linha de base apresentada na atividade de custos;
- requisitos de privacidade e controle de acesso aplicáveis aos dados de clientes e colaboradores;
- dependência de conectividade e disponibilidade das APIs externas.

## Critérios de sucesso

| Indicador | Meta do piloto |
|---|---:|
| Ordens de serviço encerradas sem retrabalho de cadastro | >= 90% |
| Sincronização de registros offline em até 5 minutos após conexão | >= 95% |
| Usuários-piloto treinados | 100% |
| Disponibilidade do ambiente no piloto | >= 99% |
| Defeitos críticos abertos na entrada em produção | 0 |
| Satisfação dos usuários-piloto | >= 4,0/5,0 |
