# zure-service-health-activity-log-lab
Laboratório prático de observabilidade e auditoria no Azure (AZ-900/AZ-104): Implementação de Action Groups reutilizáveis, alertas automatizados de Service Health e auditoria de ações administrativas via Activity Log.


# 🛡️ Azure Observability & Governance: Service Health & Activity Log Lab

Este repositório contém os registros e artefatos do laboratório prático focado em monitoramento de infraestrutura, auditoria do plano de controle e governança operacional no Microsoft Azure (preparatório para as certificações AZ-900 e AZ-104).

## 🎯 Objetivos do Laboratório
- Configurar canais reutilizáveis de notificação (**Action Groups**).
- Criar regras de alerta para incidentes globais e manutenções programadas da plataforma (**Azure Service Health**).
- Auditorar ações administrativas e criar alertas de exclusão de recursos (**Activity Log Alerts**).
- Inspecionar payloads JSON de auditoria no plano de controle do Azure Resource Manager (ARM).

## 🛠️ Recursos Provisionados
| Recurso | Tipo | Escopo | Função |
| :--- | :--- | :--- | :--- |
| `ag-gp-ops-email` | Action Group | Global | Envio automatizado de e-mails de alerta |
| `alert-gp-service-health` | Service Health Alert Rule | Subscription | Monitoramento de indisponibilidade/manutenção da Microsoft |
| `ar-gp-activity-log-delete` | Activity Log Alert Rule | Resource Group | Auditoria de exclusão de grupos de recursos (Event: Delete RG) |

## 💡 Principais Aprendizados (Certificação AZ-900 / AZ-104)
- **Gratuidade:** Alertas de *Service Health* e *Activity Log* são nativos e sem custo adicional na assinatura.
- **Plano de Controle vs. Plano de Dados:** O Activity Log registra alterações administrativas (criou/deletou recurso, alterou permissão IAM), retendo o histórico por 90 dias por padrão.
- **Service Health Layers:** Diferenciação entre *Azure Status* (público), *Service Health* (personalizado para a assinatura) e *Resource Health* (recurso individual).


<img width="1912" height="954" alt="Captura de tela 2026-11-07 100952" src="https://github.com/user-attachments/assets/061bdc97-7f89-4d9b-94be-85e9b8eeddd0" />
