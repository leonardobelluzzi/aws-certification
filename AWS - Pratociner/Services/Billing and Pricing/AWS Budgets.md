# AWS Budgets

##  Visão Geral

[AWS Budgets](https://aws.amazon.com/aws-cost-management/aws-budgets/) gives you the ability to set custom budgets that alert you when your costs or usage exceed (or are forecasted to exceed) your budgeted amount.

You can also use AWS Budgets to set reservation utilization or coverage targets and receive alerts when your utilization drops below the threshold you define.

---

##  Tipos de Budget

###  Cost Budget
Helps you **plan how much you want to spend** on a service.

**Uso:** Monitorar gastos totais e receber alertas quando exceder limites definidos.

###  Usage Budget
Helps you **plan how much you want to use** one or more services.

**Uso:** Controlar quantidade de uso de recursos (ex: horas de EC2, GB de S3).

###  Reservation Budget
This helps you track the usage of your [Reserved Instances (RI)](Services%20support%20reservations%20to%20optimize%20costs.md).

**Dois tipos de monitoramento:**

1. **RI Utilization Budgets**
   - See if your Reserved Instances are **unused or under-utilized**
   - Identifica RIs que não estão sendo aproveitadas

2. **RI Coverage Budgets**
   - See how much of your **instance usage is covered** by a reservation
   - Mostra % de instâncias cobertas por reservas

---

##  Alertas e Notificações

AWS Budgets permite receber alertas quando:
-  Custos **excedem** o orçamento definido
-  Custos são **previstos para exceder** (forecast)
-  Utilização de RI **cai abaixo** do threshold
-  Coverage de RI está **abaixo do esperado**

---

##  Serviços com Suporte a Reservations

Reservation alerts são suportados para:
- [Amazon EC2](../../EC2.md)
- [Amazon RDS](../../Technology/Database/RDS.md)
- [Amazon Redshift](../../Amazon%20Redshift%20Reserved%20Nodes.md)
- Amazon ElastiCache
- Amazon Elasticsearch

---

##  Casos de Uso

###  Principais Use Cases

| Caso de Uso | Descrição |
|-------------|-----------|
| **Controle de Custos** | Receber alertas quando gastos excederem limite mensal |
| **Otimização de RIs** | Monitorar utilização de Reserved Instances |
| **Budget por Projeto** | Criar orçamentos separados para diferentes projetos/departamentos |
| **Forecast de Gastos** | Ser alertado sobre projeções de gastos futuros |
| **Monitoramento de Uso** | Acompanhar uso de recursos específicos (GB, horas, requests) |

###  Exemplo Prático

**Cenário:** Empresa quer controlar gastos com [EC2](../../EC2.md)

1. Criar **Cost Budget** de $5.000/mês
2. Configurar alerta em 80% ($4.000)
3. Criar **RI Utilization Budget** para garantir >75% de uso
4. Receber notificações via [SNS](../../Technology/Message/SNS%20-%20Amazon%20Simple%20Notification%20Service.md) ou email

---

##  Diferenças com Outros Serviços

| Serviço | Função |
|---------|--------|
| **AWS Budgets** | Alertas e limites de orçamento |
| [Cost Explorer](AWS%20Cost%20Explorer.md) | Análise visual de custos históricos |
| [Pricing Calculator](Pricing%20Calculator.md) | Estimativa de custos antes de provisionar |
| [Billing Dashboard](../../Billing%20&%20Cost%20Management/AWS%20Billing.md) | Visualização de faturas |

---

##  Pontos Importantes para Certificação

-  AWS Budgets permite **alertas proativos** sobre custos
-  Suporta **forecast** de gastos futuros
-  Pode monitorar **utilização de Reserved Instances**
-  Três tipos principais: **Cost, Usage e Reservation**
-  Integra com SNS para notificações automáticas
-  Gratuito para os primeiros 2 budgets

---

##  Serviços Relacionados

- [AWS Cost Explorer](AWS%20Cost%20Explorer.md) - Análise de custos
- [AWS Organizations](AWS%20Organization.md) - Consolidated billing
- [Reserved Instances](Services%20support%20reservations%20to%20optimize%20costs.md) - Otimização de custos
- [Amazon CloudWatch](../../CloudWatch.md) - Monitoramento de métricas

---

**Última atualização:** 26/12/2025


## USE CASES

Receive alerts when the reservation utilization falls below the defined threshold

## USE CASE

Which AWS service would you use to send alerts when the costs for your AWS account exceed your budgeted amount?

AWS Budgets

## USE CASE

Which budget types can be created under AWS Budgets (Select three)?

**Cost budget** - Helps you plan how much you want to spend on a service.
**Usage budget** - Helps you plan how much you want to use one or more services.
**Reservation budget** - This helps you track the usage of your Reserved Instances (RI). Two ways of doing it - Reserved Instance (RI) utilization budgets (This lets you see if your Reserved Instances (RI) are unused or under-utilized), Reserved Instance (RI) coverage budgets (This lets you see how much of your instance usage is covered by a reservation).


