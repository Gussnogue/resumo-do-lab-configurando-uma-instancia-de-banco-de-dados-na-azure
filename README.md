# resumo-do-lab-configurando-uma-instancia-de-banco-de-dados-na-azure
Este repositório contém o resumo das lições aprendidas durante o desenvolvimento do lab na DIO referente à configuração de uma instancia de banco de dados na Azure

##resumo

Para criar uma Instância Gerenciada do SQL no Azure, é preciso ter assinatura ativa, permissões adequadas e planejar uma rede virtual com sub-rede dedicada (/27 ou maior, mínimo 32 IPs). No portal, acesse o Hub SQL e selecione Criar Instância Gerenciada. Preencha assinatura, grupo de recursos, nome, região, método de autenticação (SQL ou Microsoft Entra ID), usuário e senha. Configure computação e armazenamento (camada Uso Geral, Gen5, vCores, redundância de backup). Defina rede com sub-rede dedicada e revise regras de segurança, mantendo o ponto público desabilitado em produção. Opcionalmente ajuste fuso horário, replicação geográfica e tags. Revise e crie, monitorando pelo painel de notificações. O provisionamento pode levar tempo. Após concluído, crie bancos de dados, obtenha o FQDN da instância e conecte-se via SSMS, Azure Data Studio, Bastion ou VPN/ExpressRoute. Essa abordagem garante escalabilidade, segurança e integração com sua infraestrutura existente.

Fonte: [https://learn.microsoft.com/pt-br/azure/azure-sql/managed-instance/instance-create-quickstart?view=azuresql&tabs=azure-portal](https://learn.microsoft.com/pt-br/azure/azure-sql/managed-instance/instance-create-quickstart?view=azuresql&tabs=azure-portal)

