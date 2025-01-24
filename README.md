
# Automação de Infraestrutura com AWS - Projeto de TCC

Visão Geral

Este projeto foi desenvolvido como Trabalho de Conclusão de Curso (TCC) e tem como foco a automação de infraestrutura utilizando serviços da Amazon Web Services (AWS). O objetivo principal foi implementar uma arquitetura escalável, segura e automatizada que pudesse ser gerenciada com eficiência, aproveitando as melhores práticas de computação em nuvem.

Objetivos do Projeto

Automação: Reduzir o esforço manual e o tempo necessário para gerenciar a infraestrutura.

Escalabilidade: Garantir que o sistema possa lidar com variações de carga de trabalho.

Segurança: Implementar medidas de proteção de dados e acesso seguro.

Custo-benefício: Utilizar recursos da AWS de forma eficiente para reduzir custos.

Tecnologias e Serviços Utilizados

AWS Systems Manager: Para gerenciar e automatizar tarefas operacionais.

Amazon CloudWatch: Para monitoramento e geração de logs.

Auto Scaling: Para ajuste automático da capacidade de recursos.

Elastic Load Balancer (ELB): Para distribuir o tráfego de rede de forma eficiente.

AWS CloudFormation: Para provisionamento e gerenciamento da infraestrutura como código (IaC).

Amazon RDS MySQL: Para gerenciamento do banco de dados relacional.

Amazon S3: Para armazenamento de objetos e arquivos.

VPC Multi-AZ: Para criar uma infraestrutura de rede segura e de alta disponibilidade.

Arquitetura do Projeto

A arquitetura foi projetada para atender às melhores práticas recomendadas pela AWS, incluindo:

Alta Disponibilidade: Uso de múltiplas zonas de disponibilidade (AZs) para evitar pontos únicos de falha.

Segurança: Configuração de grupos de segurança e listas de controle de acesso (ACLs).

Automação: Scripts de CloudFormation e AWS Systems Manager para provisionamento e manutenção.

Estrutura do Repositório

├── cloudformation/       # Templates para provisionamento de infraestrutura
├── scripts/              # Scripts de automação e configuração
├── documentation/        # Documentação detalhada do projeto
├── diagrams/             # Diagramas de arquitetura
├── logs/                 # Logs de monitoramento (exemplo)
└── README.md             # Documentação principal

Configuração e Implantação

Clone este repositório:

git clone https://github.com/usuario/repo-automacao-infra.git

Configure as credenciais da AWS utilizando o AWS CLI:

aws configure

Execute os templates do CloudFormation para provisionar a infraestrutura:

aws cloudformation deploy --template-file cloudformation/main.yml --stack-name tcc-infra-stack

Use os scripts em scripts/ para tarefas adicionais de configuração e automação.

Monitoramento

O monitoramento da infraestrutura pode ser feito através do painel do Amazon CloudWatch. Dashboards personalizados foram configurados para acompanhar métricas críticas, como:

Utilização de CPU

Taxa de transferência de rede

Eventos de escalonamento

Resultados

Este projeto demonstrou os seguintes benefícios:

Redução do tempo de configuração em mais de 50%.

Melhoria na segurança com a implementação de políticas e monitoramento centralizado.

Alta disponibilidade garantida por meio da arquitetura Multi-AZ.

Contribuição

Contribuições são bem-vindas! Sinta-se à vontade para abrir issues ou enviar pull requests com melhorias ou correções.





