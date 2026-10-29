# Estratégia de Arquitetura AWS

## 1. Objetivo
Definir uma estratégia de arquitetura em nuvem que seja segura, escalável, resiliente, eficiente em custo e fácil de operar, alinhada aos objetivos de negócio.

## 2. Princípios norteadores
- **Business first**: decisões técnicas devem responder a metas de negócio (tempo de entrega, disponibilidade, custo e risco).
- **Well-Architected by design**: aplicar os pilares do AWS Well-Architected Framework desde o início.
- **Automação sempre que possível**: usar infraestrutura como código, pipelines e políticas automatizadas.
- **Evolução incremental**: priorizar entregas pequenas, mensuráveis e reversíveis.
- **Segurança em camadas**: proteção em identidade, rede, dados, aplicações e observabilidade.

## 3. Pilares de decisão (AWS Well-Architected)
1. **Excelência Operacional**: monitoramento, runbooks, automação de resposta e melhoria contínua.
2. **Segurança**: menor privilégio, criptografia, trilhas de auditoria e detecção de ameaças.
3. **Confiabilidade**: tolerância a falhas, recuperação e testes de resiliência.
4. **Eficiência de Performance**: escolha correta de serviços, dimensionamento e otimização contínua.
5. **Otimização de Custos**: visibilidade financeira, rightsizing e uso de pricing models adequados.
6. **Sustentabilidade**: uso eficiente de recursos e redução de desperdício computacional.

## 4. Processo estratégico (ciclo contínuo)
### Etapa 1: Descoberta e contexto
- Mapear objetivos de negócio e requisitos não funcionais.
- Definir SLAs/SLOs (disponibilidade, latência, RTO/RPO).
- Classificar dados por criticidade e sensibilidade.

### Etapa 2: Arquitetura alvo
- Definir arquitetura de referência por domínio (web, dados, integração, segurança).
- Escolher padrão de implantação (multi-tier, serverless, containers ou híbrido).
- Definir estratégia de contas e governança (AWS Organizations, SCPs, tagging).

### Etapa 3: Segurança e conformidade
- Implementar IAM com papéis e políticas de menor privilégio.
- Habilitar logging e auditoria centralizados (CloudTrail, Config, Security Hub).
- Definir baseline de criptografia (em trânsito e em repouso) e gestão de chaves.

### Etapa 4: Resiliência e continuidade
- Planejar alta disponibilidade entre AZs e, quando necessário, entre regiões.
- Definir estratégia de backup e disaster recovery (backup/restore, pilot light, warm standby, active-active).
- Testar falhas periodicamente com cenários reais.

### Etapa 5: Eficiência e custos
- Estabelecer budgets, alertas e metas de custo por produto/time.
- Aplicar rightsizing e políticas de desligamento para ambientes não produtivos.
- Avaliar uso de Savings Plans/Reserved Instances para cargas previsíveis.

### Etapa 6: Operação e melhoria contínua
- Definir indicadores operacionais e de negócio.
- Revisar arquitetura em ciclos (mensal/trimestral) com Well-Architected Reviews.
- Registrar lições aprendidas e ajustar padrões.

## 5. Modelo de governança
- **Comitê de arquitetura**: valida decisões de alto impacto.
- **Padrões reutilizáveis**: módulos IaC, templates e blueprints por tipo de carga.
- **Políticas obrigatórias**: tagging, backup, criptografia e logging.
- **Guardrails**: controles preventivos e detectivos com automação.

## 6. Roadmap sugerido (90 dias)
### 0-30 dias
- Inventário de workloads e riscos.
- Definição de padrões mínimos de segurança e observabilidade.
- Priorização de 1 a 2 workloads críticas para modernização.

### 31-60 dias
- Implementação de landing zone e guardrails.
- Migração/modernização piloto com métricas de sucesso.
- Dashboards de custo, disponibilidade e segurança.

### 61-90 dias
- Expansão do padrão para novos times e aplicações.
- Otimização de custos e performance baseada em dados reais.
- Revisão executiva com plano de próximos 6-12 meses.

## 7. Checklist de validação
- [ ] Requisitos de negócio traduzidos em métricas técnicas.
- [ ] Controles de segurança implementados por padrão.
- [ ] Plano de DR testado e documentado.
- [ ] Custos monitorados com responsáveis definidos.
- [ ] Deploy automatizado e rastreável.
- [ ] Processo de revisão contínua ativo.

## 8. Resultado esperado
Uma arquitetura alinhada ao negócio, com riscos controlados, operação previsível e capacidade de escalar sem perda de governança ou explosão de custos.
