## Pergunta 1

**Qual dos serviços abaixo é uma solução para a criação de contêineres na AWS?**

- **✅** Amazon ECS
    - O Amazon Elastic Container Service (Amazon ECS) é um serviço de orquestração de containers da AWS que simplifica a implantação, gerenciamento e escalabilidade de aplicativos baseados em containers.

- AWS Auto Scaling
    - O AWS Auto Scaling monitora os aplicativos e ajusta automaticamente a capacidade para manter um desempenho constante e previsível pelo menor custo possível.

- Amazon EC2
    - O Amazon Elastic Compute Cloud (Amazon EC2) é um serviço Web que disponibiliza capacidade computacional segura e redimensionável na nuvem.

- Amazon ECR
    - O Amazon Elastic Container Registry (Amazon ECR) é um registro de contêiner totalmente gerenciado que facilita o armazenamento, o gerenciamento, o compartilhamento e a implantação de imagens e artefatos de contêiner em qualquer lugar.

> **Explicação geral**:  
> O Amazon ECS facilita a execução e a gestão de containers na AWS, integrando-se bem com outros serviços da AWS, como o Amazon ECR para armazenamento de imagens de containers. Isso permite que desenvolvedores se concentrem na criação de aplicativos sem a complexidade de configurar uma infraestrutura de contêiner completa.

---

## Pergunta 2

**Qual é a melhor definição para Region (Região)?**

- Uma region(região) é um ponto de uma edge location(rede de borda)
    - Região (Region) é uma área geográfica com vários data centers (Zonas de Disponibilidade), enquanto uma Localização de Borda (Edge Location) é um ponto de presença usado para cache de conteúdo e entrega rápida de dados. Elas servem a propósitos diferentes na infraestrutura da AWS.

- Uma region(região) é um data center dentro de uma avalibility zone(zonas de disponibilidade)
    - Região (Region) é uma área geográfica composta por várias Zonas de Disponibilidade (Availability Zones), e cada Zona de Disponibilidade contém um ou mais data centers. Portanto, uma Região abrange múltiplas Zonas de Disponibilidade e não se limita a um único data center.

- **✅** Uma region(região) é uma localização geográfica física composta por um ou mais data centers isolados e redundantes, chamada de zonas de disponibilidade, que a AWS utiliza para implantar e operar serviços de nuvem.
    - As Regiões da AWS garantem alta disponibilidade e resiliência ao isolar fisicamente as zonas de disponibilidade, melhoram a experiência do usuário ao reduzir a latência com proximidade geográfica, e ajudam a cumprir requisitos legais de armazenamento de dados.

- Uma region(região) é um continente que agrupa todos os data centers da AWS.
    - Região (Region) é uma área geográfica específica que contém várias Zonas de Disponibilidade (Availability Zones), não um continente. Cada Região possui seus próprios data centers e não agrupa todos os data centers da AWS globalmente.

> **Explicação geral**:  
> As Regiões da AWS são localizações geográficas que contêm Zonas de Disponibilidade. Cada Região é projetada para ser completamente isolada das outras para garantir a máxima resiliência e disponibilidade dos serviços.

---

## Pergunta 3

**Quais dos seguintes serviços permite a criação de scripts e automação a partir da linha de comando?**

- AWS Console
    - O Console da AWS é uma interface gráfica baseada na web que permite gerenciar e configurar os serviços da AWS de maneira intuitiva e visual.

- AWS SDK
    - O AWS SDK (Software Development Kit) é um conjunto de ferramentas que permite aos desenvolvedores integrar e interagir facilmente com os serviços da AWS em suas aplicações.

- AWS CloudFormation
    - O AWS CloudFormation permite criar, gerenciar e configurar recursos da AWS automaticamente usando templates em JSON ou YAML.

- **✅** AWS CLI
    - A Interface da Linha de Comando (CLI) da AWS é uma ferramenta unificada para o gerenciamento de seus serviços da AWS.

> **Explicação geral**:  
> A AWS CLI oferece uma interface unificada para que os usuários interajam com os serviços AWS a partir da linha de comando. Ela é ideal para automação, execução de scripts e integração de workflows personalizados.

---

## Pergunta 4

**Qual serviço da AWS oferece uma variedade de produtos para permitir que a empresa realize essa migração de forma física?**

- **✅** AWS Snowball
    - O AWS Snow oferece uma variedade de produtos para permitir que a empresa realize a migração de grandes quantidades de dados em dispositivos físicos.

- AWS DirectConnect
    - O AWS Direct Connect é uma solução de serviço de nuvem que facilita o estabelecimento de uma conexão de rede dedicada entre suas instalações e a AWS.

- AWS DMS
    - O AWS Database Migration Service (DMS) facilita a migração e replicação de bancos de dados para a AWS de forma segura e com mínimo tempo de inatividade.

- AWS DataSync
    - O AWS DataSync é um serviço utilizado para realizar a sincronização de dados de forma automática da sua infraestrutura on-premise com a AWS.

> **Explicação geral**:  
> O AWS Snowball é parte da família AWS Snow, que oferece dispositivos físicos para a transferência de grandes quantidades de dados para a AWS, sendo ideal para ambientes onde a conectividade de rede é limitada ou inviável para grandes volumes de dados.

---

## Pergunta 5

**Como o AWS Personal Health Dashboard pode ajudar as empresas a lidarem com eventos que afetam os recursos da AWS de suas contas?**

- Criando automaticamente recursos alternativos e resilientes.
    - Máquinas adicionais são fornecidas pelo Auto Scalling Group.

- Monitorando o tráfego de rede em tempo real.
    - Monitoramento de Tráfego de rede é fornecido pelo AWS Firewall Manager.

- **✅** Fornecendo alertas proativos e orientações para diagnóstico e resolução de problemas.
    - O AWS Personal Health Dashboard fornece alertas e orientações proativas sobre eventos da AWS que podem impactar sua infraestrutura específica.

- Ofertando suporte técnico dedicado e especializado.
    - Suporte Técnico especializado pode ser contratado através do AWS IQ.

> **Explicação geral**:  
> O AWS Personal Health Dashboard fornece notificações personalizadas e orientações para ajudá-lo a planejar e responder a eventos que podem afetar seus recursos na AWS, oferecendo maior visibilidade e controle sobre sua infraestrutura.

---

## Pergunta 6

**Qual dos seguintes itens não está incluído nos tipos de uso do Free Tier (nível gratuito) da AWS?**

- Testes de Curto Prazo - Experimentação (Trial)
    - A AWS Free Tier oferece três tipos de uso gratuito: 12 Meses Gratuitos, Sempre Gratuito e Testes de Curto Prazo.

- 12 Meses gratuitos
    - A AWS Free Tier oferece três tipos de uso gratuito: 12 Meses Gratuitos, Sempre Gratuito e Testes de Curto Prazo.

- **✅** Reserved
    - Reserved não é um nível gratuito, é um modelo de pagamento de instâncias EC2.

- Sempre gratuito
    - A AWS Free Tier oferece três tipos de uso gratuito: 12 Meses Gratuitos, Sempre Gratuito e Testes de Curto Prazo.

> **Explicação geral**:  
> O AWS Free Tier permite que novos clientes da AWS experimentem o serviço de forma gratuita. Entretanto, algumas ofertas, como instâncias reservadas, exigem um compromisso financeiro que não está incluído no nível gratuito.

---

## Pergunta 7

**Qual serviço utiliza Inteligência Artificial e analisa dados gerados por eventos de diversos serviços e armazenados no S3, evitando que atividades maliciosas sejam realizadas?**

- AWS Macie
    - O Amazon Macie é um serviço de segurança e privacidade de dados totalmente gerenciado que usa machine learning e correspondência de padrões para descobrir e proteger seus dados confidenciais na AWS.

- AWS WAF
    - O AWS WAF (Web Application Firewall) é um serviço que protege aplicações web contra ameaças comuns na web.

- **✅** AWS GuardDuty
    - O Amazon GuardDuty é um serviço de detecção de ameaças gerenciado pela AWS que monitora e protege sua infraestrutura na nuvem.

- AWS Shield
    - O AWS Shield é um serviço gerenciado de proteção contra DDoS (Negação de serviço distribuída) que protege os aplicativos executados na AWS.

> **Explicação geral**:  
> O Amazon GuardDuty é um serviço de detecção de ameaças que utiliza machine learning para identificar atividades maliciosas ou não autorizadas na sua conta AWS, protegendo a infraestrutura contra ameaças em potencial.

---

## Pergunta 8

**Qual é o serviço de integração totalmente gerenciado pela AWS, que permite transferir dados com segurança entre aplicativos de Software como Serviço (SaaS) como: Salesforce, Zendesk, Slack e ServiceNow, Amazon S3 e Amazon Redshift?**

- Amazon DMS
    - O AWS Database Migration Service (AWS DMS) ajuda você a migrar bancos de dados para a AWS de modo rápido e seguro.

- **✅** Amazon AppFlow
    - O AWS AppFlow é uma solução gerenciada que facilita a transferência segura de dados entre aplicativos SaaS e serviços da AWS.

- Amazon EventBridge
    - O Amazon EventBridge é um barramento de eventos sem servidor que torna mais fácil a criação de aplicações orientadas por eventos em escala.

- Amazon SNS
    - O Amazon Simple Notification Service (Amazon SNS) é um serviço de mensagens totalmente gerenciado para comunicação de aplicação a aplicação (A2A) e aplicação a pessoa (A2P).

> **Explicação geral**:  
> O Amazon AppFlow é um serviço de integração totalmente gerenciado que facilita a transferência segura de dados entre aplicativos SaaS, como Salesforce, e serviços da AWS, como S3 e Redshift, permitindo fluxos de trabalho de dados personalizados.

---

## Pergunta 9

**Qual benefício o AWS Security Hub pode oferecer para a empresa?**

- **✅** Uma visão consolidada da postura de segurança em serviços da AWS.
    - O AWS Security Hub fornece uma visão consolidada da postura de segurança em serviços da AWS, facilitando a identificação e a correção de vulnerabilidades e ameaças.

- Uma solução de firewall avançada.
    - O AWS Firewall Manager fornece soluções avançadas para gerenciar e aplicar regras de firewall em sua infraestrutura.

- Um serviço seguro para monitorar o consumo de recursos na AWS.
    - O monitoramento de consumo de recursos pode ser feito com o Amazon CloudWatch.

- Uma plataforma para desenvolvimento de aplicativos seguros na nuvem.
    - Uma plataforma para desenvolvimento de aplicativos é fornecida pelo AWS Cloud9 e SDKs.

> **Explicação geral**:  
> O AWS Security Hub fornece uma visão consolidada da postura de segurança em serviços da AWS, permitindo a identificação e a correção de vulnerabilidades e ameaças. Ele agrega e analisa resultados de verificações de segurança de vários serviços, facilitando a gestão de segurança e garantindo uma proteção mais eficiente no ambiente de nuvem.

---

## Pergunta 10

**Para conceder acesso à conta da AWS a três novos desenvolvedores, qual serviço específico da AWS deve ser empregado?**

- **✅** AWS Identity and Access Management (IAM)
    - O IAM (Identity and Access Management) é um serviço de controle de acesso da AWS que gerencia permissões de usuários e recursos.

- Amazon Simple Storage Service (S3)
    - O Amazon S3 é um serviço de armazenamento de objetos, não é usado para gerenciar permissões de acesso de usuários.

- Amazon Elastic Compute Cloud (EC2)
    - O Amazon EC2 é um serviço de computação na nuvem que fornece capacidade de computação sob demanda e não gerencia permissões de usuários.

- Amazon CloudFront
    - O Amazon CloudFront é um serviço de rede de entrega de conteúdo (CDN) e não gerencia permissões de acesso.

> **Explicação geral**:  
> O IAM (Identity and Access Management) é um serviço de controle de acesso da AWS que gerencia permissões de usuários e recursos. Administradores podem criar identidades, como usuários e grupos, e atribuir políticas de permissão relevantes para conceder acesso a novos usuários. Isso aumenta a segurança do ambiente de computação em nuvem, garantindo que os usuários tenham apenas as permissões necessárias para realizar suas tarefas.

---

## Pergunta 11

**Qual dos pilares do Well-Architected Framework foca em como podemos continuamente melhorar processos e procedimentos?**

- **✅** Excelência Operacional
    - O pilar Excelência operacional se concentra na execução e monitoramento de sistemas e na melhoria contínua de processos e procedimentos.

- Performance Eficiente
    - O pilar de eficiência de performance se concentra na alocação estruturada e simplificada de recursos de TI e computação.

- Confiabilidade
    - O pilar da confiabilidade se concentra nos workloads que executam as funções pretendidas e na recuperação rápida de falhas em atender demandas.

- Segurança
    - O pilar Segurança se concentra na proteção de informações e sistemas.

> **Explicação geral**:  
> A AWS Well-Architected ajuda arquitetos de nuvem a construir infraestruturas seguras, resilientes, eficientes e de alta performance para aplicações e workloads. Baseada em seis pilares, incluindo a Excelência Operacional, ela fornece uma abordagem consistente para avaliar arquiteturas e implementar designs que podem se expandir com o tempo. Essa metodologia não só aumenta a qualidade das implementações, mas também assegura que as arquiteturas possam evoluir e escalar conforme as necessidades mudam.

---

## Pergunta 12

**O design dos dados de uma aplicação incorpora uma base de dados relacional, que será utilizada pontual e imprevisivelmente, uma vez que o AWS Elastic Cache também será empregado para minimizar o acesso aos dados. Em termos de economia, qual seria o tipo recomendado de instância de banco de dados neste cenário?**

- **✅** On Demand
    - Em termos de economia, a instância de banco de dados recomendada para este cenário seria uma instância sob demanda (on demand). Isso se deve ao uso pontual e imprevisível da base de dados, onde pagar apenas pelo tempo de uso efetivo oferece um custo-benefício melhor comparado a instâncias reservadas ou dedicadas.

- Dedicated Hosts
    - Os Dedicated Hosts são geralmente mais caros do que as instâncias Sob Demanda, pois oferecem servidores físicos dedicados exclusivamente para o seu uso.

- Spot
    - Embora ofereça maior economia, o plano Spot é recomendado para cargas de trabalho que podem tolerar interrupções, não sendo ideal para uso imprevisível e pontual de banco de dados.

- Reserved
    - Instâncias Reservadas são indicadas para casos onde é possível prever o uso em períodos de 1 ou 3 anos, permitindo economias significativas com pagamento adiantado.

> **Explicação geral**:  
> O AWS RDS oferece opções de preços como Sob Demanda, Instâncias Reservadas e Spot, cada uma adequada a diferentes padrões de uso. As instâncias Sob Demanda são ideais para cargas de trabalho imprevisíveis, permitindo pagar apenas pelo tempo de uso efetivo. As instâncias Reservadas são mais econômicas para cargas de trabalho estáveis e previsíveis, enquanto o Spot é mais adequado para cargas de trabalho que podem tolerar interrupções.

---

## Pergunta 13

**Uma startup deseja disponibilizar uma aplicação no endereço www.simuladoudemy.com. Qual serviço pode ser empregado para criar esse domínio?**

- **✅** Route 53
    - O serviço Amazon Route 53 é utilizado para registrar e gerenciar domínios, permitindo criar e configurar o domínio www.simuladoudemy.com.

- API Gateway
    - O API Gateway é utilizado para o gerenciamento de APIs, não para o registro de domínios.

- Auto Scalling
    - O Auto Scaling é utilizado para ajustar automaticamente o número de instâncias necessárias para suportar a carga de trabalho, não para registrar domínios.

- S3
    - O S3 pode ser habilitado para hospedar um site estático, mas não para criar ou gerenciar domínios.

> **Explicação geral**:  
> O Amazon Route 53 é um serviço de DNS escalável que permite registrar e gerenciar domínios. Ele traduz nomes de domínio em endereços IP e configura registros DNS para direcionar o tráfego para os recursos desejados, como servidores web ou balanceadores de carga.

---

## Pergunta 14

**Uma organização precisa de uma aplicação que requer 10 instâncias EC2 ativas para suportar diversos usuários logados. Qual serviço da AWS oferece um mecanismo para distribuir as requisições de forma equilibrada entre essas instâncias?**

- **✅** AWS Elastic Load Balancing (ELB)
    - O AWS Elastic Load Balancing (ELB) oferece um mecanismo para distribuir as requisições de forma equitativa entre instâncias ativas do EC2.

- Auto Scalling
    - Um Auto Scaling Group ajusta automaticamente o número de instâncias EC2 em resposta à demanda, mas não distribui o tráfego.

- Security Group
    - Security Groups controlam o tráfego de entrada e saída das instâncias EC2, mas não distribuem o tráfego.

- Amazon Route 53
    - O Amazon Route 53 roteia o tráfego para recursos na AWS, mas a distribuição de carga entre instâncias é feita pelo ELB.

> **Explicação geral**:  
> O Elastic Load Balancing (ELB) distribui o tráfego entre várias instâncias EC2 ou recursos, garantindo alta disponibilidade e escalabilidade. Existem tipos de ELB, como Application Load Balancer (ALB) e Network Load Balancer (NLB), que atendem diferentes tipos de tráfego e necessidades de desempenho.

---

## Pergunta 15

**Uma empresa pretende incorporar testes automatizados em seu fluxo de desenvolvimento. Qual serviço da AWS pode ser empregado para atender a essa necessidade?**

- **✅** AWS CodeBuild
    - O AWS CodeBuild é um serviço gerenciado de compilação e teste contínuos que automatiza a criação, teste e validação de código-fonte.

- AWS CodeTest
    - O AWS CodeTest não existe.

- AWS CodeDeploy
    - O AWS CodeDeploy é um serviço de implantação que automatiza implantações de software, não testes.

- AWS CodePipeline
    - O AWS CodePipeline é um serviço de entrega contínua que automatiza pipelines de liberação, integrando outras ferramentas de CI/CD, mas não realiza testes diretamente.

> **Explicação geral**:  
> O AWS CodeBuild automatiza a construção e os testes do código-fonte, integrando-se bem com outras ferramentas de CI/CD, como o AWS CodePipeline. Ele permite criar e testar código continuamente, facilitando a integração e a entrega contínuas de software.

---

## Pergunta 16

**A AWS é uma infraestrutura cloud global segura, extensível e confiável e que oferece mais de 200 serviços em diversos países ao redor do mundo. Sobre sua distribuição no mundo, podemos afirmar que?**

- **✅** É atualmente composta por 33 regiões, que estão divididas em aproximadamente 105 zonas de disponibilidade (AZ).
    - Uma Região AWS é uma área geográfica que contém várias Zonas de Disponibilidade (AZs), garantindo alta disponibilidade e resiliência.

- É atualmente composta por 20 regiões, que estão divididas em aproximadamente 100 zonas de disponibilidade (AZ).
    - A AWS possui mais regiões e zonas de disponibilidade do que os números mencionados nesta opção.

- É atualmente composta por 15 regiões, que estão divididas em aproximadamente 80 zonas de disponibilidade (AZ).
    - A AWS tem mais regiões e zonas de disponibilidade do que os números mencionados nesta opção.

- É atualmente composta por 25 regiões, que estão divididas em aproximadamente 90 zonas de disponibilidade (AZ).
    - A AWS tem mais regiões e zonas de disponibilidade do que os números mencionados nesta opção.

> **Explicação geral**:  
> A AWS possui uma infraestrutura global extensa e resiliente, com uma distribuição ampla de regiões e zonas de disponibilidade para garantir alta disponibilidade e reduzir a latência. O número de regiões e zonas de disponibilidade continua a crescer, refletindo a expansão contínua da AWS em termos de cobertura global e capacidade de serviço.

---

## Pergunta 17

**A equipe de TI de uma plataforma de vídeos foi incumbida de desenvolver um procedimento para possibilitar a geração de legendas automáticas em todos os vídeos disponíveis na plataforma. Qual serviço pode ajudá-los nessa tarefa?**

- **✅** Amazon Transcribe
    - O Amazon Transcribe pode ajudá-los a desenvolver um procedimento para a geração automática de legendas em todos os vídeos disponíveis na plataforma.

- Amazon Translate
    - O Amazon Translate é um serviço de tradução automática neural que fornece traduções de idiomas com rapidez, alta qualidade, acessíveis e personalizáveis. A tradução automática neural é um tipo de automação de tradução de idiomas que usa modelos de aprendizado profundo para entregar traduções que soam mais precisas e naturais do que as oferecidas por algoritmos de tradução tradicionais estatísticos e baseados em regras.

- Amazon Polly
    - O Amazon Polly é um serviço de nuvem que converte texto em fala realista. Você pode usar o Amazon Polly para desenvolver aplicações que aumentam o envolvimento e a acessibilidade.

- Amazon Lex
    - O Amazon Lex é um serviço da AWS para a criação de interfaces de conversa para qualquer aplicativo que usa voz e texto. Com o Amazon Lex, o mesmo mecanismo de conversa da plataforma do Amazon Alexa agora está disponível para todos os desenvolvedores, permitindo que você crie chatbots sofisticados em linguagem natural em aplicativos novos e existentes.

> **Explicação geral**:  
> O Amazon Transcribe é um serviço de reconhecimento automático de fala (ASR) que converte áudio em texto. Ele pode ser usado para gerar legendas automáticas em vídeos, facilitando a acessibilidade e a busca de conteúdo. O serviço suporta vários idiomas e oferece uma alta precisão na transcrição. Além disso, ele pode identificar e marcar diferentes palestrantes, o que é útil para vídeos com múltiplos participantes. O Amazon Transcribe pode ser integrado facilmente à plataforma de vídeos para processar automaticamente os arquivos de vídeo e gerar legendas. Esse procedimento melhora a experiência do usuário e atende a requisitos de acessibilidade.

---

## Pergunta 18

**Para atender às necessidades de uma área de auditoria e conformidade, é essencial assegurar a manutenção e monitoramento das configurações ideais de serviços e sistemas.Qual serviço da AWS pode ser empregado para esse tipo de gerenciamento?**

- **✅** AWS Config
    - O AWS Config é o serviço ideal para monitorar e manter configurações de serviços e sistemas, assegurando conformidade e auditoria contínua.

- Amazon GuardDuty
    -O Amazon GuardDuty é um serviço de detecção de ameaças que monitora continuamente e analisa dados de rede e atividade de conta na AWS para identificar comportamentos suspeitos e potenciais ameaças de segurança. Ele ajuda a proteger recursos na nuvem com insights acionáveis e alertas de segurança automatizados.

- AWS CloudTrail
    - O AWS CloudTrail registra e monitora atividades de API e ações na conta AWS, ajudando em auditorias e segurança. O AWS Config avalia e monitora configurações de recursos, garantindo conformidade e rastreamento de mudanças na infraestrutura. CloudTrail foca em ações e usuários, enquanto Config foca em estados de configuração dos recursos.

- AWS Identity and Access Management (IAM)
    - O AWS Identity and Access Management (IAM) permite gerenciar de forma segura o acesso aos serviços e recursos da AWS. Com ele, é possível criar e controlar permissões detalhadas para usuários, grupos e roles, garantindo que cada identidade tenha acesso apenas aos recursos necessários.

> **Explicação geral**:  
> O AWS Config é um serviço da AWS que fornece monitoramento e gerenciamento contínuo dos recursos e configurações da sua conta. Ele rastreia alterações em recursos, registra conformidade com políticas e cria snapshots do estado da infraestrutura ao longo do tempo. O AWS Config ajuda a manter a conformidade, a identificar e remediar desvios de configuração, além de possibilitar a auditoria e a análise de alterações. Com regras de avaliação personalizáveis, ele ajuda a automatizar a verificação de conformidade e a segurança dos recursos da AWS, melhorando a governança e a segurança da nuvem.

---

## Pergunta 19

**A equipe de Tecnologia da Informação de uma startup utiliza o AWS Device Farm para agilizar o ciclo de desenvolvimento de aplicativos. De que forma este serviço contribui para alcançar esse objetivo?**

- Fornecendo um ambiente de desenvolvimento integrado via Browser
    - Explicação: Essa função é do Cloud9.

- **✅** Permitindo testes em paralelo em vários dispositivos.
    - Explicação: O AWS Device Farm é um serviço da Amazon Web Services (AWS) que permite aos desenvolvedores testar seus aplicativos móveis de forma eficiente em uma ampla variedade de dispositivos reais e emuladores.

- Fornecendo um conjunto de ferramentas, bibliotecas e documentação que permitem aos desenvolvedores criar aplicativos para uma plataforma específica.
    - Explicação: Essa função é do SDK.

- Realizando testes unitários dos aplicativos numa esteira de CI/CD
    - Explicação: Essa função é do CodeBuild.

> **Explicação geral**:  
> O AWS Device Farm é um serviço da Amazon Web Services (AWS) que permite aos desenvolvedores testar seus aplicativos móveis de forma eficiente em uma ampla variedade de dispositivos reais e emuladores. Ele oferece um ambiente de teste escalável, onde os aplicativos podem ser submetidos a testes de interface do usuário, desempenho e segurança. Com o Device Farm, os desenvolvedores podem identificar problemas de compatibilidade, erros de funcionamento e melhorar a qualidade geral de seus aplicativos antes de lançá-los no mercado. Ele ajuda a acelerar o processo de desenvolvimento, economizar tempo e recursos, além de garantir que os aplicativos funcionem de maneira confiável em diversos dispositivos móveis e plataformas.

---

## Pergunta 20

**Qual é o serviço da AWS que permite aos desenvolvedores se concentrarem apenas na codificação, enquanto automatiza o provisionamento de infraestrutura, balanceamento de carga, monitoramento e implantação? Este serviço também suporta codificação em várias linguagens, incluindo .Net, Java, PHP, Node.js, Python, Ruby e Go, entre outras?**

- AWS CodeDeploy
    - Explicação: O AWS CodeDeploy é um serviço totalmente gerenciado de implantação que automatiza implantações de software em diversos serviços de computação como Amazon EC2, AWS Fargate, AWS Lambda e servidores locais.

- AWS Fargate
    - Explicação: O AWS Fargate é um mecanismo de computação sem servidor para contêineres.

- Amazon ECS
    - Explicação: O Amazon Elastic Container Service (Amazon ECS) é um serviço totalmente gerenciado de orquestração de contêineres que ajuda a implantar, gerenciar e escalar facilmente aplicações conteinerizadas.

- **✅** AWS Elastic Beanstalk
    - Explicação: O AWS Elastic Beanstalk é o serviço que simplifica a gestão da infraestrutura, balanceamento de carga, monitoramento e implantação de aplicações. Ele permite que desenvolvedores se concentrem no código e oferece suporte a várias linguagens de programação como .Net, Java, PHP, Node.js, Python, Ruby e Go.

> **Explicação geral**:  
> O AWS Elastic Beanstalk é uma plataforma de orquestração de serviços oferecida pela AWS que automatiza o provisionamento de infraestrutura necessária para executar aplicações, além de gerenciar balanceamento de carga, escalabilidade, monitoramento e implantação. Este serviço permite que os desenvolvedores se concentrem exclusivamente no desenvolvimento do código, sem a necessidade de se preocupar com a configuração e manutenção da infraestrutura subjacente. Suporta uma ampla variedade de linguagens de programação, incluindo .Net, Java, PHP, Node.js, Python, Ruby e Go, entre outras. Com o Elastic Beanstalk, é possível realizar o deploy de aplicações de maneira rápida e eficiente, aproveitando a flexibilidade e a escalabilidade da nuvem AWS. Ele também integra-se facilmente com outros serviços da AWS, como RDS, S3 e CloudWatch, para oferecer uma solução completa de desenvolvimento e operação de aplicações.

---

## Pergunta 21

**Após avaliar diversos cenários para infraestrutura, uma empresa optou por não autorizar o uso de computação compartilhada. No entanto, ela busca uma solução na AWS que preserve as características de simplicidade, agilidade e elasticidade, enquanto utiliza servidores físicos dedicados. Qual serviço atende a essa necessidade?**

- EC2 reservados
    - Explicação: O EC2 não é recomendado nesse cenário porque a empresa busca evitar computação compartilhada, e EC2 padrão utiliza infraestrutura compartilhada. Para manter simplicidade, agilidade, elasticidade e servidores físicos dedicados, a empresa deve considerar AWS Dedicated Hosts.

- Hosts spot
    - Explicação: Hosts Spot não existem porque os hosts dedicados são provisionados para uso exclusivo por um único cliente, garantindo controle total sobre o hardware. Spot Instances, por outro lado, utilizam capacidade não utilizada da AWS e podem ser interrompidas com pouca antecedência, o que não se alinha ao conceito de exclusividade e controle completo dos hosts dedicados.

- **✅** Hosts dedicados
    - Explicação: Hosts Dedicados na AWS são servidores físicos isolados que podem ser usados para executar instâncias de máquinas virtuais. Eles oferecem controle total sobre a alocação de recursos, permitindo que você atenda a requisitos de conformidade e licenciamento.

- EC2 dedicados
    - Explicação: Este modelo de uso não existe, além disso, o EC2 não é recomendado nesse cenário porque a empresa busca evitar computação compartilhada, e EC2 padrão utiliza infraestrutura compartilhada.

> **Explicação geral**:  
> Hosts Dedicados são ideais para cargas de trabalho que precisam de isolamento total, como bancos de dados sensíveis ou ambientes licenciados por núcleo. Eles oferecem visibilidade granular de recursos, controle de capacidade e previsibilidade de desempenho. No entanto, o uso de Hosts Dedicados pode ser mais caro do que o modelo de instâncias virtuais compartilhadas, como EC2.

---

## Pergunta 22

**Um dos princípios dos 12 fatores para aplicações web em nuvem é preservar o cache de sessões de estado do usuário fora da memória das instâncias EC2. Qual serviço é mais indicado para cumprir esse propósito?**

- Amazon S3
    - Explicação: O S3 é o serviço de armazenamento padrão de objetos (arquivos + metadados) da AWS.

- Amazon EBS
    - Explicação: O EBS fornece block storage para as instâncias EC2.

- Amazon EventBridge
    - Explicação: O EventBridge é um barramento de eventos para diversos serviços e aplicações da AWS.

- **✅** Amazon ElasticCache for Redis
    - Explicação: O Amazon ElastiCache for Redis é utilizado para acelerar o desempenho de aplicativos, armazenando dados frequentemente acessados em cache na memória.

> **Explicação geral**:  
> Os 12 Fatores são princípios para desenvolver aplicações SaaS escaláveis e facilmente mantidas. Um desses princípios enfatiza a necessidade de processos sem estado, o que implica armazenar dados de sessão fora das instâncias de aplicação. Armazenar dados de sessão localmente pode levar à perda de dados e inconsistências quando escalando ou substituindo instâncias.  
> O Amazon ElastiCache Redis oferece uma solução para armazenar dados de sessão centralmente, garantindo persistência, alta disponibilidade e baixa latência. Redis permite a replicação e o failover automático, suportando uma experiência de usuário consistente e confiável. Utilizando ElastiCache Redis, as aplicações podem escalar horizontalmente e manter alta performance, alinhando-se aos princípios dos 12 Fatores.

---

## Pergunta 23

**Qual é a maneira mais fácil de lançar rapidamente milhares de contêineres em uma ampla variedade de opções de computação da AWS, usando o seu CI/CD e ferramentas de automação de sua preferência?**

- Com o Amazon CodePipeline
    - Explicação: O AWS CodePipeline é utilizado para a implementação de uma esteira de CI/CD de desenvolvimento de aplicativos.

- **✅** Com o Amazon ECS
    - Explicação: O Amazon Elastic Container Service (ECS) oferece integração com várias ferramentas de CI/CD, permitindo a orquestração eficiente e escalável de contêineres em serviços como EC2 e AWS Fargate.

- Com o Amazon Lambda
    - Explicação: O Lambda é utilizado para implementar funções sem servidor na AWS.

- Com o Amazon EC2
    - Explicação: O EC2 é usado para implementar diversos tipos de máquinas para aplicações na AWS e serve como base para o ECS. No entanto, o gerenciamento dessas máquinas para contêineres é facilitado pelo ECS, que simplifica o uso de contêineres na AWS. Embora seja possível gerenciar contêineres manualmente no EC2, isso se torna muito mais trabalhoso sem a automação e orquestração fornecidas pelo ECS.

> **Explicação geral**:  
> O Amazon Elastic Container Service (ECS) é um serviço de gerenciamento de contêineres altamente escalável e de alta performance da AWS. Ele facilita a execução e a escalabilidade de aplicações baseadas em contêineres, permitindo que os desenvolvedores concentrem-se em criar e manter suas aplicações em vez de gerenciar a infraestrutura subjacente. O ECS suporta integrações com outros serviços da AWS, como IAM, ELB, e CloudWatch, proporcionando segurança e monitoramento robustos. Ele pode ser executado tanto em instâncias EC2 quanto no AWS Fargate, que oferece execução de contêineres sem gerenciamento de servidores. Além disso, o ECS se integra bem com pipelines de CI/CD, facilitando a automação do ciclo de vida de desenvolvimento de software. Com o ECS, é possível lançar e gerenciar milhares de contêineres de forma eficiente, otimizando a utilização de recursos e acelerando o tempo de desenvolvimento e implantação.

---

## Pergunta 24

**Qual é a opção abaixo que faz uso da infraestrutura das Redes de Borda (EdgeLocations) e Pontos de Presença para transferir em alta velocidade arquivos entre S3 Buckets?**

- Amazon CloudFront
    - Explicação: O Amazon CloudFront é um serviço de CDN (Content Delivery Network) projetado para distribuir conteúdo web com baixa latência.

- AWS Snow
    - Explicação: O AWS Snowball é um serviço de transferência de dados em massa que utiliza dispositivos físicos para mover grandes volumes de dados para dentro e fora da AWS, facilitando migrações e backup de dados com segurança e eficiência, especialmente quando a conectividade de rede é limitada ou lenta.

- AWS VPN
    - Explicação: A AWS VPN (Virtual Private Network) permite a criação de conexões seguras e criptografadas entre sua rede local ou dispositivos remotos e a infraestrutura da AWS. Ela oferece dois tipos de VPN: Site-to-Site VPN, para conectar redes on-premises a redes AWS, e Client VPN, para conectar usuários individuais de forma segura à rede AWS.

- **✅** Transfer Accelerations
    - Explicação: O Transfer Acceleration do Amazon S3 que otimiza a transferência de arquivos utilizando a rede global da AWS para acelerar a movimentação de dados para e entre buckets S3.

> **Explicação geral**:  
> O Amazon S3 Transfer Acceleration é um recurso do Amazon S3 que utiliza a rede global da AWS para acelerar a transferência de arquivos de e para buckets S3. Ele é especialmente útil para transferências de longa distância, como ao mover dados entre continentes. Transfer Acceleration redireciona os uploads e downloads por meio de pontos de presença (edge locations) da AWS, otimizando a rota e reduzindo a latência. Esse recurso melhora significativamente a velocidade de transferência de grandes volumes de dados, tornando-o ideal para aplicações que exigem movimentação rápida e eficiente de dados. Ele pode ser ativado com um simples ajuste nas configurações do bucket S3, proporcionando uma solução poderosa e fácil de usar para otimização de transferências.

---

## Pergunta 25

**Qual recurso da AWS permite o gerenciamento dos serviços através de uma interface web?**

- **✅** AWS Management Console
    - Explicação: O AWS Management Console é uma interface baseada na web que permite aos usuários interagir e gerenciar serviços da AWS de forma intuitiva.

- AWS CloudFormation
    - Explicação: O AWS CloudFormation é um serviço que permite modelar e provisionar a infraestrutura AWS como código, facilitando a criação, atualização e gerenciamento de recursos AWS de forma automatizada e repetível. Ele usa templates para definir os recursos e suas dependências, proporcionando consistência e controle nas implantações.

- AWS CloudWatch
    - Explicação: AWS CloudWatch serve para monitorar e gravar log de diversos serviços da AWS e de aplicações desenvolvidas pelos clientes.

- AWS Software Development Kit (SDK)
    - Explicação: AWS SDK fornece diversas bibliotecas para integração a IDE de diversas linguagens de programação integrando com mais facilidade o desenvolvedor com os serviços da AWS. Ex. Java, C#, Node, Python, entre outras.

> **Explicação geral**:  
> O AWS Management Console é uma interface baseada na web que permite aos usuários interagir e gerenciar serviços da AWS de forma intuitiva. Ele oferece uma visão unificada dos recursos, permitindo criar, configurar e monitorar serviços sem a necessidade de linha de comando. Com uma interface amigável, o Console facilita a administração de recursos, o gerenciamento de permissões, o monitoramento de métricas e o acesso a recursos de aprendizado. Isso agiliza as tarefas de gerenciamento e configuração, mesmo para usuários sem conhecimento técnico profundo.

---

## Pergunta 26

**Qual é a principal função do Security Group?**

- Proteger dados de comunicação em trânsito
    - Explicação: Security Groups controlam o acesso ao tráfego de rede, mas não criptografam os dados em trânsito. A proteção de dados em trânsito é realizada utilizando protocolos de criptografia como TLS/SSL, implementados nos serviços e aplicativos em execução nas instâncias EC2. O AWS Certificate Manager (ACM) facilita a obtenção, implantação e gerenciamento de certificados SSL/TLS, garantindo comunicações seguras.

- Promover e gerenciar a escalabilidade automática de instâncias EC2 com base na demanda e nas políticas definidas.
    - Explicação: Security Groups não promovem auto scaling de instâncias EC2. O auto scaling é gerenciado pelo serviço AWS Auto Scaling, que ajusta automaticamente a capacidade de computação com base na demanda e nas políticas definidas.

- **✅** Atuar como uma espécie de firewall para controlar a autorização do tráfego de entrada e saída de máquinas EC2 que estejam associados a ele.
    - Explicação: A principal função do Security Group na AWS é atuar como um firewall virtual para controlar o tráfego de entrada e saída das instâncias EC2. Ele define regras que permitem ou bloqueiam tráfego com base em endereços IP, portas e protocolos, garantindo a segurança das instâncias ao restringir o acesso a apenas fontes e destinos autorizados.

- Criar rotas de tráfego entre subredes de uma VPC
    - Explicação: Security Groups não criam ou gerenciam rotas de tráfego entre subredes. Isso é feito através das tabelas de rotas em uma VPC, configuradas para controlar como os pacotes são encaminhados entre as subredes e outros recursos de rede.

> **Explicação geral**:  
> Security Groups na AWS atuam como firewalls virtuais, controlando o tráfego de entrada e saída para instâncias EC2 com base em regras definidas. Eles permitem ou bloqueiam tráfego por endereço IP, porta e protocolo, assegurando que apenas fontes e destinos autorizados possam acessar as instâncias. Security Groups são stateful, o que significa que as respostas ao tráfego permitido de entrada são automaticamente permitidas a sair. Esses grupos são integrados com vários serviços da AWS, incluindo Amazon RDS, Elastic Load Balancing (ELB), e AWS Lambda, garantindo a segurança e o controle de acesso em diferentes partes da infraestrutura na nuvem. Essa integração facilita a aplicação consistente de políticas de segurança em todo o ambiente AWS.

---

## Pergunta 27

**Qual serviço da AWS é recomendado na implementação e no gerenciamento de banco de dados relacionais?**

- AWS KMS
    - Explicação: O AWS Key Management Service (KMS) facilita a criação e o gerenciamento de chaves criptográficas e o controle do seu uso em uma ampla variedade de serviços da AWS e em seus aplicativos.

- **✅** Amazon RDS
    - Explicação: O Amazon Relational Database Service (RDS) é uma coleção de serviços gerenciados que facilita a configuração, operação e escalabilidade de bancos de dados relacionais na nuvem.

- AWS DMS
    - Explicação: O AWS Database Migration Service (AWS DMS) ajuda você a migrar bancos de dados para a AWS de modo rápido e seguro.

- DynamoDB
    - Explicação: O Amazon DynamoDB é um banco de dados de valores-chave e documentos que oferece desempenho em milissegundos de um dígito em qualquer escala. É um banco de dados totalmente gerenciado, multirregional, multiativo e durável com segurança, backup e restauração integrados e armazenamento em cache na memória para aplicativos em escala de Internet.

> **Explicação geral**:  
> O Amazon Relational Database Service (RDS) é uma coleção de serviços gerenciados que facilita a configuração, operação e escalabilidade de bancos de dados na nuvem. Ele suporta vários mecanismos de banco de dados, incluindo Amazon Aurora compatível com MySQL, Amazon Aurora compatível com PostgreSQL, MySQL, MariaDB, PostgreSQL, Oracle e SQL Server. O RDS automatiza tarefas administrativas como provisionamento de hardware, configuração do banco de dados, patching e backups, permitindo que os usuários se concentrem em suas aplicações. Ele também oferece alta disponibilidade e recuperação de desastres com opções Multi-AZ e réplicas de leitura. Além disso, o Amazon RDS pode ser implantado on-premises com o Amazon RDS on AWS Outposts, fornecendo uma solução de banco de dados gerenciada que se estende ao seu data center local, garantindo consistência na gestão e operação dos bancos de dados, tanto na nuvem quanto on-premises.

---

## Pergunta 28

**Qual é a melhor maneira de manter aplicações resilientes na infraestrutura da AWS?**

- Implementar o Amazon CloudFront
    - Explicação: O uso do CloudFront ajuda a melhorar a performance na distribuição de conteúdo. No entanto, se a origem da informação estiver em uma única zona de disponibilidade (AZ) e esta ficar indisponível, a aplicação poderá ser impactada, mesmo com o uso do CloudFront.

- **✅** Distribuir as instâncias em mais de uma zona de disponibilidade
    - Explicação: As boas práticas orientam a distribuir os recursos em zonas de disponibilidade diferentes. Se ocorrer problema em uma delas, as outras devem responder as demandas da aplicação com o mínimo impacto possível.

- Distribuir as instâncias em duas VPCs diferentes e dentro da mesma zona de disponibilidade
    - Explicação: Distribuir as instâncias em duas VPCs diferentes dentro da mesma zona de disponibilidade não garante a resiliência. Se a AZ ficar indisponível, ambas as VPCs serão afetadas, impactando a aplicação.

- Utilizar o Auto Scaling para subir uma nova máquina sempre que alguma cair.
    - Explicação: Utilizar o Auto Scaling para subir uma máquina quando outra cai garante a disponibilidade de um recurso e escalabilidade. Entretanto, se todas as instâncias estiverem em uma única zona de disponibilidade (AZ) que apresenta problemas, há o risco de a aplicação ficar indisponível.

> **Explicação geral**:  
> As boas práticas de distribuição de recursos em diferentes zonas de disponibilidade (AZs) contribuem significativamente para a disponibilidade e resiliência das aplicações. Ao alocar recursos em múltiplas AZs, você cria redundância, garantindo que se uma AZ enfrentar problemas, as outras possam continuar operando e atendendo às demandas da aplicação com o mínimo impacto possível. A resiliência é aumentada, pois o sistema pode se recuperar rapidamente de falhas, e a disponibilidade é mantida, assegurando que o serviço permaneça acessível aos usuários. Essa abordagem minimiza interrupções e assegura uma experiência de usuário consistente, mesmo diante de falhas ou interrupções em uma das zonas de disponibilidade. Em resumo, a distribuição em AZs é uma estratégia essencial para construir sistemas robustos e confiáveis na nuvem.

---

## Pergunta 29

**Um desenvolvedor deseja acessar os serviços da AWS enquanto programa em seu computador. Qual serviço é utilizado dentro do código da aplicação para interagir com os serviços da AWS?**

- AWS Workspaces
    - Explicação: O AWS Workspaces oferece desktops virtuais Windows e Linux de acordo com a necessidade.

- **✅** AWS SDKs
    - Explicação: O AWS SDK (Software Development Kit) é a ferramenta que permite aos desenvolvedores acessar os serviços da AWS diretamente de seu código de aplicação.

- AWS CLI
    - Explicação: O AWS CLI é o serviço utilizado para acessar e gerenciar os serviços da AWS através da linha de comando.

- AWS Console Manager
    - Explicação: O AWS Console Manager é a interface web utilizada para gerenciar todos os serviços da AWS.

> **Explicação geral**:  
> O AWS SDK (Software Development Kit) é um conjunto de ferramentas que permite aos desenvolvedores integrar serviços da AWS diretamente em seus aplicativos. Ele fornece bibliotecas e APIs específicas para várias linguagens de programação, como Python, Java, e JavaScript, facilitando a comunicação com os serviços da AWS e a implementação de funcionalidades avançadas. Já o AWS Toolkit é uma extensão ou plugin que se instala em IDEs, como IntelliJ, Visual Studio Code e Eclipse, oferecendo suporte para desenvolvimento, gerenciamento e depuração de aplicações AWS diretamente no ambiente de desenvolvimento. Enquanto o SDK é utilizado para interagir programaticamente com a AWS, o Toolkit oferece uma interface gráfica e funcionalidades integradas para facilitar o desenvolvimento e a integração com os serviços da AWS.

---

## Pergunta 30

**Qual serviço da AWS faz recomendações para a otimização de segurança dos seus recursos?**

- IAM
    - Explicação: IAM (Identity and Access Management) é um serviço da AWS que gerencia permissões e controle de acesso a recursos, permitindo a criação de usuários e grupos com políticas de acesso detalhadas para proteger e organizar o ambiente na nuvem.

- **✅** Trusted Advisor
    - Explicação: O AWS Trusted Advisor fornece recomendações em tempo real para otimizar infraestruturas na AWS, melhorando segurança, performance e eficiência de custos. Ele verifica a conta da AWS em várias categorias, como otimização de custos, performance, segurança, tolerância a falhas e limites de serviço, oferecendo conselhos práticos para aprimorar suas operações.

- MFA
    - Explicação: MFA (Autenticação Multifator) é um recurso de segurança que adiciona uma camada extra de proteção, exigindo que os usuários forneçam dois ou mais métodos de autenticação, como senha e um código temporário, ao acessar recursos da AWS.

- Security Group
    - Explicação: Security Group atua como um firewall virtual para instâncias EC2, controlando o tráfego de entrada e saída baseado em regras definidas, garantindo a segurança e o controle granular sobre as comunicações na rede.

> **Explicação geral**:  
> O AWS Trusted Advisor é um serviço que fornece recomendações em tempo real para ajudar a otimizar suas infraestruturas da AWS, melhorando a segurança, a performance e a eficiência de custos. Ele verifica sua conta da AWS em relação às melhores práticas em várias categorias, incluindo:
> 
> - Otimização de Custos: Identifica oportunidades para reduzir gastos, como instâncias EC2 subutilizadas ou recursos não utilizados.
> - Performance: Sinaliza áreas onde a performance pode ser melhorada, como balanceamento de carga e throughput de armazenamento.
> - Segurança: Aponta vulnerabilidades de segurança e oferece recomendações para melhorar a segurança, como permissões excessivas ou falta de autenticação multifator (MFA).
> - Tolerância a Falhas: Sugere melhorias para aumentar a resiliência e a disponibilidade dos seus recursos, como a configuração de backups automáticos e a distribuição de instâncias em múltiplas zonas de disponibilidade.
> - Limites de Serviço: Avisa sobre a proximidade de limites de serviço da AWS para evitar interrupções.
> 
> O Trusted Advisor oferece um conjunto abrangente de verificações e conselhos práticos para garantir que suas operações na AWS sejam eficientes e seguras.

---

## Pergunta 31

**Uma empresa está desenvolvendo um aplicativo para enviar e-mails de aniversário para mais de 1000 clientes diariamente. Qual serviço da AWS pode ser integrado a qualquer aplicativo para atender a esse requisito?**

- Amazon CloudWatch
    - Explicação: O Amazon CloudWatch monitora e coleta métricas e logs dos recursos da AWS, ajudando a observar e responder a mudanças de estado.

- Amazon Simple Notification Service (SNS)
    - Explicação: O Amazon SNS (Simple Notification Service) facilita o envio de notificações em tempo real para usuários e aplicações.

- **✅** Amazon Simple Email Service (SES)
    - Explicação: O Amazon Simple Email Service (SES) é o serviço ideal para ser integrado a um aplicativo que precisa enviar e-mails diariamente. Ele oferece uma plataforma escalável e econômica para envio de e-mails em massa, com alta entrega e flexibilidade para personalização.

- Amazon EventBridge
    - Explicação: O Amazon EventBridge permite a construção de arquiteturas orientadas a eventos, conectando aplicações usando eventos de fontes da AWS e aplicações SaaS.

> **Explicação geral**:  
> O Amazon Simple Email Service (SES) é um serviço da AWS que oferece uma maneira escalável e econômica de enviar e-mails. Ele permite o envio de e-mails transacionais, de marketing e outros tipos de mensagens para clientes. O SES oferece alta disponibilidade, escalabilidade automática e integração com outros serviços AWS. É possível utilizar o SES para disparar e-mails a partir de aplicativos ou sistemas, bem como criar campanhas de e-mail marketing personalizadas. Além disso, o SES oferece recursos para monitoramento de entregas e gerenciamento de reputação de IP, garantindo a capacidade de atingir a caixa de entrada dos destinatários.

---

## Pergunta 32

**Qual serviço oferece um grupo de ferramentas que podem ser usadas em conjunto ou individualmente para permitir que desenvolvedores de front-end da web e de dispositivos móveis criem aplicações seguras e escaláveis full-stack, com tecnologia desenvolvida pela AWS?**

- AWS BeanStalk
    - Explicação: O AWS Elastic Beanstalk é um serviço de fácil utilização para implantação e escalabilidade de aplicações e serviços da web desenvolvidos com Java, .NET, PHP, Node.js, Python, Ruby, Go e Docker em servidores familiares como Apache, Nginx, Passenger e IIS.

- AWS SDK
    - Explicação: AWS SDK permite que acesse e gerencie serviços da AWS com sua linguagem ou plataforma de desenvolvimento preferencial.

- AWS Fargate
    - Explicação: O AWS Fargate é um mecanismo de computação sem servidor para contêineres que funciona com o ECS e EKS.

- **✅** AWS Amplify
    - Explicação: O AWS Amplify oferece um conjunto de ferramentas que ajudam desenvolvedores de front-end a criar aplicações web e móveis seguras e escaláveis utilizando tecnologia da AWS.

> **Explicação geral**:  
> O Amplify é um conjunto de ferramentas e recursos que permite que desenvolvedores frontend desenvolvam para plataformas móveis e Web criem aplicações completas de forma rápida e fácil na AWS. Eles podem contar com a flexibilidade do uso de todos os serviços da AWS para se adaptar à evolução dos casos de uso. Com o Amplify, você pode configurar o backend de uma aplicação Web ou móvel e conectá-la em minutos, criar visualmente o frontend de uma IU para a Web e gerenciar facilmente o conteúdo da aplicação fora do Console AWS.

---


## Pergunta 33

**O departamento de marketing de uma empresa está elaborando uma campanha com duração de 12 meses. Antecipadamente, prevê-se um aumento no número de clientes no site, exigindo a adição de mais 3 instâncias EC2 para atender à demanda ao longo desse período. Qual tipo de instância apresentaria um custo mais vantajoso para esse cenário?**

- On Demand
    - Explicação: On demand oferece flexibilidade máxima sem compromissos antecipados, mas a um custo mais alto.

- Spot
    - Explicação: Spot permitem aproveitar a capacidade ociosa da AWS a preços reduzidos, mas sem garantias de disponibilidade contínua, sendo mais adequadas para cargas de trabalho que podem ser interrompidas.

- Dedicated Hosts
    - Explicação: Dedicated Hosts garantem isolamento físico e são ideais para necessidades de conformidade e licenciamento específico, mas podem ser mais caros e menos flexíveis do que outras opções.

- **✅** Reserved
    - Explicação: Nestes cenários com previsão de tempo de uso e processamento, o uso de instâncias reservadas gera uma economia de até 72% em comparação ao modelo sob demanda (on demand) para períodos de 1 a 3 anos.

> **Explicação geral**:  
> Em cenários onde há previsão de uso contínuo e processamento por longos períodos, o uso de instâncias reservadas no Amazon EC2 pode gerar economias de até 72% em comparação ao modelo sob demanda (on demand) para compromissos de 1 a 3 anos. Instâncias reservadas permitem que você pague antecipadamente por capacidade de computação com um custo reduzido, ideal para cargas de trabalho estáveis e previsíveis.
> 
> Quando se utilizam outros serviços de computação além do EC2, como AWS Fargate e AWS Lambda, o plano mais indicado seria o Saving Plans. O AWS Saving Plans oferece flexibilidade, pois aplica descontos ao uso de computação em todos esses serviços, independentemente da zona de disponibilidade ou região, proporcionando uma economia geral baseada no compromisso de uso por 1 ou 3 anos.

---

## Pergunta 34

**Uma organização possui uma aplicação hospedada no EC2 que requer o envio de notificações para outras aplicações e serviços com base em eventos. Qual dos serviços abaixo é mais apropriado para atender a essa necessidade?**

- Amazon Simple Email Service (SES)
    - Explicação: O Amazon Simple Email Service (SES) é um serviço em nuvem de e-mail eficaz, flexível e dimensionável. Com ele, os desenvolvedores podem enviar e-mails de qualquer aplicação.

- **✅** Amazon Simple Notification Service (SNS)
    - Explicação: O Amazon Simple Notification Service (SNS) é o serviço mais apropriado para essa necessidade, pois permite o envio de notificações em tempo real para outras aplicações e serviços com base em eventos. Ele suporta diversos protocolos, incluindo HTTP/HTTPS, email, SMS e AWS Lambda.

- Amazon Simple Queue Service (SQS)
    - Explicação: O Amazon Simple Queue Service (SQS) é um serviço de filas de mensagens gerenciado que permite o desacoplamento e a escalabilidade de microsserviços, sistemas distribuídos e aplicações sem servidor. O SQS elimina a complexidade e a sobrecarga associadas ao gerenciamento e à operação de middleware orientado a mensagens, além de permitir que os desenvolvedores se dediquem a criar diferenciais.

- Amazon CloudWatch
    - Explicação: O Amazon CloudWatch é um serviço de monitoramento e observação que fornece dados e insights práticos para monitorar aplicativos, responder às alterações de performance em todo o sistema, otimizar a utilização de recursos e obter uma visualização unificada da integridade operacional.

> **Explicação geral**:  
> O Amazon Simple Notification Service (SNS) é ideal para enviar notificações em tempo real de uma aplicação baseada em eventos. Ele implementa um modelo de publicação/assinatura (pub/sub), onde as mensagens são publicadas em tópicos e entregues a todos os assinantes desses tópicos. Os assinantes podem incluir diversos sistemas e serviços, como endpoints HTTP/HTTPS, filas SQS, funções Lambda, emails e mensagens SMS. Isso permite uma integração fácil e flexível com novos sistemas, facilitando a expansão e atualização da arquitetura de notificações da aplicação. O SNS também garante alta disponibilidade e entrega durável de mensagens, assegurando que as notificações sejam recebidas mesmo em caso de falhas temporárias nos serviços.

---

## Pergunta 35

**Uma empresa precisa implementar métodos em suas contas para facilitar a concessão de acessos aos times de desenvolvimento e aos novos colaboradores que ingressarem. Como isso pode ser realizado?**

- Utilizando o AWS Federation para criar um grupo de desenvolvedores e gerenciar todos os seus acessos.
    - Explicação: O AWS Federation não existe, entretanto, acessos Federados (Federation) são utilizados para integrar processos de autenticação de terceiros com a AWS. Ex. Google, Facebook, Apple, etc. Este podem ser implementados com o Amazon Cognito.

- Utilizando o AWS SDK para criar um grupo de desenvolvedores e gerenciar todos os seus acessos.
    - Explicação: O AWS SDK é uma plataforma de desenvolvimento que acelera o processo de desenvolvimento de software na AWS, apesar disso, o acesso tem que ser concedido pelo IAM.

- Utilizando o IAM Roles para criar um grupo de desenvolvedores e gerenciar todos os seus acessos.
    - Explicação: Funções (Roles) são tipos de identidades criados no IAM para que as aplicações ou serviços possam recebem autorização para acessar outras aplicações ou serviços.

- **✅** Utilizando o AWS IAM Grupos para criar um grupo de desenvolvedores e gerenciar todos os seus acessos.
    - Explicação: Para facilitar a concessão de acessos, a empresa pode utilizar AWS IAM Grupos. Criar grupos para diferentes equipes (como Desenvolvimento, DevOps, Arquitetura) e anexar políticas de permissão apropriadas a cada grupo. Adicionar novos colaboradores aos grupos correspondentes para conceder os acessos necessários de forma eficiente.

> **Explicação geral**:  
> O AWS IAM Grupos permite criar grupos para gerenciar e agilizar a concessão de acessos a diferentes perfis de colaboradores. Isso facilita a atribuição de permissões específicas a equipes como Desenvolvimento, DevOps, Arquitetura e DBAs, entre outras. Ao organizar usuários em grupos, é possível aplicar políticas de acesso de forma consistente e eficiente, garantindo que cada equipe tenha os direitos apropriados para suas funções. Isso simplifica a administração e melhora a segurança, ao assegurar que apenas os membros de cada grupo tenham as permissões necessárias.

---

## Pergunta 36

**Um aplicativo necessita que os dados estejam organizados e distribuídos em tabelas, relacionadas por chaves, para atender a um requisito funcional. Qual banco de dados abaixo NÃO é recomendado para essa finalidade?**

- MySQL
    - Explicação: MySQL é relacional e pode ser utilizado na solução apresentada.

- Aurora
    - Explicação: Aurora é relacional e pode ser utilizado na solução apresentada.

- **✅** DynamoDB
    - Explicação: O DynamoDB não é um banco relacional e não atende esses requisitos.

- MariaDB
    - Explicação: MariaDB é relacional e pode ser utilizado na solução apresentada.

> **Explicação geral**:  
> O Amazon DynamoDB é um serviço de banco de dados NoSQL totalmente gerenciado, oferecendo armazenamento escalável e alta disponibilidade. Ele é projetado para aplicações que exigem latência baixa e alto desempenho, escalonando automaticamente conforme a demanda. O DynamoDB utiliza modelos de dados flexíveis, permitindo a armazenagem de informações estruturadas, e oferece opções de replicação global para disponibilidade global e recuperação de desastres.

---

## Pergunta 37

**Qual das seguintes opções deve ser configurada para que uma função Lambda escreva dados no Amazon DynamoDB?**

- Amazon API Gateway
    - Explicação: O Amazon API Gateway é um serviço totalmente gerenciado que facilita a criação, publicação, manutenção, monitoramento e segurança de APIs em qualquer escala. Ele permite que desenvolvedores criem APIs RESTful e WebSocket para acessar serviços backend como AWS Lambda, EC2 e outros serviços web, fornecendo controle de tráfego, autenticação e monitoramento.

- IAM Users
    - Explicação: Os IAM Users (Usuários IAM) são identidades criadas no AWS Identity and Access Management (IAM) para representar pessoas que precisam interagir com os recursos da AWS. Cada usuário possui credenciais únicas e pode ser atribuído a políticas que definem suas permissões, controlando o que eles podem acessar e fazer dentro da conta AWS.

- Amazon SNS
    - Explicação: O Amazon SNS é um serviço de mensagem que facilita o envio de notificações em tempo real a múltiplos sistemas e serviços usando o modelo pub/sub.

- **✅** IAM Roles
    - Explicação: Para que qualquer aplicação consiga acessar serviços da AWS é necessária a criação e gerenciamento de IAM Roles (Funções do IAM) com as permissões necessárias.

> **Explicação geral**:  
> O IAM roles (Identity and Access Management) são entidades na AWS que concedem permissões temporárias a entidades confiáveis, como serviços ou usuários externos. Diferentemente das contas de usuário, as roles não têm credenciais permanentes, melhorando a segurança. As roles são usadas para delegar acesso a recursos específicos sem compartilhar senhas ou chaves de acesso, permitindo uma gestão mais granular de permissões e reforçando a política do menor privilégio.

---

## Pergunta 38

**Um objeto do S3 é composto por quais componentes? (selecione 3 alternativas)**

- Roles
    - Explicação: Roles são funções do IAM para gerenciar acesso de aplicativos a serviços da AWS.

- **✅** Metadados
    - Explicação: Informações adicionais associadas ao objeto, como data de criação, tipo de conteúdo e outras propriedades definidas pelo usuário ou automaticamente pela AWS.

- **✅** Dados
    - Explicação: O conteúdo real armazenado no objeto, que pode ser qualquer tipo de arquivo ou dado binário.

- Policy
    - Explicação: Uma policy é um documento que define permissões e regras de acesso a recursos na AWS, especificando o que uma identidade pode ou não fazer.

- **✅** Identificador exclusivo (chave)
    - Explicação: Um identificador único dentro de um bucket que é usado para acessar e recuperar o objeto.

> **Explicação geral**:  
> Um objeto no Amazon S3 (Simple Storage Service) é composto por dados, metadados e um identificador exclusivo (chave). Os dados representam o conteúdo real que está sendo armazenado, como arquivos de mídia ou documentos. Os metadados são informações descritivas sobre o objeto, como data de criação e tipo de conteúdo. A chave é um nome exclusivo que identifica o objeto no bucket.
> 
> Os benefícios da composição de um objeto no Amazon S3 incluem a flexibilidade de armazenar qualquer tipo de dado de forma escalável e durável, a capacidade de acessar objetos rapidamente usando URLs únicos, a redundância de dados para alta disponibilidade e a integração com outros serviços da AWS para análise, processamento e backup de dados. Além disso, o S3 oferece opções de controle de acesso, criptografia e gerenciamento de ciclo de vida para otimizar o armazenamento e proteger os dados de acordo com as necessidades da organização.

---

## Pergunta 39

**Qual é o serviço da AWS que permite selecionar uma imagem de uma máquina pré-configurada para lançar uma instância EC2?**

- **✅** Amazon AMI
    - Explicação: Amazon Machine Image (AMI) são templates que contêm a configuração necessária, incluindo o sistema operacional, o servidor de aplicações e outras configurações, para lançar uma instância EC2. As AMIs podem ser usadas para criar instâncias rapidamente com a mesma configuração, garantindo consistência e eficiência no provisionamento de servidores.

- Amazon EBS
    - Explicação: O Amazon EBS (Elastic Block Store) fornece armazenamento em bloco para instâncias EC2, mas não é utilizado para selecionar e lançar instâncias a partir de imagens pré-configuradas como o Amazon Machine Image (AMI).

- Amazon ECR
    - Explicação: O Amazon ECR (Elastic Container Registry) é um serviço de registro de contêineres, usado para armazenar, gerenciar e implantar imagens de contêiner Docker, e não para lançar instâncias EC2 a partir de imagens de máquinas pré-configuradas.

- Amazon EFS
    - Explicação: O Amazon EFS (Elastic File System) oferece armazenamento de arquivos escalável para uso com instâncias EC2, mas não é utilizado para selecionar e lançar instâncias a partir de imagens pré-configuradas como o Amazon Machine Image (AMI).

> **Explicação geral**:  
> Amazon Machine Image (AMI) é um template que contém a configuração necessária para lançar uma instância EC2, incluindo sistema operacional e servidores de aplicação. AMIs permitem criar instâncias rapidamente com a mesma configuração, garantindo consistência e eficiência. Em Auto Scaling, AMIs garantem que todas as instâncias escaladas automaticamente sejam idênticas, atendendo à demanda de forma consistente. AMIs são úteis para backup e recuperação rápida de instâncias, criação de ambientes de desenvolvimento e teste, desdobramento de aplicações em múltiplas regiões e migração de sistemas para a nuvem. Esses usos asseguram a manutenção de uma infraestrutura flexível, eficiente e confiável na AWS.

---

## Pergunta 40

**Qual componente de rede pode ser utilizado para hospedar instâncias EC2 na AWS?**

- AWS Autoscaling
    - Explicação: O Amazon EC2 Auto Scaling ajuda a manter a disponibilidade das aplicações e permite adicionar ou remover instâncias do EC2 automaticamente de acordo com as condições que você definir.

- AWS Trusted Advisor
    - Explicação: O AWS Trusted Advisor faz recomendações que ajudam você a seguir as melhores práticas da AWS. O Trusted Advisor avalia a sua conta através de verificações. Essas verificações identificam formas de otimizar sua infraestrutura da AWS, aumentar a segurança e o desempenho, reduzir os custos gerais e monitorar as cotas do serviço.

- **✅** AWS VPC
    - Explicação: A VPC (Virtual Private Cloud) é usada para criar uma rede isolada onde você pode lançar e gerenciar recursos, como instâncias EC2, com controle total sobre a configuração de rede.

- AWS Elastic Load Balancer
    - Explicação: O Elastic Load Balancing (ELB) distribui automaticamente o tráfego de entrada de aplicações entre diversos destinos, como instâncias do Amazon EC2, contêineres, endereços IP, funções do Lambda e dispositivos virtuais.

> **Explicação geral**:  
> O Amazon Virtual Private Cloud (Amazon VPC) permite controle total sobre a rede virtual, incluindo posicionamento de recursos, conectividade e segurança. Configure a VPC dividindo a rede em sub-redes para organizar e isolar recursos. Em uma aplicação de três camadas: a camada de apresentação usa sub-redes públicas para instâncias EC2 com acesso à Internet; a camada de aplicação utiliza sub-redes privadas para servidores acessíveis apenas pela camada de apresentação; e a camada de banco de dados emprega sub-redes privadas para bancos de dados como o Amazon RDS, acessíveis apenas pela camada de aplicação. A comunicação entre sub-redes é gerida por tabelas de rotas e gateways, e VPCs podem intercomunicar-se através de peering e gateways de trânsito, garantindo segurança e eficiência na infraestrutura na nuvem.

---

## Pergunta 41

**O AWS Application Migration Service (MGN) oferece uma variedade de métodos de migração para ajudar as organizações a migrarem aplicativos e cargas de trabalho para a AWS. Qual ou quais são os principais métodos de migração suportados pelo MGN e como eles se diferenciam?**

- O MGN suporta apenas a migração por replicação contínua, onde as alterações no aplicativo são replicadas em tempo real para a nuvem AWS.
    - Explicação: O MGN suporta múltiplos métodos de migração, permitindo que as empresas escolham a abordagem mais adequada às suas necessidades, as demais opções apresentam só um método.

- O MGN suporta apenas a migração por transmissão de dados, onde os dados são transferidos diretamente para a nuvem AWS sem replicação contínua ou migração de snapshot.
    - Explicação: O MGN suporta múltiplos métodos de migração, permitindo que as empresas escolham a abordagem mais adequada às suas necessidades, as demais opções apresentam só um método.

- O MGN suporta apenas a migração por transmissão de dados envolve a transferência de dados diretamente para a nuvem.
    - Explicação: O MGN suporta múltiplos métodos de migração, permitindo que as empresas escolham a abordagem mais adequada às suas necessidades, as demais opções apresentam só um método.

- **✅** O MGN suporta migração por replicação contínua, migração de snapshot e migração por transmissão de dados. A migração por replicação contínua envolve a replicação em tempo real, a migração de snapshot captura um estado específico do aplicativo, e a migração por transmissão de dados envolve a transferência de dados diretamente para a nuvem.
    - Explicação: O AWS Application Migration Service (MGN) é uma solução da Amazon Web Services que simplifica o processo de migração de aplicativos e cargas de trabalho para a nuvem AWS. Ele automatiza tarefas complexas, como replicação de dados em tempo real e criação de snapshots, proporcionando economia de custos e eficiência operacional.

> **Explicação geral**:  
> O AWS Application Migration Service (MGN) é uma solução da Amazon Web Services que simplifica o processo de migração de aplicativos e cargas de trabalho para a nuvem AWS. Ele automatiza tarefas complexas, como replicação de dados em tempo real e criação de snapshots, proporcionando economia de custos e eficiência operacional. O MGN suporta múltiplos métodos de migração, permitindo que as empresas escolham a abordagem mais adequada às suas necessidades. Além disso, ajuda a identificar e avaliar as dependências de aplicativos, facilitando uma migração mais precisa e minimizando interrupções nos negócios.

---

## Pergunta 42

Qual serviço de armazenamento de dados da Amazon é empregado pelas áreas de Business Intelligence, possibilitando a análise de dados estruturados e semi-estruturados para gerar insights para o negócio?

- Amazon QuickSight
    - Explicação: O Amazon QuickSight é um serviço de Business Intelligence (BI) da AWS que permite criar e compartilhar visualizações interativas de dados, facilitando a obtenção de insights. Ele oferece análises ad hoc, dashboards interativos e relatórios automatizados, integrando-se com diversas fontes de dados, incluindo AWS, bancos de dados on-premises e aplicações SaaS.

- Amazon EMR
    - Explicação: O Amazon EMR (Elastic MapReduce) é um serviço gerenciado que facilita o processamento de grandes volumes de dados usando frameworks como Apache Hadoop e Apache Spark. Ele é ideal para tarefas de análise de big data, como mineração de dados, processamento de logs e transformação de dados em larga escala.

- **✅** Amazon RedShift
    - Explicação: O Amazon Redshift é ideal para executar consultas complexas e análises em grandes volumes de dados. O serviço de armazenamento de dados da Amazon utilizado para Business Intelligence, permitindo a análise de dados estruturados e semi-estruturados para gerar insights.

- Amazon Kinesis
    - Explicação: O Amazon Kinesis é um serviço da AWS projetado para coletar, processar e analisar dados em tempo real em grande escala. Ele permite a ingestão de dados de diversas fontes, como logs de aplicativos, streams de eventos, dados de sensores IoT e interações de sites, processando-os quase instantaneamente.

> **Explicação geral**:  
> O Amazon Redshift é um serviço de data warehouse totalmente gerenciado pela AWS, projetado para analisar grandes volumes de dados estruturados e semi-estruturados. Ele permite a execução de consultas complexas e análises rápidas, integrando-se facilmente com ferramentas de Business Intelligence (BI). Redshift é otimizado para desempenho e pode escalar para petabytes de dados, proporcionando insights valiosos para o negócio. É ideal para empresas que precisam consolidar dados de várias fontes, executar análises ad hoc e gerar relatórios detalhados. Com suporte a SQL e integração com o ecossistema AWS, Redshift facilita a análise de dados e a tomada de decisões informadas.

---

## Pergunta 43

Qual serviço AWS é ideal para armazenar dados que raramente precisam ser acessados, mas ainda requerem durabilidade a longo prazo e custo baixo?

- S3 Standard
    - Explicação: O Simple Storage Service Standard é utilizado para salvar arquivos que são acessados com frequência numa solução, o seu custo é mais alto por isso.

- DynamoDb
    - Explicação: O DynamoDb é um serviço de banco de dados não relacional para persistir os dados de uma aplicação.

- EC2
    - Explicação: O Elastic Computing Cloud é o serviço que oferece diversas configurações de processamento e memória para uma aplicação, não para armazenamento de dados.

- **✅** S3 Glacier
    - Explicação: O Amazon S3 Glacier é a melhor opção para armazenar dados que raramente precisam ser acessados, oferecendo durabilidade a longo prazo e custos baixos. Ele é ideal para backups, arquivamento e armazenamento de dados com pouca necessidade de recuperação rápida.

> **Explicação geral**:  
> O Amazon S3 oferece várias classes de armazenamento para diferentes necessidades:
> 
> - S3 Standard: Para dados acessados frequentemente, com baixa latência e alta taxa de transferência, ideal para sites dinâmicos e aplicativos móveis.
> - S3 Intelligent-Tiering: Move automaticamente dados entre camadas de acesso frequente e infrequente com base nos padrões de acesso, otimizando custos.
> - S3 Standard-IA (Infrequent Access): Para dados acessados com menor frequência, mas que ainda precisam de acesso rápido, como backups e recuperação de desastres.
> - S3 One Zone-IA: Similar ao Standard-IA, mas armazenado em uma única zona de disponibilidade, oferecendo um custo mais baixo.
> - S3 Glacier: Para arquivamento de dados raramente acessados, com tempos de recuperação que variam de minutos a horas, ideal para backups de longo prazo.
> - S3 Glacier Deep Archive: A opção mais econômica, para dados que podem tolerar tempos de recuperação de até 12 horas, ideal para conformidade e arquivamento de dados de longo prazo.
> 
> Essas camadas permitem gerenciar dados de forma eficiente, equilibrando custo e acessibilidade conforme necessário.

---

## Pergunta 44

Uma empresa lançou um piloto de uma aplicação e ainda não tem uma estimativa precisa do número de clientes que a utilizarão. A aplicação requer alta disponibilidade e o piloto está programado para durar três meses.

Em termos de pagamento, qual seria o plano mais apropriado para este cenário?

- Dedicated Hosts
    - Explicação: O plano Dedicated Hosts não é indicado porque envolve custos significativamente mais altos e é ideal para cargas de trabalho que necessitam de isolamento físico por motivos de conformidade ou licenciamento específico.

- **✅** On-Demand
    - Explicação: Dado que o período de piloto é de apenas dois meses e a quantidade de usuários e instâncias de máquinas necessárias ainda é incerta, o plano On-Demand é o mais apropriado. Este modelo permite pagar apenas pelos recursos efetivamente utilizados, oferecendo flexibilidade e escalabilidade sem compromissos de longo prazo.

- Reserved
    - Explicação: O plano Reserved não é indicado porque exige um compromisso de longo prazo, tipicamente de 1 a 3 anos, o que não é adequado para um piloto de apenas dois meses.

- Spot
    - Explicação: O plano Spot não é indicado porque oferece capacidade de computação a preços reduzidos, mas sem garantias de disponibilidade contínua. As instâncias Spot podem ser interrompidas pela AWS com pouco aviso quando a capacidade é necessária para outras tarefas, o que pode comprometer a alta disponibilidade e estabilidade necessárias para o piloto da aplicação.

> **Explicação geral**:  
> O plano On-Demand é ideal para projetos de curta duração e demandas imprevisíveis, como testes e desenvolvimentos. Ele permite pagar apenas pelos recursos utilizados, sem compromissos de longo prazo, oferecendo flexibilidade e escalabilidade. Empresas podem ajustar a quantidade de instâncias conforme necessário, evitando custos associados ao superprovisionamento. Este modelo é econômico e perfeito para startups ou projetos experimentais, garantindo que os recursos estejam disponíveis sem comprometer grandes investimentos financeiros.

---

## Pergunta 45

Qual tecnologia o time de desenvolvimento da sua empresa precisa dominar para criar aplicações que utilizam o banco de dados DynamoDB?

- **✅** APIs do serviço e o JSON com atributos e comandos
    - Explicação: Para trabalhar com o Amazon DynamoDB, é essencial entender como utilizar suas APIs e como inserir comandos via JSON.

- Amazon Athena
    - Explicação: O Amazon Athena não pode ser usado diretamente para consultar dados armazenados no DynamoDB. O Athena é projetado para consultar dados armazenados no Amazon S3 usando SQL.

- Comandos SQL
    - Explicação: O Amazon DynamoDB é um banco de dados NoSQL que utiliza uma API baseada em JSON para operações, ao invés de SQL. Isso é devido ao seu modelo de dados chave-valor e a necessidade de escalabilidade e flexibilidade que não são compatíveis com a abordagem relacional do SQL.

- Gremlin
    - Explicação: O Gremlin não é diretamente um serviço da AWS, mas uma linguagem de consulta para grafos que pode ser usada com bancos de dados de grafos como o Amazon Neptune. O Amazon Neptune é um banco de dados de grafos totalmente gerenciado pela AWS que suporta tanto Gremlin (para consultas de grafos orientados a propriedades) quanto SPARQL (para grafos RDF).

> **Explicação geral**:  
> O DynamoDB permite a execução de operações como leitura, escrita, atualização e exclusão de dados através de comandos estruturados em JSON. Conhecer essas APIs e a estrutura dos comandos JSON é fundamental para manipular dados, configurar tabelas, e gerenciar índices no DynamoDB. Essas operações são realizadas utilizando as APIs fornecidas pelo DynamoDB, permitindo interações eficientes e personalizadas com o banco de dados.

---

## Pergunta 46

Qual é o plano de suporte que oferece tempo de resposta menor que 15 minutos para caso de sistema essencial aos negócios inativo?

- Todos
    - Explicação: Cada plano de suporte possui características distintas e os tempos de resposta variam significativamente entre eles.

- Developer
    - Explicação: Sem tempo de resposta garantido para sistemas de produção inativos, também não recomendado para cargas de produção.

- Business
    - Explicação: Tempo de resposta inferior a 1 hora para sistemas de produção inativos.

- **✅** Enterprise
    - Explicação: Este é o único plano com o tempo de resposta inferior a 15 minutos para sistemas críticos e essenciais aos negócios inativos.

> **Explicação geral**:  
> A AWS oferece cinco planos de suporte: Basic, Developer, Business, Enterprise On-Ramp (novo) e Enterprise.
> 
> - Basic: Sem tempo de resposta garantido para sistemas de produção inativos, não recomendado para cargas de produção.
> - Developer: Sem tempo de resposta garantido para sistemas de produção inativos, também não recomendado para cargas de produção.
> - Business: Tempo de resposta inferior a 1 hora para sistemas de produção inativos.
> - Enterprise On-Ramp: Tempo de resposta inferior a 30 minutos para sistemas de produção inativos.
> - Enterprise: Tempo de resposta inferior a 15 minutos para sistemas críticos e essenciais aos negócios inativos.
> 
> Recomendo estudar e comparar as diferenças dos planos diretamente no site da AWS para escolher o mais adequado às suas necessidades.

---

## Pergunta 47

Ao implementar cargas de trabalhos (workloads) na AWS, uma empresa deve realizar estimativas e monitoramento das cobranças relacionadas à transferência de dados, a fim de tomar decisões arquiteturais que minimizem os custos.

Considerando esse contexto, qual opção representa um cenário em que o tráfego é isento de custos?

- Transferência de dados da AWS para a Internet
    - Explicação: A transferência de dados da AWS para a Internet não é isenta de custos. Esse tráfego gera cobranças, que variam conforme a quantidade de dados transferidos e a região de origem. Para minimizar os custos, é importante considerar a otimização do tráfego de saída e o uso de serviços como o Amazon CloudFront, que pode reduzir os custos de transferência de dados ao entregar conteúdo a partir de localizações mais próximas dos usuários finais.

- Todo tráfego de dados é cobrado
    - Explicação: Na AWS, nem todo tráfego de dados é cobrado.

- **✅** Transferência de dados da Internet para AWS
    - Explicação: A transferência de dados da Internet para a AWS é isenta de custos. Isso permite que empresas carreguem dados na nuvem sem incorrer em despesas adicionais com transferência de dados.

- Transferência de dados de saída entre regiões
    - Explicação: A transferência de dados entre regiões (inter-region) na AWS não é isenta de custos. Esse tipo de tráfego gera cobranças, que podem variar conforme a quantidade de dados transferidos e as regiões envolvidas.

> **Explicação geral**:  
> Na AWS, nem todo tráfego de dados é cobrado.
> 
> Aqui estão alguns cenários específicos:
> 
> **Isento de Custos**:
> 
> - Transferência de dados da Internet para a AWS: O tráfego de entrada da Internet para a AWS é geralmente gratuito.
> - Transferência de dados dentro da mesma Zona de Disponibilidade (AZ): O tráfego entre instâncias dentro da mesma AZ é gratuito.
> 
> **Cobrados**:
> 
> - Transferência de dados entre regiões (inter-region): O tráfego de dados entre diferentes regiões da AWS é cobrado.
> - Transferência de dados da AWS para a Internet: Esse tráfego é cobrado, com taxas que variam conforme a quantidade de dados transferidos e a região de origem.
> - Transferência de dados entre Zonas de Disponibilidade (intra-region): O tráfego entre diferentes Zonas de Disponibilidade dentro da mesma região também pode gerar custos.
> 
> Para minimizar custos, as empresas devem considerar esses fatores ao projetar a arquitetura de suas aplicações na AWS.

---


## Pergunta 48

Uma organização deseja rapidamente implementar uma interface de chatbot com inteligência artificial e linguagem natural, integrada ao Facebook Messenger.

Qual serviço da AWS facilita essa implementação?

- **✅** Amazon Lex
    - Explicação: O Amazon Lex facilita a criação rápida de chatbots com IA para integração com o Facebook Messenger.

- Amazon Polly
    - Explicação: O Amazon Polly é um serviço de nuvem que converte texto em fala realista. Você pode usar o Amazon Polly para desenvolver aplicações que aumentam o envolvimento e a acessibilidade. O Amazon Polly oferece suporte a vários idiomas e inclui diversas de vozes realistas, para que você possa criar aplicações compatíveis com fala que funcionam em vários locais e use a voz ideal para os seus clientes.

- Amazon Comprehend
    - Explicação: O Amazon Comprehend é um serviço de Natural Language Processing (NLP – Processamento de linguagem natural) que usa Machine Learning para obter significados e insights em documentos em texto. Ele identifica o idioma do texto, extrai as frases principais, lugares, pessoas, marcas ou eventos, entende o sentimento em relação a produtos ou serviços e identifica os tópicos principais a partir de uma biblioteca de documentos. A origem desse texto pode ser páginas da Web, feeds de mídia social, e-mails ou artigos.

- Amazon Kendra
    - Explicação: O Amazon Kendra é um serviço de pesquisa altamente preciso e inteligente que habilita seus usuários a pesquisarem dados não estruturados e estruturados usando processamento de linguagem natural e algoritmos de pesquisa avançados. Ele retorna respostas específicas para perguntas, proporcionando aos usuários uma experiência próxima à interação com um especialista humano.

> **Explicação geral**:  
> O Amazon Lex é um serviço para criar interfaces de conversação com voz e texto, utilizando a mesma tecnologia de aprendizado profundo que alimenta o Amazon Alexa. Ele permite a construção de chatbots sofisticados que podem ser integrados facilmente ao Facebook Messenger, proporcionando interações naturais e intuitivas com os usuários. Além disso, o Amazon Lex simplifica o desenvolvimento ao fornecer ferramentas de reconhecimento de fala automática (ASR) e compreensão de linguagem natural (NLU), agilizando a criação e implementação do chatbot.

---

## Pergunta 49

Uma equipe de desenvolvimento observou que 30% das consultas realizadas por uma aplicação no banco de dados sempre retornam o mesmo resultado.

Qual serviço da AWS pode ser implantado para armazenar em cache esses resultados e reduzir os acessos ao banco de dados?

- AWS RAM
    - Explicação: O AWS Resource Access Manager (RAM) permite compartilhar recursos da AWS entre contas diferentes, facilitando a colaboração e eliminando a duplicação de infraestrutura. Ele suporta a partilha de recursos como sub-redes VPC e roles do IAM. Isso ajuda a reduzir custos e simplificar a administração de recursos compartilhados.

- **✅** Amazon ElastiCache
    - Explicação: O Amazon ElastiCache é um serviço de cache gerenciado da AWS que facilita a implantação e a operação de caches na nuvem. Ele oferece suporte a cache em memória usando mecanismos populares, como o Redis e o Memcached, para acelerar o desempenho de aplicativos e reduzir a carga em bancos de dados.

- Amazon EC2
    - Explicação: O Amazon Elastic Compute Cloud (Amazon EC2) é um serviço Web que disponibiliza capacidade computacional segura e redimensionável na nuvem.

- Amazon EBS
    - Explicação: O Amazon Elastic Block Store (EBS) é um serviço de armazenamento em bloco fácil de usar e de alta performance, projetado para uso com o Amazon Elastic Compute Cloud (EC2) para taxas de transferência e cargas de trabalho intensivas de transações em qualquer escala.

> **Explicação geral**:  
> O Amazon ElastiCache é extremamente útil para armazenar em cache dados repetidos retornados de bancos de dados, melhorando significativamente o desempenho das aplicações. É um serviço de cache gerenciado da AWS que facilita a implantação e operação de caches na nuvem. Ele suporta mecanismos populares de cache em memória, como Redis e Memcached, acelerando o desempenho de aplicativos e aliviando a carga em bancos de dados. O ElastiCache automatiza tarefas como provisionamento, escalabilidade, monitoramento e manutenção de clusters de cache, permitindo que os desenvolvedores se concentrem no desenvolvimento do aplicativo. Com isso, melhora-se a latência, escalabilidade e resiliência dos aplicativos, otimizando a experiência do usuário. Além disso, o ElastiCache integra-se facilmente com outros serviços da AWS, proporcionando uma solução completa para o gerenciamento de caches na nuvem.

---

## Pergunta 50

Qual é a classe de armazenamento do S3 que pode diminuir os custos, à medida que move os objetos automaticamente entre camadas, de acordo com a frequência de uso?

- S3 Standard Infrequent Access
    - Explicação: O S3 Standard-Infrequent Access (S3 Standard-IA) é uma classe de armazenamento do Amazon S3 projetada para dados acessados com menos frequência, mas que ainda precisam de acesso rápido quando necessário. Ele oferece um custo mais baixo por gigabyte armazenado em comparação ao S3 Standard, sendo ideal para dados de backup, recuperação de desastres e outros dados que precisam ser acessados ocasionalmente.

- **✅** S3 Intelligent-Tiering
    - Explicação: O S3 Intelligent-Tiering é uma classe de armazenamento do Amazon S3 que otimiza automaticamente os custos ao mover dados entre camadas de acesso frequente e infrequente com base na frequência de acesso dos objetos, sem impacto na performance.

- S3 Glacier
    - Explicação: O S3 Glacier é uma classe de armazenamento do Amazon S3 projetada para arquivamento de dados a longo prazo com baixíssimo custo. É ideal para dados que são raramente acessados e podem tolerar tempos de recuperação que variam de minutos a horas.

- S3 Standard
    - Explicação: O S3 Standard é uma classe de armazenamento do Amazon S3 projetada para dados acessados frequentemente, oferecendo baixa latência e alta taxa de transferência. É ideal para uma ampla gama de casos de uso, incluindo armazenamento de sites, aplicativos móveis, e processamento de big data.

> **Explicação geral**:  
> O Intelligent-Tiering é uma classe de armazenamento do Amazon S3 que otimiza automaticamente os custos ao mover os objetos entre as classes de armazenamento "Frequent Access" e "Infrequent Access" com base nos padrões de acesso. Ele monitora a frequência de acesso dos objetos e, se um objeto não for acessado com frequência, ele é movido para a classe "Infrequent Access" para reduzir custos. Se o objeto voltar a ser acessado com mais frequência, ele é movido de volta para a classe "Frequent Access". Isso permite um armazenamento eficiente, mantendo o desempenho e reduzindo os custos associados.

---

## Pergunta 51

Quais são as principais funcionalidades do Amazon SageMaker?

(selecione duas alternativas)

- Preparar, documentar e publicar APIs com raml sawgger
    - Explicação: Essa é uma das funções do Api Gateway.

- Preparar, Construir e implantar APIs Rest
    - Explicação: Essa é uma das funções do Api Gateway.

- Preparar e Migrar bancos de dados na AWS
    - Explicação: Essa é a função do AWS Database Migration Service (DMS).

- **✅** Preparar, Construir, Treinar e Implantar modelos de machine learning na AWS
    - Explicação: Amazon SageMaker é um serviço gerenciado de aprendizado de máquina da AWS que permite criar, treinar e implantar modelos de machine learning de maneira eficiente.

- **✅** Oferecer uma IDE para uso de Machine Learning
    - Explicação: O SageMaker possui uma IDE (Integrated Development Environment) que facilita a escrita de código e a colaboração em projetos de aprendizado de máquina.

> **Explicação geral**:  
> O Amazon SageMaker é um serviço gerenciado de machine learning da AWS que facilita a criação, treinamento e implantação de modelos de aprendizado de máquina de forma eficiente. Ele oferece um ambiente abrangente para todo o fluxo de trabalho de ML, desde a preparação dos dados até a implementação do modelo em produção.
> 
> O SageMaker inclui uma IDE (Integrated Development Environment) que simplifica a escrita de código e a colaboração em projetos de machine learning. Ele vem com notebooks Jupyter pré-configurados com bibliotecas populares, ferramentas de visualização e capacidades integradas para implantar modelos diretamente em produção, facilitando o ciclo de vida completo do aprendizado de máquina.


---

## Pergunta 52

Qual é o documento que fornece uma declaração formal de uma ou mais permissões no IAM?

- **✅** Políticas (Policies)
    - Explicação: As políticas são escritas em JSON e definem explicitamente o que um usuário, grupo ou role pode ou não pode fazer em relação aos recursos da AWS. As policies são anexadas a roles, usuários ou grupos para controlar o acesso.

- Funções (Roles)
    - Explicação: Roles (funções) são identidades temporárias no AWS IAM que fornecem permissões específicas quando assumidas por usuários, serviços ou aplicações, sem usar credenciais permanentes. Policies (políticas) são documentos JSON que definem essas permissões, especificando ações permitidas ou negadas em recursos da AWS.

- Grupos (Groups)
    - Explicação: Grupos no AWS IAM são coleções de usuários que permitem a aplicação coletiva de políticas de permissão. Anexando políticas a um grupo, todos os membros herdam essas permissões, simplificando o gerenciamento de acesso. Isso facilita a administração e garante consistência nas permissões dos usuários.

- Usuários (Users)
    - Explicação: Usuários no AWS IAM são entidades individuais que representam pessoas ou serviços que precisam interagir com os recursos da AWS. Cada usuário possui credenciais únicas e pode ter políticas de permissão anexadas diretamente para definir o que eles podem acessar e fazer. Isso permite um controle preciso e seguro sobre o acesso aos recursos na AWS.

> **Explicação geral**:  
> Policies ou Políticas de Permissão na AWS são objetos JSON que definem as permissões para identidades do IAM (usuários, grupos ou roles) e recursos da AWS. Ao criar políticas, você as anexa a identidades ou recursos para gerenciar o acesso. Quando uma entidade de segurança do IAM faz uma solicitação, a AWS avalia as políticas associadas para determinar se a ação solicitada é permitida ou negada. Essas políticas detalham ações permitidas ou negadas em serviços específicos, garantindo controle granular sobre o acesso aos recursos. A utilização de políticas permite a implementação de práticas de segurança e conformidade robustas na infraestrutura da AWS.


---

## Pergunta 53

Qual plano de suporte oferece acesso aos engenheiros do Cloud Support por telefone, e-mail e chat 24 horas por dia, 7 dias por semana?

- **✅** Business
    - Explicação: Esse tipo de suporte só é oferecido para os planos recomendados para cargas de produção, o Business, Enterprise on-Ramp e Enterprise.

- Standard
    - Explicação: Standard não é um nome válido para os planos de suporte ofertados pela AWS.

- Basic
    - Explicação: O plano Basic da AWS oferece suporte limitado em comparação com os planos pagos. Ele fornece acesso ao AWS Trusted Advisor e ao AWS Personal Health Dashboard, mas não inclui acesso aos engenheiros do Cloud Support por telefone, e-mail e chat 24 horas por dia, 7 dias por semana.

- Developer
    - Explicação: O plano Developer da AWS oferece acesso aos engenheiros do Cloud Support por e-mail durante o horário comercial, mas não por telefone ou chat 24 horas por dia, 7 dias por semana.

> **Explicação geral**:  
> A AWS oferece cinco planos de suporte: Basic, Developer, Business, Enterprise On-Ramp e Enterprise.
> 
> - Basic: Gratuito, fornece acesso ao AWS Trusted Advisor e AWS Personal Health Dashboard, mas não inclui suporte técnico 24/7 por engenheiros.
> - Developer: Inclui suporte técnico por e-mail durante o horário comercial com tempo de resposta de até 24 horas para problemas gerais. Adequado para testar e explorar a AWS.
> - Business: Suporte 24/7 por telefone, e-mail e chat, com tempos de resposta mais rápidos (1 hora para questões urgentes). Inclui suporte técnico e consultivo, acesso ao AWS Support API e instruções operacionais.
> - Enterprise On-Ramp: Projetado para empresas com workloads críticas. Oferece suporte 24/7 por telefone, e-mail e chat, com tempos de resposta prioritários. Inclui gerenciamento de contas técnicas e revisões operacionais.
> - Enterprise: Suporte técnico 24/7 com tempos de resposta mais rápidos (15 minutos para problemas críticos). Oferece um Technical Account Manager (TAM) dedicado, revisões arquitetônicas, gestão proativa e acesso a programas de suporte empresarial personalizados.
> 
> Esses planos variam em termos de custo, abrangência de suporte e tempos de resposta, permitindo que empresas escolham o nível adequado de suporte para suas necessidades.

---

## Pergunta 54

Qual ação é de responsabilidade dos clientes quando é preciso garantir que dados em volumes EBS estejam seguros e com seus backups realizados?

- Ativar a Multi-AZ para volumes EBS.
    - Explicação: A configuração Multi-AZ (Multi-Availability Zone) é usada principalmente para serviços de banco de dados, como RDS, para replicar dados automaticamente em várias zonas de disponibilidade, aumentando a disponibilidade e a tolerância a falhas. No caso de volumes EBS, a criação e replicação de snapshots é a abordagem correta para backups e segurança dos dados.

- Configurar o IAM para acesso a snapshots.
    - Explicação: Embora a configuração do IAM (Identity and Access Management) seja crucial para gerenciar permissões e acesso a snapshots, por si só, isso não garante que os dados sejam realmente protegidos ou que os backups sejam realizados. É uma medida de segurança complementar, não uma ação direta de backup.

- Utilizar instâncias reservadas para armazenamento de snapshots.
    - Explicação: Instâncias reservadas são usadas para executar instâncias EC2 com um custo reduzido em compromissos de longo prazo. Elas não estão relacionadas ao armazenamento de snapshots, que é um serviço específico do Amazon EBS.

- **✅** Criar snapshots dos volumes EBS e replicá-los em outras regiões
    - Explicação: Para garantir a segurança e a durabilidade dos dados, os clientes devem criar snapshots dos volumes EBS e, frequentemente, replicá-los para outras regiões. Snapshots são backups incrementais que capturam o estado dos dados em um volume EBS e podem ser usados para restaurar volumes em caso de falha ou perda de dados.

> **Explicação geral**:  
> Criar snapshots dos volumes EBS e replicá-los em outras regiões é uma prática recomendada para garantir a segurança e a durabilidade dos dados. Snapshots são backups incrementais que capturam o estado atual dos dados em um volume EBS, permitindo a restauração em caso de falha ou perda de dados. Replicar esses snapshots em diferentes regiões aumenta a resiliência contra desastres locais, como falhas de zona de disponibilidade ou desastres naturais. Este processo de replicação pode ser automatizado utilizando ferramentas e scripts da AWS, assegurando que os backups sejam realizados regularmente e de forma eficiente. Essa estratégia é essencial para uma recuperação rápida e confiável em situações de emergência, protegendo os dados críticos da sua infraestrutura na nuvem.


---

## Pergunta 55

Qual é o serviço que, seguindo as melhores práticas, pode ser usado para identificar vulnerabilidades e desvios de segurança em aplicativos antes de serem implantados ou durante sua execução em ambiente de produção?

- AWS Trusted Advisor
    - Explicação: O AWS Trusted Advisor te auxilia checando o ambiente e te indicando as melhores práticas de implementação.

- AWS GuardDuty
    - Explicação: O Amazon GuardDuty é um serviço de detecção de ameaças que monitora continuamente atividades mal-intencionadas e comportamentos não autorizados para proteger suas contas, cargas de trabalho e dados da AWS armazenados no Amazon S3.

- **✅** AWS Inspector
    - Explicação: O AWS Inspector é um serviço que realiza análise automática de vulnerabilidades em aplicativos, ajudando a identificar e corrigir problemas de segurança antes e durante a execução em produção.

- AWS WAF
    - Explicação: O AWS WAF é um firewall de aplicações Web que ajuda a proteger suas aplicações Web ou APIs contra bots e exploits comuns na Web que podem afetar a disponibilidade, comprometer a segurança ou consumir recursos em excesso.

> **Explicação geral**:  
> O AWS Inspector é um serviço de avaliação automatizada de segurança da AWS que analisa recursos de computação em busca de vulnerabilidades e configurações inadequadas. Ele realiza varreduras regulares para identificar ameaças de segurança, avalia a exposição a riscos e fornece recomendações para remediação. O Inspector suporta ambientes Windows e Linux, ajudando a aprimorar a postura de segurança, minimizar riscos e fortalecer a conformidade com padrões regulatórios. Isso permite que os usuários mantenham a segurança de suas implantações na nuvem e protejam os dados e aplicativos contra potenciais ameaças.


---

## Pergunta 56

Uma empresa criou várias funções Lambda para consultar informações e integrá-las em um processo de avaliação de crédito, adotando uma abordagem orientada a eventos.

Qual serviço, com mínima necessidade de codificação, pode ser utilizado para expressar lógicas de negócios complexas na forma de fluxos de trabalho para compor essa solução?

- **✅** AWS Step Functions
    - Explicação: O AWS Step Functions é o serviço recomendado, pois permite criar fluxos de trabalho para coordenar várias funções Lambda, expressando lógicas de negócios complexas com uma quantidade mínima de codificação.

- AWS SQS
    - Explicação: O AWS SQS - Simple Queue Service é um serviço de mensageria recomendado pra desacoplar sistemas e pode ser utilizado na arquitetura com Step Functions também.

- AWS BPM
    - Explicação: Este serviço não existe na AWS.

- AWS SNS
    - Explicação: O AWS SNS - Simple Message Service é um serviço de troca de mensagens recomendado para arquiteturas Pub/Sub e utilização de tópicos e também pode ser utilizado na arquitetura junto com o Step Functions.

> **Explicação geral**:  
> AWS Step Functions é um serviço de orquestração de fluxo de trabalho que facilita a criação e a coordenação de aplicativos distribuídos e baseados em serviços. Ele permite criar fluxos de trabalho visualmente, definindo passos individuais como funções Lambda, tarefas de ECS, atividades de data pipeline, entre outros. Esses passos são organizados em um gráfico de estado, onde você pode controlar a sequência, os desvios e as decisões. O Step Functions lida automaticamente com o estado e os retries, garantindo a resiliência dos fluxos de trabalho. Isso simplifica a criação de processos complexos, otimiza a organização e oferece uma abordagem mais gerenciável para orquestração de serviços.

---

## Pergunta 57

Qual das seguintes opções NÃO está associada ao Amazon Cognito?

- integra com a autenticação de mídias sociais como Apple, Facebook, Google e Amazon
    - Explicação: O Amazon Cognito permite que seus usuários façam login diretamente com um nome de usuário e uma senha ou por meio de terceiros, como o Facebook, a Amazon, o Google ou a Apple.

- **✅** permite autenticação de APIs pela linha de comando
    - Explicação: O Amazon Cognito não é ideal para autenticação de APIs pela linha de comando porque ele é projetado principalmente para autenticação de usuários em aplicações web e móveis, utilizando fluxos de autenticação baseados em navegador. Para autenticação de APIs pela linha de comando, AWS recomenda o uso de AWS IAM roles e políticas de segurança.

- adiciona autenticação em aplicativo web e móveis
    - Explicação: O Amazon Cognito fornece autenticação, autorização e gerenciamento de usuários para suas aplicações Web e móveis.

- integra com SAML 2.0 e OpenID
    - Explicação: O Amazon Cognito integra-se com SAML 2.0 e OpenID Connect, permitindo autenticação federada e login único (SSO). Essas integrações facilitam a gestão de identidades e acesso em aplicações web e móveis.

> **Explicação geral**:  
> O Amazon Cognito oferece autenticação, autorização e gerenciamento de usuários para aplicações web e móveis. Ele permite que os usuários façam login diretamente com um nome de usuário e senha ou utilizem provedores de identidade de terceiros, como Facebook, Google, Amazon e Apple. Além disso, o Cognito suporta login social e integração com provedores de identidade SAML e OpenID Connect (OIDC) através de seus grupos de usuários. Isso torna o Cognito ideal para aplicações que necessitam de uma solução robusta de gerenciamento de identidades, facilitando a implementação de login social, autenticação federada e SSO (Single Sign-On). É especialmente útil em cenários onde a segurança e a experiência do usuário são prioridades, como em plataformas de e-commerce, serviços financeiros e aplicações empresariais.


---

## Pergunta 58

Qual dos serviços abaixo é umas das formas de criar e gerenciar chaves de criptografia para muitos serviços dentro da AWS?

- AWS KSM
    - Explicação: Este serviço não existe.

- **✅** AWS KMS
    - Explicação: O AWS Key Management Service (KMS) é um serviço de gerenciamento de chaves que permite criar e controlar o acesso a chaves de criptografia utilizadas para proteger dados na AWS.

- AWS Config
    - Explicação: O AWS Config é um serviço que permite acessar, auditar e avaliar as configurações dos recursos da AWS. O Config monitora e grava continuamente registros das configurações de recursos da AWS e lhe permite automatizar a avaliação das configurações registradas com base nas configurações desejadas.

- AWS ACM
    - Explicação: O AWS Certificate Manager (ACM) é um serviço da AWS que facilita a criação, o gerenciamento e a implantação de certificados SSL/TLS para uso com serviços da AWS e seus recursos internos conectados. O ACM automatiza a renovação de certificados, ajudando a proteger as comunicações de rede com criptografia robusta e sem a necessidade de gerenciar manualmente os certificados.

> **Explicação geral**:  
> O AWS Key Management Service (KMS) é um serviço de gerenciamento de chaves que permite criar e controlar o acesso a chaves de criptografia utilizadas para proteger dados na AWS. Ele oferece um ambiente seguro para criar, importar e gerenciar chaves de criptografia, permitindo criptografar e descriptografar dados de forma transparente em serviços da AWS. O KMS centraliza o gerenciamento de chaves, oferece integração com vários serviços da AWS e permite a auditoria de atividades relacionadas a chaves. Isso ajuda a atender a requisitos de conformidade e a proteger dados sensíveis em ambientes de nuvem.


---

## Pergunta 59

Uma aplicação crítica utiliza de 5 a 10 instâncias EC2 para suportar a grande volumetria de requisição e processamento. Pelos seus estudos, essa infraestrutura atenderá a necessidade pelos próximos 3 anos sem grandes alterações.

Qual seria a melhor estratégia para garantir a escalabilidade e otimizar os custos destas instâncias?

- Utilizar 10 instâncias OnDemand
    - Explicação: Como parte do processamento é previsível, você deixaria de economizar ao não reservar parte delas com antecedência para obter desconto.

- Utilizar 10 instâncias Reserved
    - Explicação: Como parte do processamento é imprevisível, você contraria 5 máquinas antecipadamente sem ter certeza que as utilizariam.

- Utilizar 5 instâncias Reserved e 5 instâncias Spot
    - Explicação: Apesar de sem mais barata, Spot não é indicada para aplicações críticas, uma vez que pode ser interrompida.

- **✅** Utilizar 5 instâncias Reserved e 5 instâncias OnDemand
    - Explicação: Como você já tem certeza que vai utilizar no mínimo 5 recursos é melhor ter desconto no plano reserved (72% em relação ao onDemand) e manter as demais no plano onDemand para usar de acordo com a necessidade pagando um pouco mais ou não pagando nada se não precisar escalar e provisionar essas instâncias.

> **Explicação geral**:  
> Para economizar, uma estratégia eficaz é combinar instâncias reservadas e sob demanda. Instâncias reservadas oferecem descontos significativos em troca de um compromisso de uso de um ou três anos, sendo ideais para cargas de trabalho estáveis e previsíveis. Instâncias sob demanda podem ser usadas para lidar com picos de carga e demandas variáveis, garantindo flexibilidade. Além disso, os Saving Plans proporcionam uma alternativa flexível às instâncias reservadas, oferecendo até 72% de desconto em troca de um compromisso de uso de um ou três anos, aplicável a qualquer uso de computação na AWS, incluindo EC2, Fargate e Lambda. Essa combinação maximiza a economia e a eficiência no gerenciamento de recursos.

---

## Pergunta 60

Qual plano de suporte oferece um gerente técnico de conta para monitorar o ambiente proativamente e sugerir melhorias para otimização dos serviços?

- Business
    - Explicação: Não oferece o gerenciamento técnico e contas.

- Developer
    - Explicação: Não oferece o gerenciamento técnico e contas.

- Basic
    - Explicação: Não oferece o gerenciamento técnico e contas.

- **✅** Enterprise
    - Explicação: Apenas o plano de suporte enterprise oferece o gerente de contas técnico. O plano enterprise on ramp, que foi lançado recentemente, oferece um grupo de gerentes de contas técnicos para fornecer orientação proativa e coordenar o acesso a programas e especialistas da AWS para o gerenciamento de contas técnico.

> **Explicação geral**:  
> Existem várias configurações de serviços de acordo com cada plano de suporte.
> 
> Os planos vigentes são Basic, Developer, Business, Enterprise on ramp e Enterprise.
> 
> As características que variam em cada plano são as seguintes:
> 
> - Verificação de práticas recomendas do AWS Trusted Advisor
> - Suporte técnico aprimorado
> - Tempo de resposta
> - Orientações de arquitetura
> - Gerenciamento programático de casos
> - Suporte a software de terceiros
> - Programas proativos e autoatendimento
> - Gerenciamento de contas técnico
> - Treinamento
> - Assistência à conta
> - Preço


---

## Pergunta 61

Uma desenvolvedora criou um workflow orientado a eventos e deseja que uma função sem servidor registre uma log em um banco de dados ao concluir o processo.

Qual serviço é mais apropriado para atender a essa finalidade?

- Amazon SES
    - Explicação: Serviço de e-mail que permite enviar e-mails em massa e gerenciar campanhas de e-mail marketing.

- Amazon SNS
    - Explicação: Serviço de mensagens que envia notificações para diversos endpoints, como e-mails e SMS.

- **✅** AWS Lambda
    - Explicação: O AWS Lambda é o serviço mais apropriado para essa finalidade. Ele permite executar código em resposta a eventos sem a necessidade de gerenciar servidores. A função Lambda pode ser configurada para registrar logs em um banco de dados após a conclusão do processo, integrando-se facilmente com outros serviços da AWS.

- Amazon SQS
    - Explicação: Serviço de filas que armazena e gerencia mensagens entre componentes de uma aplicação distribuída.

> **Explicação geral**:  
> O AWS Lambda é um serviço de computação serverless que executa código em resposta a eventos sem precisar configurar ou manter servidores. Ele suporta diversas linguagens de programação e pode ser ativado por eventos como uploads de arquivos, chamadas de API ou alterações em bancos de dados. Com escalabilidade automática, o Lambda é ideal para criar microserviços, processar dados em tempo real e automatizar processos.

---

## Pergunta 62

Usuários que utilizam aplicações em nuvem sem se preocuparem com sua construção e implementação estão usando qual tipo de nuvem?

- **✅** SaaS
    - Explicação: Software as a Service (SaaS) é um modelo de entrega de software em que aplicativos são hospedados em nuvem e disponibilizados aos usuários pela internet, sem a necessidade de instalação local.

- PaaS
    - Explicação: Platform as a Service (PaaS) é um modelo de computação em nuvem que fornece uma plataforma completa, incluindo infraestrutura, desenvolvimento, e ferramentas de gerenciamento, permitindo que os desenvolvedores criem, implantem e gerenciem aplicações sem se preocupar com a gestão da infraestrutura subjacente.

- BaaS
    - Explicação: Backend as a Service (BaaS) é um modelo de computação em nuvem que fornece serviços de backend, como gerenciamento de bases de dados, autenticação de usuários, notificações push e armazenamento em nuvem, permitindo que desenvolvedores se concentrem no desenvolvimento do frontend sem se preocupar com a infraestrutura do backend.

- IaaS
    - Explicação: Infrastructure as a Service (IaaS) é um modelo de computação em nuvem que fornece recursos de computação virtualizados, como servidores, armazenamento e redes, através da internet, permitindo que os usuários implantem e gerenciem suas próprias aplicações e sistemas operacionais.

> **Explicação geral**:  
> Software as a Service (SaaS) é um modelo de entrega de software em que os aplicativos são hospedados na nuvem e acessados pela internet, eliminando a necessidade de instalação local. A AWS oferece diversos serviços SaaS, incluindo Amazon Chime para comunicações, Amazon WorkDocs para colaboração de documentos, Amazon Connect para centrais de atendimento, Amazon QuickSight para análise de dados e Amazon WorkMail para e-mail e calendário. Esses serviços permitem que empresas e usuários utilizem aplicativos sem a complexidade de gerenciar a infraestrutura subjacente, facilitando o acesso, a escalabilidade e a atualização contínua. Além dos serviços AWS, alguns dos serviços SaaS mais comuns e amplamente utilizados no mundo incluem Google Workspace para produtividade e colaboração, Microsoft Office 365 para aplicações de escritório, Salesforce para gerenciamento de relacionamento com clientes (CRM) e Slack para comunicação e colaboração em equipe.


---

## Pergunta 63

Uma organização pretende aprimorar a segurança de seus recursos na AWS, buscando uma solução que facilite o provisionamento, gerenciamento e implantação de certificados Secure Sockets Layer (SSL)/Transport Layer Security (TLS) a serem empregados nos serviços da AWS e nos recursos internos conectados.

Qual serviço pode ser empregado para atender a essa finalidade?

- AWS Direct Connect
    - Explicação: O AWS Direct Connect oferece uma conexão de rede dedicada entre seu data center e a AWS, proporcionando maior largura de banda, menor latência e transferência de dados mais segura e eficiente em comparação à internet pública.

- Amazon GuardDuty
    - Explicação: O Amazon GuardDuty é um serviço de detecção de ameaças que monitora continuamente atividades maliciosas e comportamento suspeito em suas contas e cargas de trabalho da AWS. Ele utiliza machine learning, análise comportamental e integração com fontes de inteligência de ameaças para identificar e alertar sobre possíveis riscos de segurança.

- **✅** AWS Certificate Manager
    - Explicação: O AWS Certificate Manager é um serviço da AWS que facilita a aquisição, implantação e gerenciamento de certificados SSL/TLS para recursos da AWS. Ele é é útil para proteger comunicações entre aplicativos e usuários, garantindo a segurança dos dados transmitidos.

- AWS KMS
    - Explicação: O AWS KMS não é adequado para criptografia de dados trocados diretamente com o usuário final porque é projetado para gerenciar e proteger chaves de criptografia usadas por aplicações e serviços dentro da AWS.

> **Explicação geral**:  
> O AWS Certificate Manager é um serviço da AWS que facilita a aquisição, implantação e gerenciamento de certificados SSL/TLS para recursos da AWS. Ele oferece certificados gratuitos gerenciados e também permite importar certificados existentes. O Certificate Manager é útil para proteger comunicações entre aplicativos e usuários, garantindo a segurança dos dados transmitidos. Pode ser usado em serviços como o Amazon CloudFront, Elastic Load Balancing e outros para habilitar o tráfego HTTPS. Ele automatiza a renovação de certificados e gerencia tarefas associadas à criptografia, simplificando a administração e a segurança de recursos na nuvem.


---

## Pergunta 64

Quais dos itens abaixo fazem parte dos pilares do Well-Architected Framework?

(Selecione 3 alternativas)

- **✅** Otimização de Custos
    - Explicação: Consiste em administrar os custos de TI para entregar valor ao negócio de forma econômica.

- **✅** Eficiência de Performance
    - Explicação: Diz respeito ao uso eficiente de recursos de TI para atender aos requisitos do sistema de maneira eficiente e flexível.

- Disponibilidade
    - Explicação: Apesar de a disponibilidade ser um componente crucial do pilar de Confiabilidade no AWS Well-Architected Framework, ela não é um dos seis pilares principais.

- Resiliência
    - Explicação: Apesar de a resiliência ser um componente crucial do pilar de Confiabilidade no AWS Well-Architected Framework, ela não é um dos seis pilares principais.

- **✅** Sustentabilidade
    - Explicação: Envolve a melhoria contínua da eficiência e redução do impacto ambiental dos sistemas em nuvem.

> **Explicação geral**:  
> O AWS Well-Architected Framework é composto por seis pilares que fornecem as melhores práticas e orientações para construir sistemas confiáveis, seguros, eficientes e rentáveis na nuvem. Esses pilares são:
> 
> - Excelência Operacional: Envolve a execução e monitoramento das operações do sistema para entregar valor de negócios e melhorar continuamente processos e procedimentos. Inclui práticas como automação de mudanças, resposta a eventos e definição de padrões operacionais.
> - Segurança: Foca na proteção de informações, sistemas e ativos, implementando controles rigorosos de acesso e resposta a incidentes. Inclui a gestão de identidades e permissões, criptografia de dados e monitoramento contínuo de ameaças e vulnerabilidades.
> - Confiabilidade: Assegura que um sistema possa se recuperar de falhas e cumprir suas funções pretendidas de forma consistente. Envolve práticas como recuperação de desastres, planejamento de capacidade e monitoramento de saúde do sistema.
> - Eficiência de Performance: Diz respeito ao uso eficiente de recursos de TI para atender aos requisitos do sistema de maneira eficiente e flexível. Envolve a seleção de tipos e tamanhos de recursos adequados, e o monitoramento de desempenho para fazer ajustes necessários.
> - Otimização de Custos: Consiste em administrar os custos de TI para entregar valor ao negócio de forma econômica. Envolve práticas como o uso de modelos de preços eficientes, desligamento de recursos não utilizados e otimização de uso de recursos.
> - Sustentabilidade: Envolve a melhoria contínua da eficiência e redução do impacto ambiental dos sistemas em nuvem. Inclui práticas como otimização de uso de recursos, escolha de arquiteturas eficientes em termos de energia e consideração de impactos ambientais no design de sistemas.
> 
> Esses pilares ajudam a garantir que as arquiteturas de sistemas na AWS sejam robustas, seguras, eficientes e alinhadas com os objetivos de negócio.


---

## Pergunta 65

Qual é o serviço de DNS da AWS que, entre outras coisas, transforma nomes de urls em código IP para acessar os recursos da Cloud?

- ACL
    - Explicação: ACL (Access Control List) é uma lista de regras que define quais usuários ou sistemas podem acessar determinados recursos e quais operações eles podem realizar. Em redes, as ACLs são usadas para controlar o tráfego de entrada e saída em roteadores e firewalls. No contexto de sistemas de arquivos e armazenamento, ACLs determinam as permissões de leitura, escrita e execução para arquivos e diretórios, permitindo uma gestão granular da segurança e acesso.

- Amazon ELB
    - Explicação: O Elastic Load Balancing distribui automaticamente o tráfego de entrada de aplicações entre diversos destinos, como instâncias do Amazon EC2, contêineres, endereços IP, funções do Lambda e dispositivos virtuais.

- AWS Auto Scaling
    - Explicação: O AWS Auto Scaling monitora os aplicativos e ajusta automaticamente a capacidade para manter um desempenho constante e previsível pelo menor custo possível.

- **✅** Amazon Route 53
    - Explicação: O Amazon Route 53 é o serviço de DNS da AWS que converte nomes de URLs em endereços IP para acessar recursos na nuvem. Além de roteamento de tráfego, ele oferece registro de domínio e monitoramento de integridade, garantindo alta disponibilidade e escalabilidade para suas aplicações.

> **Explicação geral**:  
> O Amazon Route 53 é o serviço de DNS da AWS que transforma nomes de URLs em endereços IP para acessar recursos na nuvem, facilitando a navegação e o roteamento de tráfego. Além disso, o Route 53 oferece funcionalidades como registro de domínio, permitindo que os usuários registrem e gerenciem seus próprios nomes de domínio diretamente na AWS. Ele também suporta roteamento de tráfego baseado em políticas, incluindo failover, geolocalização e balanceamento de carga, melhorando a disponibilidade e desempenho das aplicações. Com monitoramento de integridade integrado, o Route 53 pode detectar falhas nos endpoints e redirecionar o tráfego para recursos saudáveis, assegurando alta disponibilidade. Esses recursos tornam o Route 53 uma solução robusta para gerenciamento de DNS, adequando-se a diversos casos de uso em aplicações web, serviços de microserviços e sistemas distribuídos.

