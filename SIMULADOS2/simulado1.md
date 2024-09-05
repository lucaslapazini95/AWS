### Pergunta 1

**Incorreto**  
**Which of the following is a benefit of using AWS managed services such as Amazon Relational Database Service (Amazon RDS)?**

- **Sua resposta está incorreta:** The customer needs to patch the underlying OS
- The customer needs to manage database backups
- There is no need to optimize database instance type and size
- **Resposta correta:** The performance of AWS managed Amazon Relational Database Service (Amazon RDS) instance is better than a customer-managed database instance

**Explicação geral**  
**Correct option:**

**The performance of AWS managed Amazon Relational Database Service (Amazon RDS) instance is better than a customer-managed database instance**

O Amazon Relational Database Service (Amazon RDS) facilita a configuração, operação e escalabilidade de um banco de dados relacional na nuvem. Ele fornece capacidade redimensionável e econômica enquanto automatiza tarefas administrativas demoradas, como provisionamento de hardware, configuração de banco de dados, aplicação de patches e backups.

O Amazon RDS oferece uma seleção de tipos de instância otimizados para se adequar a diferentes casos de uso de bancos de dados relacionais. Os tipos de instância incluem combinações variadas de CPU, memória, armazenamento e capacidade de rede, proporcionando flexibilidade para escolher a combinação apropriada de recursos para seu banco de dados, otimizando-o para o seu caso de uso, selecionando o tipo e o tamanho de instância corretos.

Como as instâncias RDS são otimizadas para memória, desempenho ou E/S, o desempenho da instância do Amazon Relational Database Service (Amazon RDS) gerenciada pela AWS é melhor do que o de uma instância de banco de dados gerenciada pelo cliente.

**Incorrect options:**

- The customer needs to patch the underlying OS
- The customer needs to manage database backups
- There is no need to optimize database instance type and size

Essas três opções contradizem os detalhes fornecidos anteriormente na explicação, portanto, essas opções estão incorretas.

**Reference:**  
[https://aws.amazon.com/rds/instance-types/](https://aws.amazon.com/rds/instance-types/)

**Domínio:**  
Cloud Concepts

---

### Pergunta 2

**Incorreto**  
**Which of the following statements are CORRECT regarding the AWS VPC service? (Select two)**

- **Sua seleção está correta:** A Security Group can have allow rules only
- **Sua seleção está incorreta:** A Network Address Translation instance (NAT instance) is managed by AWS
- A Security Group can have both allow and deny rules
- **Seleção correta:** A Network Address Translation gateway (NAT gateway) is managed by AWS
- A network access control list (network ACL) can have allow rules only

**Explicação geral**  
**Correct options:**

- **A Security Group can have allow rules only**
- **A Network Address Translation gateway (NAT gateway) is managed by AWS**

Um grupo de segurança atua como um firewall virtual para sua instância para controlar o tráfego de entrada e saída. Os grupos de segurança atuam no nível da instância, não no nível da sub-rede. Você pode especificar regras de permissão, mas não regras de negação. Você pode especificar regras separadas para o tráfego de entrada e saída.

**Security Group Overview:**  
[https://docs.aws.amazon.com/vpc/latest/userguide/VPC_SecurityGroups.html](https://docs.aws.amazon.com/vpc/latest/userguide/VPC_SecurityGroups.html)

Uma lista de controle de acesso de rede (network ACL) é uma camada opcional de segurança para sua VPC que atua como um firewall para controlar o tráfego de entrada e saída de uma ou mais sub-redes (ou seja, funciona no nível da sub-rede). Uma ACL de rede possui regras de entrada e saída separadas, e cada regra pode permitir ou negar tráfego.

**network access control list (network ACL) Overview:**  
[https://docs.aws.amazon.com/vpc/latest/userguide/vpc-network-acls.html](https://docs.aws.amazon.com/vpc/latest/userguide/vpc-network-acls.html)

Você pode usar um gateway de tradução de endereços de rede (NAT) ou uma instância de tradução de endereços de rede (NAT) para permitir que instâncias em uma sub-rede privada se conectem à internet ou a outros serviços da AWS, mas impedindo que a internet inicie uma conexão com essas instâncias. O NAT gateway é gerenciado pela AWS, mas a instância NAT é gerenciada por você.

**Comparison table for differences between NAT gateway and NAT instance:**  
[https://docs.aws.amazon.com/vpc/latest/userguide/vpc-nat-comparison.html](https://docs.aws.amazon.com/vpc/latest/userguide/vpc-nat-comparison.html)

**Incorrect options:**

- A Security Group can have both allow and deny rules
- A Network Address Translation instance (NAT instance) is managed by AWS
- A network access control list (network ACL) can have allow rules only

Essas três opções contradizem os detalhes fornecidos anteriormente na explicação, portanto, essas opções estão incorretas.

**References:**  
[https://docs.aws.amazon.com/vpc/latest/userguide/VPC_SecurityGroups.html](https://docs.aws.amazon.com/vpc/latest/userguide/VPC_SecurityGroups.html)  
[https://docs.aws.amazon.com/vpc/latest/userguide/vpc-network-acls.html](https://docs.aws.amazon.com/vpc/latest/userguide/vpc-network-acls.html)

**Domínio:**  
Cloud Concepts

---

### Pergunta 3

**Incorreto**  
**AWS Web Application Firewall (WAF) offers protection from common web exploits at which layer?**

- **Sua resposta está incorreta:** Layer 3
- Layer 4 and 7
- Layer 4
- **Resposta correta:** Layer 7

**Explicação geral**  
**Correct option:**

**Layer 7**

O AWS WAF é um firewall de aplicação web que permite monitorar as solicitações HTTP e HTTPS encaminhadas para uma API do Amazon API Gateway, Amazon CloudFront ou um Application Load Balancer. As solicitações HTTP e HTTPS fazem parte da camada de Aplicação, que é a camada 7.

**Incorrect options:**

- **Layer 3** - A camada 3 é a camada de Rede e essa camada decide qual caminho físico os dados seguirão ao se mover na rede. O AWS Shield oferece proteção nessa camada. O WAF não oferece proteção nessa camada.
- **Layer 4** - A camada 4 é a camada de Transporte e, nessa camada, a transmissão de dados ocorre usando os protocolos TCP ou UDP. O AWS Shield oferece proteção nessa camada. O WAF não oferece proteção nessa camada.
- **Layer 4 and 7** - Esta opção foi adicionada como um distrator.

**Reference:**  
[https://docs.aws.amazon.com/waf/latest/developerguide/what-is-aws-waf.html](https://docs.aws.amazon.com/waf/latest/developerguide/what-is-aws-waf.html)

**Domínio:**  
Security and Compliance

---

### Pergunta 4

**Incorreto**  
**An intern at an IT company provisioned a Linux based On-demand EC2 instance with per-second billing but terminated it within 30 seconds as he wanted to provision another instance type. What is the duration for which the instance would be charged?**

- **Sua resposta está incorreta:** 600 seconds
- **Resposta correta:** 60 seconds
- 30 seconds
- 300 seconds

**Explicação geral**  
**Correct option:**

**60 seconds**

Há uma cobrança mínima de um minuto para instâncias EC2 baseadas em Linux, então essa é a opção correta.

**Incorrect options:**

- 30 seconds
- 300 seconds
- 600 seconds

Essas três opções contradizem os detalhes fornecidos anteriormente na explicação, então essas opções estão incorretas.

**Reference:**  
[https://aws.amazon.com/blogs/aws/new-per-second-billing-for-ec2-instances-and-ebs-volumes/](https://aws.amazon.com/blogs/aws/new-per-second-billing-for-ec2-instances-and-ebs-volumes/)

**Domínio:**  
Billing and Pricing

---

### Pergunta 5

**Incorreto**  
**A startup wants to provision an EC2 instance for the lowest possible cost for a long-term duration but needs to make sure that the instance would never be interrupted. As a Cloud Practitioner, which of the following options would you recommend?**

- **Sua resposta está incorreta:** EC2 On-Demand Instance
- EC2 Dedicated Host
- **Resposta correta:** EC2 Reserved Instance (RI)
- EC2 Spot Instance

**Explicação geral**  
**Correct option:**

**EC2 Reserved Instance (RI)**

Uma Instância Reservada EC2 (RI) oferece economias significativas (até 75%) nos custos do Amazon EC2 em comparação com a precificação de instâncias sob demanda. Uma Instância Reservada (RI) não é uma instância física, mas sim um desconto de cobrança aplicado ao uso de instâncias sob demanda em sua conta. Você pode comprar uma Instância Reservada (RI) para um compromisso de um ou três anos, com o compromisso de três anos oferecendo um desconto maior. Uma instância reservada (RI) não pode ser interrompida. Portanto, esta é a opção correta.

**EC2 Pricing Options Overview:**  
[https://aws.amazon.com/ec2/pricing/](https://aws.amazon.com/ec2/pricing/)

**Incorrect options:**

- **EC2 On-Demand Instance** - Uma Instância On-Demand do EC2 é uma instância que você usa sob demanda. Você tem controle total sobre seu ciclo de vida — você decide quando iniciar, parar, hibernar, iniciar, reiniciar ou encerrar. Não há necessidade de compromisso de longo prazo ao comprar Instâncias On-Demand. Não há pagamento antecipado e você paga apenas pelos segundos em que suas Instâncias On-Demand estão em execução. O preço por segundo para execução de uma Instância On-Demand é fixo. Instâncias on-demand não podem ser interrompidas. No entanto, instâncias on-demand não são tão econômicas quanto as instâncias reservadas, então essa opção não é correta.
- **EC2 Spot Instance** - Uma Instância Spot do EC2 é uma instância EC2 não utilizada que está disponível por menos do que o preço On-Demand. Como as Instâncias Spot permitem que você solicite instâncias EC2 não utilizadas com grandes descontos (até 90%), você pode reduzir significativamente seus custos do Amazon EC2. As Instâncias Spot são adequadas para análise de dados, trabalhos em lote, processamento em segundo plano e tarefas opcionais. Essas instâncias podem ser terminadas com pouco aviso, então não são adequadas para workloads críticos que precisam ser executados em um momento específico. Portanto, esta opção não é correta para o caso de uso fornecido.
- **EC2 Dedicated Host** - Um Amazon EC2 Dedicated Host permite que você use suas licenças de software elegíveis de fornecedores como Microsoft e Oracle no Amazon EC2, de forma que você obtenha a flexibilidade e a eficácia de custos de usar suas licenças, mas com a resiliência, simplicidade e elasticidade da AWS. Um Amazon EC2 Dedicated Host é um servidor físico totalmente dedicado ao seu uso, então você pode ajudar a atender aos requisitos de conformidade corporativa. Não é economicamente eficiente em comparação com uma instância On-Demand. Então, essa opção não é correta.

**Reference:**  
[https://aws.amazon.com/ec2/pricing/](https://aws.amazon.com/ec2/pricing/)

**Domínio:**  
Billing and Pricing

---

### Pergunta 6

**Incorreto**  
**Which of the following Amazon S3 storage classes takes the most time to retrieve data (also known as first byte latency)?**

- **Sua resposta está incorreta:** Amazon S3 Glacier Flexible Retrieval
- Amazon S3 Intelligent-Tiering
- **Resposta correta:** Amazon S3 Glacier Deep Archive
- Amazon S3 Standard

**Explicação geral**  
**Correct option:**

**Amazon S3 Glacier Deep Archive**

O Amazon S3 Glacier Deep Archive é a classe de armazenamento de menor custo do Amazon S3 e suporta retenção de longo prazo e preservação digital para dados que podem ser acessados uma ou duas vezes por ano. Ele é projetado para clientes — especialmente aqueles em indústrias altamente regulamentadas, como Serviços Financeiros, Saúde e Setores Públicos — que retêm conjuntos de dados por 7 a 10 anos ou mais para atender aos requisitos de conformidade regulamentar. O Amazon S3 Glacier Deep Archive também pode ser usado para casos de uso de backup e recuperação de desastres. Ele tem um tempo de recuperação (latência do primeiro byte) de 12 a 48 horas.

**Incorrect options:**

- **Amazon S3 Standard** - O Amazon S3 Standard oferece armazenamento de objetos com alta durabilidade, disponibilidade e desempenho para dados acessados com frequência. O Amazon S3 Standard tem um tempo de recuperação (latência do primeiro byte) de milissegundos.
- **Amazon S3 Intelligent-Tiering** - A classe de armazenamento Amazon S3 Intelligent-Tiering é projetada para otimizar custos movendo automaticamente os dados para o nível de acesso mais econômico, sem impacto no desempenho ou sobrecarga operacional. Ela funciona armazenando objetos em dois níveis de acesso: um nível otimizado para acesso frequente e outro nível de custo mais baixo otimizado para acesso infrequente. O Amazon S3 Intelligent-Tiering tem um tempo de recuperação (latência do primeiro byte) de milissegundos.
- **Amazon S3 Glacier Flexible Retrieval** - O Amazon S3 Glacier Flexible Retrieval oferece armazenamento de baixo custo, até 10% mais barato (do que o Amazon S3 Glacier Instant Retrieval), para dados de arquivo que são acessados 1 a 2 vezes por ano e são recuperados de forma assíncrona. Para dados de arquivo que não requerem acesso imediato, mas precisam da flexibilidade para recuperar grandes conjuntos de dados sem custo, como casos de uso de backup ou recuperação de desastres, o Amazon S3 Glacier Flexible Retrieval (anteriormente Amazon S3 Glacier) é a classe de armazenamento ideal.

**Reference:**  
[https://aws.amazon.com/s3/storage-classes/](https://aws.amazon.com/s3/storage-classes/)

**Domínio:**  
Technology

---

### Pergunta 7

**Incorreto**  
**Which of the following AWS Support plans provide access to guidance, configuration, and troubleshooting of AWS interoperability with third-party software? (Select two)**

- **Sua seleção está incorreta:** AWS Corporate Support
- **Sua seleção está correta:** AWS Enterprise Support
- AWS Basic Support
- **Seleção correta:** AWS Business Support
- AWS Developer Support

**Explicação geral**  
**Correct options:**

- **AWS Enterprise Support**
- **AWS Business Support**

O AWS Enterprise Support oferece aos clientes um serviço tipo concierge, onde o principal foco é ajudar o cliente a alcançar seus resultados e obter sucesso na nuvem. Com o Enterprise Support, você obtém suporte técnico 24x7 de engenheiros de alta qualidade, ferramentas e tecnologia para gerenciar automaticamente a saúde do seu ambiente, orientação arquitetônica consultiva entregue no contexto de suas aplicações e casos de uso, e um Gerente de Conta Técnico designado (TAM) para coordenar o acesso a programas proativos/preventivos e especialistas em assuntos da AWS. Você obtém acesso a orientação, configuração e solução de problemas de interoperabilidade da AWS com muitos sistemas operacionais, plataformas e componentes de pilha de aplicativos comuns.

**AWS Business Support**

Você deve usar o AWS Business Support se tiver workloads de produção na AWS e desejar acesso técnico 24x7 por telefone, e-mail e chat, além de orientação arquitetônica no contexto de seus casos de uso específicos. Você tem acesso total às verificações de boas práticas do AWS Trusted Advisor. Você tem acesso a orientação, configuração e solução de problemas de interoperabilidade da AWS com muitos sistemas operacionais, plataformas e componentes de pilha de aplicativos comuns.

**Exam Alert:**  
Revise as diferenças entre os planos de suporte AWS Developer Support, AWS Business Support, AWS Enterprise On-Ramp Support e AWS Enterprise Support, pois você pode esperar pelo menos algumas perguntas no exame:

**Incorrect options:**

- **AWS Basic Support** - O AWS Basic Support oferece apenas acesso aos seguintes itens:

  - Atendimento ao cliente e comunidades: Acesso 24x7 ao atendimento ao cliente, documentação, whitepapers e fóruns de suporte.
  - AWS Trusted Advisor: Acesso às verificações principais do Trusted Advisor e orientação para provisionar seus recursos seguindo as melhores práticas para aumentar o desempenho e melhorar a segurança.
  - AWS Health: Seu Painel de Controle de Saúde da Conta: Uma visão personalizada da saúde dos serviços da AWS, e alertas quando seus recursos são impactados.

- **AWS Developer Support** - Você deve usar o plano de suporte AWS Developer Support se estiver testando ou fazendo desenvolvimento inicial na AWS e desejar a capacidade de obter suporte técnico baseado em e-mail durante o horário comercial. Este plano também oferece orientação geral sobre como os serviços podem ser usados para vários casos de uso, workloads ou aplicações. Você não tem acesso ao Gerenciamento de Eventos de Infraestrutura com este plano.

Ambos os planos não suportam acesso a orientação, configuração e solução de problemas de interoperabilidade da AWS com software de terceiros.

- **AWS Corporate Support** - Esta é uma opção fictícia e foi adicionada como um distrator.

**Reference:**  
[https://aws.amazon.com/premiumsupport/plans/](https://aws.amazon.com/premiumsupport/plans/)

**Domínio:**  
Billing and Pricing

---

### Pergunta 8

**Incorreto**  
**An e-commerce company has deployed an RDS database in a single Availability Zone (AZ). The engineering team wants to ensure that in case of an AZ outage, the database should continue working on the same endpoint without any manual administrative intervention. Which of the following solutions can address this use-case?**

- **Sua resposta está incorreta:** Deploy the database via AWS Elastic Beanstalk
- Provision the database via AWS CloudFormation
- Configure the database in RDS read replica mode with automatic failover to the standby
- **Resposta correta:** Configure the database in RDS Multi-AZ deployment with automatic failover to the standby

**Explicação geral**  
**Correct option:**

**Configure the database in RDS Multi-AZ deployment with automatic failover to the standby**

Quando você provisiona uma instância de banco de dados Multi-AZ, o Amazon RDS cria automaticamente uma instância de banco de dados primária e replica os dados de forma síncrona para uma instância de standby em uma Zona de Disponibilidade (AZ) diferente. Em caso de falha de infraestrutura, o Amazon RDS realiza uma troca automática para o standby (ou para um read replica no caso do Amazon Aurora), para que você possa retomar as operações do banco de dados assim que a troca for concluída. Como o endpoint para sua instância de banco de dados permanece o mesmo após a troca, sua aplicação pode retomar a operação do banco de dados sem a necessidade de intervenção administrativa manual.

**Incorrect options:**

- **Deploy the database via AWS Elastic Beanstalk** - Você não pode implantar apenas um banco de dados via Elastic Beanstalk, pois ele é destinado para implantação automática de aplicações quando você carrega seu código. O Elastic Beanstalk cuida automaticamente da implantação, desde o provisionamento de capacidade, balanceamento de carga, auto-escalonamento até o monitoramento de saúde da aplicação. Portanto, essa opção está incorreta.
- **Configure the database in RDS read replica mode with automatic failover to the standby** - Para o RDS, os Read replicas permitem que você crie cópias somente leitura que são sincronizadas com seu banco de dados mestre. Não há standby disponível ao usar read replicas. Em caso de falha de infraestrutura, você deve promover manualmente o read replica para ser sua própria instância de banco de dados independente, o que significa que o endpoint do banco de dados mudaria. Portanto, essa opção está incorreta.
- **Provision the database via AWS CloudFormation** - Você pode provisionar o banco de dados via CloudFormation, com certeza, no entanto, isso não fornece nenhuma recuperação automática em caso de desastre.

**References:**  
[https://aws.amazon.com/rds/features/multi-az/](https://aws.amazon.com/rds/features/multi-az/)

**Domínio:**  
Cloud Concepts

---

### Pergunta 9

**Incorreto**  
**A financial services company wants to ensure that its AWS account activity meets the governance, compliance and auditing norms. As a Cloud Practitioner, which AWS service would you recommend for this use-case?**

- **Sua resposta está incorreta:** AWS Config
- Amazon CloudWatch
- **Resposta correta:** AWS CloudTrail
- AWS Trusted Advisor

**Explicação geral**  
**Correct option:**

**AWS CloudTrail**

Você pode usar o CloudTrail para registrar, monitorar e reter a atividade da conta relacionada a ações em sua infraestrutura da AWS. O CloudTrail fornece um histórico de eventos da atividade da sua conta AWS, incluindo ações realizadas através do Console de Gerenciamento da AWS, SDKs da AWS, ferramentas de linha de comando e outros serviços da AWS.

**How CloudTrail Works:**  
[https://aws.amazon.com/cloudtrail/](https://aws.amazon.com/cloudtrail/)

**Incorrect options:**

- **AWS Config** - O AWS Config é um serviço que permite avaliar, auditar e avaliar as configurações de seus recursos da AWS. O Config monitora e registra continuamente as configurações dos seus recursos da AWS e permite que você automatize a avaliação das configurações registradas em relação às configurações desejadas.
- **Amazon CloudWatch** - O Amazon CloudWatch é um serviço de monitoramento e observabilidade desenvolvido para engenheiros DevOps, desenvolvedores, engenheiros de confiabilidade de sites (SREs) e gerentes de TI. O CloudWatch fornece dados e insights acionáveis para monitorar aplicativos, responder a mudanças de desempenho em todo o sistema, otimizar o uso de recursos e obter uma visão unificada da saúde operacional. Este é um excelente serviço para construir sistemas resilientes.
- **AWS Trusted Advisor** - O AWS Trusted Advisor é uma ferramenta online que fornece orientação em tempo real para ajudar você a provisionar seus recursos seguindo as melhores práticas da AWS em otimização de custos, segurança, tolerância a falhas, limites de serviço e melhoria de desempenho.

**Exam Alert:**  
Você pode ver casos de uso pedindo para selecionar uma entre CloudWatch vs CloudTrail vs Config. Basta lembrar esta regra prática:

- Pense em monitoramento de desempenho de recursos, eventos e alertas; pense em CloudWatch.
- Pense em atividade específica da conta e auditoria; pense em CloudTrail.
- Pense em histórico de alterações específicas de recursos, auditoria e conformidade; pense em Config.

**Reference:**  
[https://aws.amazon.com/cloudtrail/](https://aws.amazon.com/cloudtrail/)

**Domínio:**  
Cloud Concepts

---

### Pergunta 10

**Incorreto**  
**Which of the following AWS services support reservations to optimize costs? (Select three)**

- **Sua seleção está incorreta:** Amazon DocumentDB
- **Sua seleção está incorreta:** AWS Lambda
- **Sua seleção está correta:** Amazon Elastic Compute Cloud (Amazon EC2)
- **Seleção correta:** Amazon DynamoDB
- **Seleção correta:** Amazon Relational Database Service (Amazon RDS)
- Amazon Simple Storage Service (Amazon S3)

**Explicação geral**  
**Correct options:**

- **Amazon Elastic Compute Cloud (Amazon EC2)**
- **Amazon DynamoDB**
- **Amazon Relational Database Service (Amazon RDS)**

Os seguintes serviços da AWS suportam reservas para otimizar custos:

- **Amazon EC2 Reserved Instances (RI):** Você pode usar o Amazon EC2 Reserved Instances (RI) para reservar capacidade e receber um desconto no uso de instâncias em comparação com o preço de instâncias On-Demand.
- **Amazon DynamoDB Reserved Capacity:** Se você puder prever sua necessidade de capacidade de leitura e gravação do Amazon DynamoDB, a Capacidade Reservada oferece economias significativas em relação ao preço normal da capacidade provisionada do DynamoDB.
- **Amazon ElastiCache Reserved Nodes:** Os Amazon ElastiCache Reserved Nodes oferecem a opção de fazer um pagamento único baixo para cada nó de cache que você deseja reservar e, em troca, receber um desconto significativo na cobrança por hora para esse nó.
- **Amazon RDS RIs:** Como o Amazon EC2 RIs, o Amazon RDS RIs pode ser comprado usando termos de No Upfront, Partial Upfront ou All Upfront. Todos os tipos de Instância Reservada estão disponíveis para os mecanismos de banco de dados Aurora, MySQL, MariaDB, PostgreSQL, Oracle e SQL Server.
- **Amazon Redshift Reserved Nodes:** Se você pretende manter um cluster do Amazon Redshift em execução continuamente por um período prolongado, deve considerar a compra de ofertas de nós reservados. Essas ofertas proporcionam economias significativas em relação à precificação on-demand, mas exigem que você reserve nós de computação e se comprometa a pagar por esses nós por um período de 1 ou 3 anos.

**Incorrect options:**

- **Amazon DocumentDB** - O Amazon DocumentDB (com compatibilidade com MongoDB) é um serviço de banco de dados de documentos rápido, escalável, altamente disponível e totalmente gerenciado que suporta workloads MongoDB. Como um banco de dados de documentos, o Amazon DocumentDB facilita o armazenamento, consulta e indexação de dados JSON.
- **AWS Lambda** - O AWS Lambda permite que você execute código sem provisionar ou gerenciar servidores. Você paga apenas pelo tempo de computação que consome.
- **Amazon Simple Storage Service (Amazon S3)** - O Amazon Simple Storage Service (Amazon S3) é um serviço de armazenamento de objetos que oferece escalabilidade, disponibilidade de dados, segurança e desempenho líderes do setor.

Nenhum desses serviços da AWS suporta reservas para otimizar custos.

**Reference:**  
[https://d0.awsstatic.com/whitepapers/aws_pricing_overview.pdf](https://d0.awsstatic.com/whitepapers/aws_pricing_overview.pdf)

**Domínio:**  
Billing and Pricing

### Pergunta 11

**Correto**  
**Which of the following are correct statements regarding the AWS Global Infrastructure? (Select two)**

- **Sua seleção está correta:** Each AWS Region consists of a minimum of three Availability Zones (AZ)
- **Sua seleção está correta:** Each Availability Zone (AZ) consists of one or more discrete data centers
- Each AWS Region consists of two or more Edge Locations
- Each AWS Region consists of a minimum of two Availability Zones (AZ)
- Each Availability Zone (AZ) consists of two or more discrete data centers

**Explicação geral**  
**Correct options:**

- **Each AWS Region consists of a minimum of three Availability Zones (AZ)**
- **Each Availability Zone (AZ) consists of one or more discrete data centers**

A AWS possui o conceito de uma Região, que é um local físico ao redor do mundo onde a AWS agrupa seus data centers. A AWS chama cada grupo de data centers lógicos de Zona de Disponibilidade (AZ). Cada Região da AWS consiste em um mínimo de três Zonas de Disponibilidade (AZs) isoladas e fisicamente separadas dentro de uma área geográfica. Cada AZ possui energia, refrigeração e segurança física independentes e está conectada por redes redundantes e de baixa latência.

Uma Zona de Disponibilidade (AZ) é um ou mais data centers discretos com energia, rede e conectividade redundantes em uma Região da AWS. Todas as AZs em uma Região da AWS estão interconectadas com redes de alta largura de banda e baixa latência, através de uma fibra metropolitana totalmente redundante, proporcionando alta taxa de transferência e baixa latência entre as AZs.

**AWS Regions and Availability Zones Overview:**  
[https://aws.amazon.com/about-aws/global-infrastructure/regions_az/](https://aws.amazon.com/about-aws/global-infrastructure/regions_az/)

**Incorrect options:**

- **Each AWS Region consists of a minimum of two Availability Zones (AZ)**
- **Each Availability Zone (AZ) consists of two or more discrete data centers**
- **Each AWS Region consists of two or more Edge Locations**

Essas três opções contradizem os detalhes fornecidos anteriormente na explicação, então essas opções estão incorretas.

**Reference:**  
[https://aws.amazon.com/about-aws/global-infrastructure/regions_az/](https://aws.amazon.com/about-aws/global-infrastructure/regions_az/)

**Domínio:**  
Technology

---

### Pergunta 12

**Incorreto**  
**A web application stores all of its data on Amazon S3 buckets. A client has mandated that data be encrypted before sending it to Amazon S3.**

**Which of the following is the right technique for encrypting data as needed by the customer?**

- **Sua resposta está incorreta:** Enable server-side encryption with AWS Key Management Service (AWS KMS) keys (SSE-KMS)
- Encryption is enabled by default for all the objects written to Amazon S3. Additional configuration is not required
- **Resposta correta:** Enable client-side encryption using AWS encryption SDK
- Enable server-side encryption with Amazon S3 Managed Keys (SSE-S3)

**Explicação geral**  
**Correct option:**

**Enable client-side encryption using AWS encryption SDK**

O ato de criptografar dados antes de enviá-los para o Amazon S3 é denominado criptografia no lado do cliente. O SDK de criptografia da AWS é uma biblioteca de criptografia no lado do cliente separada dos SDKs específicos de linguagem. Você pode usar essa biblioteca de criptografia para implementar mais facilmente as melhores práticas de criptografia no Amazon S3. Ao contrário dos clientes de criptografia do Amazon S3 nos SDKs específicos de linguagem da AWS, o SDK de criptografia da AWS não é vinculado ao Amazon S3 e pode ser usado para criptografar ou descriptografar dados que serão armazenados em qualquer lugar.

**Incorrect options:**

- **Enable server-side encryption with Amazon S3 Managed Keys (SSE-S3)** - Quando você usa criptografia no lado do servidor com Chaves Gerenciadas do Amazon S3 (SSE-S3), cada objeto é criptografado com uma chave única. Como medida adicional, ele criptografa a própria chave com uma chave raiz que é regularmente rotacionada.

- **Enable server-side encryption with AWS Key Management Service (AWS KMS) keys (SSE-KMS)** - A criptografia no lado do servidor com chaves AWS KMS (SSE-KMS) é semelhante ao SSE-S3, mas com alguns benefícios adicionais e cobranças pelo uso desse serviço. Existem permissões separadas para o uso de uma chave KMS que oferecem proteção adicional contra acesso não autorizado aos seus objetos no Amazon S3. O SSE-KMS também fornece um registro de auditoria que mostra quando sua chave KMS foi usada e por quem.

A criptografia no lado do servidor é a criptografia de dados no seu destino pela aplicação ou serviço que os recebe. O Amazon S3 criptografa seus dados no nível do objeto à medida que os grava em discos em seus data centers e os descriptografa para você quando você os acessa. Portanto, a criptografia no lado do servidor não é a resposta correta para o cenário atual. Portanto, ambas as opções estão incorretas.

- **Encryption is enabled by default for all the objects written to Amazon S3. Additional configuration is not required** - Embora seja correto que a criptografia esteja habilitada por padrão para todos os objetos gravados no Amazon S3, o caso de uso dado exige que os dados sejam criptografados antes de serem enviados ao Amazon S3, o que não pode ser realizado com a opção dada. Portanto, essa opção está incorreta.

**References:**  
[https://docs.aws.amazon.com/en_us/AmazonS3/latest/userguide/UsingClientSideEncryption.html](https://docs.aws.amazon.com/en_us/AmazonS3/latest/userguide/UsingClientSideEncryption.html)  
[https://docs.aws.amazon.com/en_us/AmazonS3/latest/userguide/serv-side-encryption.html](https://docs.aws.amazon.com/en_us/AmazonS3/latest/userguide/serv-side-encryption.html)

**Domínio:**  
Security and Compliance

---

### Pergunta 13

**Incorreto**  
**According to the AWS Shared Responsibility Model, which of the following are responsibilities of AWS? (Select two)**

- **Sua seleção está correta:** Operating the infrastructure layer, the operating system and the platform for the Amazon S3 service
- **Sua seleção está incorreta:** Enabling Multi Factor Authentication on AWS accounts in your organization
- Creating IAM role for accessing Amazon EC2 instances
- Creating S3 bucket policies for appropriate user access
- **Seleção correta:** Replacing faulty hardware of Amazon EC2 instances

**Explicação geral**  
**Correct options:**

De acordo com o AWS Shared Responsibility Model, a AWS é responsável pela "Segurança da Nuvem". Isso inclui proteger a infraestrutura que executa todos os serviços oferecidos na Nuvem AWS. Esta infraestrutura é composta pelo hardware, software, rede e instalações que executam os serviços da Nuvem AWS.

- **Replacing faulty hardware of Amazon EC2 instances** - Substituir hardware defeituoso das instâncias Amazon EC2 faz parte da manutenção da infraestrutura "da" nuvem. Esta é a responsabilidade da AWS.
- **Operating the infrastructure layer, the operating system and the platform for the Amazon S3 service** - Para serviços abstratos, como Amazon S3 e Amazon DynamoDB, a AWS opera a camada de infraestrutura, o sistema operacional e as plataformas, e os clientes acessam os endpoints para armazenar e recuperar dados.

**Shared Responsibility Model Overview:**  
[https://aws.amazon.com/compliance/shared-responsibility-model/](https://aws.amazon.com/compliance/shared-responsibility-model/)

**Incorrect options:**

- **Enabling Multi Factor Authentication on AWS accounts in your organization** - Habilitar a autenticação multifator para contas da AWS em sua organização é sua responsabilidade. Por outro lado, a AWS é responsável por garantir que os dados do usuário criados e suas relações e políticas sejam armazenados em uma infraestrutura à prova de falhas.

- **Creating IAM role for accessing Amazon EC2 instances** - Criar funções de usuário e políticas é responsabilidade do cliente. Os clientes decidirão "quais" recursos recebem "que" acesso.

- **Creating S3 bucket policies for appropriate user access** - Criar políticas de bucket para acesso aos dados do Amazon S3 é responsabilidade do cliente. O cliente decide quem tem acesso aos dados que ele armazena no S3 e usará as ferramentas da AWS para implementar esses requisitos. A AWS, por outro lado, é responsável por manter os dados seguros contra falhas de hardware e software.

**Reference:**  
[https://aws.amazon.com/compliance/shared-responsibility-model/](https://aws.amazon.com/compliance/shared-responsibility-model/)

**Domínio:**  
Security and Compliance

---

### Pergunta 14

**Incorreto**  
**An IT company is planning to migrate from an on-premises environment to AWS Cloud. Which of the following expense areas would result in cost savings when the company moves to AWS Cloud? (Select two)**

- **Sua seleção está incorreta:** SaaS application license fee
- **Sua seleção está correta:** Data center physical security expenditure
- Developer salary
- Project manager salary
- **Seleção correta:** Data center hardware infrastructure expenditure

**Explicação geral**  
**Correct options:**

- **Data center hardware infrastructure expenditure**
- **Data center physical security expenditure**

A empresa não precisa gastar na infraestrutura de hardware de computação e na segurança física do data center. Portanto, essas áreas de despesa resultariam em economia de custos. O gasto com a taxa de licença de aplicativo SaaS, salário do desenvolvedor e salário do gerente de projeto permaneceria o mesmo.

**Exam Alert:**  
Confira as seis vantagens da computação em nuvem. Você certamente será questionado sobre as vantagens da computação em nuvem em comparação com uma configuração tradicional on-premises:  
[https://docs.aws.amazon.com/whitepapers/latest/aws-overview/six-advantages-of-cloud-computing.html](https://docs.aws.amazon.com/whitepapers/latest/aws-overview/six-advantages-of-cloud-computing.html)

**Incorrect options:**

- **SaaS application license fee**
- **Developer salary**
- **Project manager salary**

Conforme explicado anteriormente, o gasto com a taxa de licença de aplicativo SaaS, salário do desenvolvedor e salário do gerente de projeto permaneceria o mesmo, então essas opções estão incorretas.

**Reference:**  
[https://docs.aws.amazon.com/whitepapers/latest/aws-overview/six-advantages-of-cloud-computing.html](https://docs.aws.amazon.com/whitepapers/latest/aws-overview/six-advantages-of-cloud-computing.html)

**Domínio:**  
Cloud Concepts

---

### Pergunta 15

**Correto**  
**A company wants to identify the optimal AWS resource configuration for its workloads so that the company can reduce costs and increase workload performance. Which of the following services can be used to meet this requirement?**

- **Sua resposta está correta:** AWS Compute Optimizer
- AWS Systems Manager
- AWS Cost Explorer
- AWS Budgets

**Explicação geral**  
**Correct option:**

**AWS Compute Optimizer**

O AWS Compute Optimizer recomenda os recursos ideais da AWS para suas cargas de trabalho para reduzir custos e melhorar o desempenho, usando aprendizado de máquina para analisar métricas históricas de utilização. Superprovisionar recursos pode levar a custos de infraestrutura desnecessários, e subprovisionar recursos pode levar a um desempenho ruim da aplicação. O Compute Optimizer ajuda você a escolher configurações ideais para três tipos de recursos da AWS: instâncias Amazon EC2, volumes Amazon EBS e funções AWS Lambda, com base nos seus dados de utilização.

O Compute Optimizer recomenda até 3 opções de mais de 140 tipos de instâncias EC2, bem como uma ampla gama de opções de configuração de volumes EBS e funções Lambda, para dimensionar corretamente suas cargas de trabalho. O Compute Optimizer também projeta qual seria a utilização de CPU, utilização de memória e tempo de execução de sua carga de trabalho nas opções recomendadas de recursos da AWS. Isso ajuda você a entender como sua carga de trabalho teria se comportado nas opções recomendadas antes de implementar as recomendações.

**How Compute Optimizer works:**  
[https://aws.amazon.com/compute-optimizer/](https://aws.amazon.com/compute-optimizer/)

**Incorrect options:**

- **AWS Systems Manager** - O AWS Systems Manager é o hub de operações da AWS. O Systems Manager fornece uma interface de usuário unificada para que você possa rastrear e resolver problemas operacionais em seus aplicativos e recursos da AWS a partir de um local central. Com o Systems Manager, você pode automatizar tarefas operacionais para instâncias Amazon EC2 ou instâncias Amazon RDS. Você também pode agrupar recursos por aplicativo, visualizar dados operacionais para monitoramento e solução de problemas, implementar fluxos de trabalho de alteração pré-aprovados e auditar alterações operacionais para seus grupos de recursos. O Systems Manager não pode ser usado para identificar a configuração ideal de recursos para cargas de trabalho que estão sendo executadas na AWS.

- **AWS Budgets** - O AWS Budgets permite definir orçamentos personalizados para acompanhar seus custos e uso, desde os casos de uso mais simples até os mais complexos. Com o AWS Budgets, você pode optar por ser alertado por e-mail ou notificação do SNS quando os custos reais ou previstos excederem o limite do seu orçamento, ou quando a utilização ou cobertura do seu RI e dos planos de poupança cair abaixo do limite desejado. Com as Ações do Orçamento da AWS, você também pode configurar ações específicas para responder ao status de custo e uso em suas contas, de forma que, se seus custos ou uso excederem ou forem previstos para exceder o limite, as ações possam ser executadas automaticamente ou com sua aprovação para reduzir o gasto excessivo não intencional.

- **AWS Cost Explorer** - O AWS Cost Explorer possui uma interface fácil de usar que permite visualizar, entender e gerenciar seus custos e uso da AWS ao longo do tempo. As Recomendações de Rightsizing de Recursos do Cost Explorer e o Compute Optimizer usam o mesmo mecanismo de recomendação. O mecanismo de recomendação do Compute Optimizer oferece recomendações para ajudar os clientes a identificar os tipos de instâncias EC2 ideais para suas cargas de trabalho. O console e a API do Cost Explorer mostram um subconjunto dessas recomendações que podem levar a economias de custos e as complementa com informações específicas de custo e economia do cliente (por exemplo, informações de cobrança, créditos disponíveis, RI e planos de poupança) para ajudar os responsáveis pela gestão de custos a identificar rapidamente oportunidades de economia por meio do dimensionamento correto da infraestrutura. O console e a API do Compute Optimizer fornecem todas as recomendações, independentemente das implicações de custo.

**Reference:**  
[https://aws.amazon.com/compute-optimizer/](https://aws.amazon.com/compute-optimizer/)

**Domínio:**  
Technology
