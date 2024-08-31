## Pergunta 1

**Qual dos seguintes bancos de dados, conhecidos por suas características específicas de escalabilidade e flexibilidade, opera no modelo não relacional?**

- **✅** DynamoDB
    - O DynamoDB é o único não relacional da lista, os demais são todos relacionais.

- MariaDB
    - O MariaDB é um banco de dados relacional que utiliza tabelas estruturadas para armazenar dados em linhas e colunas, seguindo o modelo SQL. Na AWS, pode ser usado em instâncias do Amazon RDS para facilitar o gerenciamento e a escalabilidade, ou em instâncias EC2 para maior controle sobre a configuração.

- Oracle
    - O Oracle Database é um banco de dados relacional robusto e amplamente utilizado que pode ser implementado na AWS via Amazon RDS para gerenciamento simplificado e alta disponibilidade, ou no Amazon EC2 para maior controle e personalização.

- MySQL
    - O MySQL é um banco de dados relacional que pode ser utilizado no Amazon RDS para gerenciamento simplificado e alta disponibilidade, ou no Amazon EC2 para maior controle e personalização.

> **Explicação geral**:  
> O Amazon DynamoDB é um banco de dados NoSQL que se destaca por sua flexibilidade e escalabilidade, diferente dos bancos de dados relacionais. Ele não exige um esquema fixo para os dados, permitindo que você armazene dados em tabelas com um modelo de chave-valor. A chave é usada para identificar registros, enquanto o valor pode ser um documento JSON ou outros tipos de dados não estruturados. Isso permite que DynamoDB se adapte facilmente a diferentes tipos de dados e consultas, facilitando o trabalho com grandes volumes de dados variados.

---

## Pergunta 2

**Qual é a principal função para o NACL - Network Access Control List dentro de uma rede virtual privada da cloud?**

- É um serviço que lista todos os usuários que podem utilizar a rede através de acesso ssh

- **✅** É um serviço opcional que serve como um firewall para controlar o fluxo de entrada e saída de dados de uma ou mais subnets.
    - É uma camada de segurança opcional para sua VPC que funciona como firewall para controlar o tráfego de entrada e saída de uma ou mais sub-redes.

- É um serviço que lista todos os usuários que podem criar instâncias EC2 na rede
    - O NACL não lista usuários, ele gerencia uma lista de IPs para permitir ou negar o tráfego de entrada ou saída das subnets.

- É um serviço de uso obrigatório, que serve como um firewall para controlar o fluxo de entrada e saída de dados de uma ou mais subnets.
    - O uso de NACL não é obrigatório.

> **Explicação geral**:  
> Uma lista de controle de acesso (ACL) à rede é uma camada de segurança opcional para sua VPC que funciona como um firewall para controlar o tráfego de entrada e saída de uma ou mais sub-redes. Você pode configurar Network ACLs com regras semelhantes às dos grupos de segurança, permitindo ou negando tráfego com base em protocolos, portas e endereços IP de origem e destino. As ACLs de rede são avaliadas de forma sequencial, com cada regra sendo aplicada em ordem numérica. Elas fornecem uma camada adicional de segurança ao impedir que determinados tipos de tráfego indesejado entrem ou saiam de suas sub-redes. Network ACLs são particularmente úteis para estabelecer uma política de segurança consistente e granular em toda a VPC, complementando as regras dos grupos de segurança aplicadas nas instâncias individuais. Além disso, são ideais para cenários onde é necessário bloquear um tráfego específico em nível de subnet, fornecendo um controle mais detalhado sobre o fluxo de dados na sua infraestrutura de rede.

---

## Pergunta 3

**O Amazon EC2 é o principal serviço utilizado para processamento computacional em nuvem da AWS. Atualmente, qual é a menor instância, em relação ao processamento e memória ofertados pelo serviço?**

- m5dn.metal
    - A maior instância EC2 disponível na AWS é a "m5dn.metal", com capacidade para até 96 vCPUs e 384 GiB de memória RAM, oferecendo alto desempenho para cargas de trabalho intensivas e exigentes.

- t2.micro
    - A instância "t2.nano" é menor que a "t2.micro" em termos de recursos, possuindo 1 vCPU e 512 MiB de RAM, enquanto a "t2.micro" tem 1 vCPU e 1 GiB de RAM. A "t2.micro" é mais adequada para cargas de trabalho leves, como desenvolvimento e testes, enquanto a "t2.nano" é destinada a tarefas extremamente leves e com baixo consumo de recursos. Ambas as instâncias possuem a flexibilidade dos "créditos de CPU" para lidar com picos de atividade.

- m5.large
    - A instância intermediária EC2 da AWS, como a "m5.large", oferece um equilíbrio entre recursos e custo, com 2 vCPUs e 8 GiB de memória RAM. Ela é adequada para cargas de trabalho com demandas moderadas de recursos, como aplicativos da web, bancos de dados e ambientes de desenvolvimento.

- **✅** t2.nano
    - A menor instância EC2 disponível na AWS é a "t2.nano", com 1 vCPU e 512 MiB de memória RAM.

> **Explicação geral**:  
> A menor instância EC2 disponível na AWS é a "t2.nano", com 1 vCPU e 512 MiB de memória RAM. Projetada para cargas de trabalho muito leves, é ideal para tarefas simples e com baixo consumo de recursos. Também possui a flexibilidade dos "créditos de CPU". É importante considerar as necessidades específicas da aplicação antes de escolher o tipo de instância mais adequado para garantir o desempenho ideal.

---

## Pergunta 4

**Qual é a ferramenta feita para desenvolvedores e cientistas de dados prepararem, construirem, treinarem e implantarem seus modelos de aprendizado de máquina na AWS (ML-Machine Learning)?**

- Amazon EMR
    - O Amazon EMR é a plataforma de big data em nuvem líder do setor para processar grandes quantidades de dados usando ferramentas de código aberto.

- Amazon Step Function
    - O AWS Step Functions é um serviço de fluxo de trabalho visual que utiliza pouco código, usado para orquestrar serviços da AWS, automatizar processos de negócios e criar aplicações sem servidor. Os fluxos de trabalho gerenciam falhas, novas tentativas, paralelização, integrações de serviços e observabilidade, de modo que os desenvolvedores possam se concentrar na lógica de negócios com maior valor.

- **✅** Amazon SageMaker
    - A ferramenta da AWS destinada a desenvolvedores e cientistas de dados para preparar, construir, treinar e implantar modelos de aprendizado de máquina é o Amazon SageMaker.

- Amazon RedShift
    - Com o Redshift, você pode consultar e combinar exabytes de dados estruturados e semiestruturados em data warehouses, bancos de dados operacionais e seu data lake usando o SQL padrão.

> **Explicação geral**:  
> O Amazon SageMaker é um serviço gerenciado da AWS que facilita a preparação, construção, treinamento e implantação de modelos de aprendizado de máquina. Ele fornece um ambiente integrado para cientistas de dados e desenvolvedores, oferecendo ferramentas como notebooks Jupyter para exploração de dados e desenvolvimento de modelos. SageMaker suporta frameworks populares como TensorFlow, PyTorch, e Apache MXNet, permitindo flexibilidade no desenvolvimento. O serviço automatiza o ajuste de hiperparâmetros para otimizar os modelos e oferece escalabilidade automática durante o treinamento. SageMaker também simplifica a implantação de modelos em produção com endpoints de inferência gerenciados, garantindo alta disponibilidade e escalabilidade. Além disso, integrações com outros serviços AWS, como S3 e Lambda, aprimoram o fluxo de trabalho de machine learning, tornando-o uma solução abrangente para criar e gerenciar modelos de ML na nuvem.

---

## Pergunta 5

**Com qual serviço da AWS você pode identificar e refinar facilmente suas políticas para permitir o acesso de usuários e aplicações, apenas aos serviços que estão sendo utilizados, te ajudando a adotar da melhor forma o princípio do menor privilégio?**

- **✅** AWS IAM
    - O AWS Identity and Access Management (IAM) é um serviço que gerencia o acesso aos recursos da AWS de forma granular. Ele permite criar e gerenciar identidades (usuários, grupos, funções) e definir permissões para recursos específicos. O conceito de "menor privilégio" no IAM preconiza atribuir apenas as permissões necessárias para que os usuários ou sistemas realizem suas tarefas, minimizando riscos ao restringir o acesso excessivo a recursos sensíveis e aumentando a segurança geral da infraestrutura na nuvem.

- AWS MFA
    - O AWS MFA - Multi Facto Autenticator adiciona uma camada a mais na autenticação da sua conta.

- AWS Cognito
    - O AWS Cognito permite adicionar cadastramento, login e controle de acesso de usuários a aplicações Web e móveis, não a serviços da AWS.

- IAM AMI
    - Amazon Machine Image (AMI) é uma imagem pré-configurada usada para criar instâncias EC2 na AWS, contendo o sistema operacional, configurações e aplicativos necessários. AMIs facilitam o rápido provisionamento de novos servidores com configurações consistentes.

> **Explicação geral**:  
> O AWS Identity and Access Management (IAM) é um serviço que permite gerenciar o acesso aos recursos da AWS de forma granular. Ele possibilita a criação e gestão de identidades (usuários, grupos, funções) e a definição de permissões específicas para recursos. O IAM segue o princípio do "menor privilégio", que consiste em atribuir apenas as permissões estritamente necessárias para que usuários ou sistemas realizem suas tarefas. Isso minimiza riscos ao restringir o acesso excessivo a recursos sensíveis e melhora a segurança geral da infraestrutura na nuvem. Além disso, o IAM integra-se com outros serviços da AWS, permitindo políticas de segurança abrangentes e a capacidade de auditar e monitorar o uso e acesso através de serviços como AWS CloudTrail, garantindo conformidade e proteção robusta para suas operações na nuvem.

---

## Pergunta 6

**Qual serviço da AWS utiliza dispositivos físicos especializados para transferir grandes volumes de dados, enviando-os através de meios de transporte seguros para integrá-los na infraestrutura da AWS, especialmente útil para ambientes com conectividade limitada ou transferência massiva de dados?**

- AWS Direct Connect
    - O AWS Direct Connect estabelece uma conexão de rede dedicada entre sua infraestrutura on-premises e a AWS, enquanto a família AWS Snow utiliza dispositivos físicos para transferir grandes volumes de dados. Snow é ideal para ambientes com conectividade limitada ou para migração massiva de dados, onde o Direct Connect não é aplicável.

- AWS DMS
    - O AWS Database Migration Service (AWS DMS) ajuda você a migrar bancos de dados para a AWS de modo rápido e seguro. O banco de dados de origem permanece totalmente operacional durante a migração, minimizando o tempo de inatividade de aplicações que dependem do banco de dados.

- AWS DataSync
    - O AWS DataSync é um serviço de transferência de dados on-line que simplifica, automatiza e acelera a movimentação de dados entre os sistemas de armazenamento on-premises e os serviços de armazenamento da AWS, e também entre serviços de armazenamento da AWS.

- **✅** AWS Snowball
    - O AWS Snowball, da família Snow, é um dispositivo de computação, migração de dados e armazenamento de borda com duas opções. Os dispositivos do Snowball Edge Storage Optimized fornecem armazenamento de blocos e armazenamento de objetos compatível com o Amazon S3, além de 40 vCPUs. Ele é ideal para armazenamento local e transferência de dados em larga escala.

> **Explicação geral**:  
> O AWS Snowball, parte da família Snow, é um dispositivo de computação, migração de dados e armazenamento de borda com duas opções principais. Os dispositivos Snowball Edge Storage Optimized fornecem armazenamento de blocos e armazenamento de objetos compatível com o Amazon S3, além de 40 vCPUs, sendo ideais para armazenamento local e transferência de dados em larga escala. Para volumes ainda maiores, o AWS Snowmobile é um caminhão de transferência de dados capaz de mover exabytes de dados para a AWS, utilizando um contêiner seguro e protegido. A família Snow é projetada para ambientes com conectividade limitada ou para migrações massivas, onde métodos tradicionais, como AWS Direct Connect, não são viáveis.

---

## Pergunta 7

**Qual componente da infraestrutura global da AWS o Amazon CloudFront utiliza para garantir a baixa latência na distribuição de conteúdo?**

- Família Snow
    - O AWS Snow é uma família de dispositivos físicos usados para transferir grandes volumes de dados para dentro e fora da AWS de forma segura. CloudFront é ideal para distribuição rápida de conteúdo online, enquanto AWS Snow é utilizado para migração de dados em massa e em ambientes com conectividade limitada.

- ElastiCache
    - O Amazon CloudFront utiliza Pontos de Presença (PoPs) para entregar conteúdo com baixa latência, enquanto o Amazon ElastiCache melhora a performance de aplicativos através de caching em memória com Redis ou Memcached.

- **✅** Pontos de Presença
    - O Amazon CloudFront utiliza os Pontos de Presença (PoPs), que incluem Edge Locations e Regional Edge Caches, para garantir baixa latência na distribuição de conteúdo. Esses componentes da infraestrutura global da AWS permitem que o conteúdo seja entregue aos usuários de maneira rápida e eficiente, minimizando a distância entre os servidores de origem e os usuários finais.

- Partições
    - O Amazon CloudFront utiliza Pontos de Presença (PoPs) para garantir baixa latência na distribuição de conteúdo ao redor do mundo, enquanto particionamento (partitions) é uma técnica de armazenamento de dados que divide um banco de dados ou tabela em partes menores para melhorar a gestão e performance.

> **Explicação geral**:  
> O Amazon CloudFront utiliza Pontos de Presença (PoPs), incluindo Edge Locations e Regional Edge Caches, para garantir baixa latência na distribuição de conteúdo. Os PoPs estão estrategicamente localizados ao redor do mundo para minimizar a distância entre os servidores de origem e os usuários finais. Isso permite uma entrega de conteúdo rápida e eficiente, melhorando a experiência do usuário. CloudFront armazena em cache o conteúdo nos PoPs, reduzindo a carga nos servidores de origem e acelerando o tempo de resposta. Esse uso extensivo da infraestrutura global da AWS assegura que os dados sejam entregues de forma rápida e confiável.

---

## Pergunta 8

**Qual serviço oferece uma forma fácil de modelar uma coleção de recursos, relacionados da AWS e de terceiros, provisioná-los com rapidez e consistência e gerenciar todo o seu ciclo de vida mediante o tratamento da infraestrutura como código e versionamento?**

- **✅** AWS CloudFormation
    - O AWS CloudFormation é um serviço que permite criar e gerenciar recursos na AWS por meio de código, seguindo o conceito de Infrastructure as Code (IAC). IAC envolve definir a infraestrutura como código, permitindo automação, replicabilidade e controle versionamento.

- AWS YAML
    - Este serviço não existe, entretanto, "YAML" é um formato de arquivo que define os serviços através de identações no arquivo, que pode ser substituídos por aquivo JSON para implementar IAC.

- AWS Stack
    - Este serviço não existe, entretanto, uma "stack" no CloudFormation é a instância de execução de um template, representando um conjunto de recursos que são criados, atualizados ou excluídos juntos.

- AWS IAC
    - AWS IAC não existe. IAC é sigla de Infra as Code, que é um tipo de serviço que o CloudFormation oferece.

> **Explicação geral**:  
> O AWS CloudFormation é um serviço que permite criar e gerenciar recursos na AWS por meio de código, seguindo o conceito de Infrastructure as Code (IAC). Os templates são arquivos escritos em JSON ou YAML que descrevem a infraestrutura desejada, incluindo recursos como instâncias EC2, buckets S3 e bancos de dados RDS. Esses templates permitem automação, replicabilidade e controle de versionamento da infraestrutura. Uma "stack" no CloudFormation é a instância de execução de um template, representando um conjunto de recursos que são criados, atualizados ou excluídos juntos. O versionamento no CloudFormation facilita rastrear alterações nas configurações de infraestrutura ao longo do tempo, facilitando a colaboração, auditoria e reversão de mudanças quando necessário. Isso torna a gestão de ambientes em nuvem mais eficiente e controlada, promovendo boas práticas de DevOps e garantindo consistência na implantação de recursos.

---

## Pergunta 9

**Qual é o firewall da AWS que protege suas aplicações web de bots e outras ameaças comuns que podem afetar a disponibilidade e a performance dos seus serviços?**

- **✅** AWS WAF
    - O AWS WAF é um firewall de aplicações Web que ajuda a proteger suas aplicações Web ou APIs contra bots e exploits comuns na Web que podem afetar a disponibilidade, comprometer a segurança ou consumir recursos em excesso.

- AWS Shield
    - O AWS Shield é um serviço gerenciado de proteção contra DDoS (Negação de serviço distribuída) que protege os aplicativos executados na AWS. O AWS Shield oferece de detecção e mitigações em linha automáticas e sempre ativas que minimizam o tempo de inatividade e a latência dos aplicativos, fornecendo proteção contra DDoS sem necessidade de envolver o AWS Support.

- AWS CloudFront
    - O Amazon CloudFront é um serviço rápido de rede de entrega de conteúdo (CDN) que entrega dados, vídeos, aplicações e APIs a clientes em todo o mundo com segurança, baixa latência e altas velocidades de transferência em um ambiente de uso facilitado para desenvolvedores.

- AWS Certificate Manager
    - O AWS Certificate Manager é um serviço que permite provisionar, gerenciar e implantar facilmente certificados Secure Sockets Layer (SSL)/Transport Layer Security (TLS) para uso com os serviços da AWS e os recursos internos conectados.

> **Explicação geral**:  
> O AWS WAF é um firewall de aplicações web que protege suas aplicações web ou APIs contra bots e exploits comuns, como injeção SQL e cross-site scripting (XSS). Ele ajuda a manter a disponibilidade, a segurança e a performance, impedindo ataques que poderiam comprometer recursos e dados. O AWS WAF permite criar regras personalizadas para filtrar o tráfego HTTP/S com base em condições específicas, como endereços IP, strings de consulta, headers, e outros atributos. Integrado com serviços como Amazon CloudFront e Application Load Balancer, ele proporciona uma camada adicional de segurança e controle sobre o tráfego web. O WAF também oferece proteção contra ataques DDoS, complementando o AWS Shield.

---

## Pergunta 10

**Quais são os três principais tipos de cloud computing?**

(selecione 3 alternativas)

- **✅** PaaS - Plataforma como serviço
    - PaaS (Platform as a Service) fornece uma plataforma completa para desenvolvimento e implantação de aplicativos, com componentes gerenciados, como bancos de dados.

- BaaS - Backend como serviço
    - Existem outros tipos menos comuns com o BaaS (Backend como serviço), etc.

- **✅** SaaS - Software como serviço
    - SaaS (Software as a Service) oferece aplicativos completos hospedados na nuvem, como serviços de produtividade, sem a necessidade de gerenciar infraestrutura ou plataforma.

- **✅** IaaS - Infraestrutura como serviço
    - IaaS (Infrastructure as a Service) oferece recursos fundamentais de infraestrutura, como servidores virtuais e armazenamento, permitindo controle e configuração mais granulares.

> **Explicação geral**:  
> Os três principais tipos de computação em nuvem são infraestrutura como serviço, plataforma como serviço e software como serviço. Cada tipo de computação em nuvem oferece diferentes níveis de controle, flexibilidade e gerenciamento para que você possa selecionar o conjunto certo de serviços para as suas necessidades.

---

## Pergunta 11

**Sua empresa implementou alguns serviços que identificam problemas de segurança na sua infraestrutura da AWS. Qual é o serviço que, através de visualização interativa e unificada de seus recursos, usuários e interações, facilita a investigação e a identificação rápidas da causa raiz dos problemas de segurança ou atividades suspeitas na sua rede?**

- Amazon Macie
    - O Amazon Macie é um serviço de segurança e privacidade de dados totalmente gerenciado que usa machine learning e correspondência de padrões para descobrir e proteger seus dados confidenciais.

- AWS Security Hub
    - O AWS Security Hub é um serviço de gerenciamento de procedimentos de segurança na nuvem que realiza verificações de práticas recomendadas de segurança, agrega alertas e permite a correção automatizada.

- **✅** Amazon Detective
    - O serviço que facilita a investigação e a identificação rápidas da causa raiz de problemas de segurança ou atividades suspeitas na sua rede, através de visualização interativa e unificada de seus recursos, usuários e interações, é o AWS Detective.

- Amazon GuardDuty
    - O Amazon GuardDuty é um serviço de detecção de ameaças(não causa raiz) que monitora continuamente suas contas e workloads da para detectar atividade maliciosa e fornece resultados de segurança detalhados para visibilidade e correção.

> **Explicação geral**:  
> O Amazon Detective facilita a análise, a investigação e a identificação rápidas da causa raiz de potenciais problemas de segurança ou atividades suspeitas. O Amazon Detective coleta automaticamente dados de log de seus recursos da AWS e usa machine learning, análise estatística e teoria dos gráficos para criar um conjunto de dados vinculados que permite realizar facilmente investigações de segurança mais rápidas e eficientes. Pode analisar trilhões de eventos de várias fontes de dados, como Virtual Private Cloud (VPC) Flow Logs, AWS CloudTrail e Amazon GuardDuty, e criar automaticamente uma visualização interativa e unificada de seus recursos, usuários e interações entre eles ao longo do tempo. O foco do serviço é identificar a causa raiz.

---

## Pergunta 12

**O que o AWS Fargate adiciona ao Amazon ECS?**

- Balanceamento de Carga
    - Balanceamento de carga é com o ELB - Elastic Load Balancing.

- **✅** Execução de conteiner sem servidor
    - O AWS Fargate dispensa a configuração de servidores e diminui a mão de obra para o uso de conteiners ofertando execuções sem servidores.

- Orquestração com Kubernetes
    - Orquestração de Kubernetes é com o EKS - Elastic Kubernetes Service.

- Registro de Imagem
    - Registro de imagem é com o AMI - Amazon Management Image, se for de imagem docker é com o ECR - Elastic Conteiner Register.

> **Explicação geral**:  
> O AWS Fargate é um serviço que permite a execução de contêineres sem a necessidade de configurar e gerenciar servidores, reduzindo significativamente a carga de trabalho operacional. Com o Fargate, você apenas define as especificações dos contêineres, como CPU e memória, e o serviço cuida do provisionamento, escalabilidade e manutenção da infraestrutura subjacente. Isso elimina a necessidade de gerenciar clusters de EC2 ou ajustar a capacidade manualmente. Fargate é ideal para arquiteturas serverless, permitindo que as equipes de desenvolvimento se concentrem no design e na implementação das aplicações, sem se preocupar com a gestão da infraestrutura. Ele integra-se perfeitamente com Amazon ECS e EKS, oferecendo uma solução flexível e escalável para executar contêineres na AWS.

---

## Pergunta 13

**Quais são as principais características do Amazon Kinesis?**

(selecione duas alternativas)

- armazenar dados processados para gerar insights futuros.
    - O Amazon Kinesis é um serviço de processamento de dados em tempo real que coleta, processa e analisa dados em fluxo, mas não armazena os dados processados no próprio serviço. Em vez disso, ele pode encaminhar os dados processados para outros serviços de armazenamento da AWS, como Amazon S3, Amazon Redshift ou Amazon DynamoDB, para armazenamento e análise adicional.

- executar MapReduce
    - É o Amazon EMR que gerencia e facilita a execução de frameworks de big data, como Hadoop, incluindo o processamento de dados com MapReduce, em clusters escaláveis.

- **✅** gerar insights rápidos de acordo com os dados obtidos
    - O Kinesis permite que você obtenha insights imediatos sobre seus dados em fluxo, possibilitando a tomada de decisões rápidas.

- executar consultas SQL diretamente nos dados armazenados no Amazon S3
    - É o Amazon Athena que permite executar consultas SQL diretamente nos dados armazenados no Amazon S3, facilitando a análise de dados sem a necessidade de infraestrutura adicional.

- **✅** coletar, processar e analisar streaming de dados em tempo real
    - O Kinesis facilita a coleta, o processamento e a análise de dados de streaming em tempo real.

> **Explicação geral**:  
> O Kinesis facilita a coleta, o processamento e a análise de dados de streaming em tempo real, permitindo que você obtenha insights oportunos e reaja rapidamente às novas informações. Oferece recursos essenciais para processar dados de streaming em qualquer escala de forma econômica, além da flexibilidade de escolher as ferramentas mais adequadas aos requisitos dos aplicativos. Você pode consumir dados em tempo real como vídeo, áudio, logs de aplicativos, clickstreams de sites e dados de telemetria de IoT para machine learning, análises e outros aplicativos. O Kinesis permite processar e analisar dados assim que são recebidos e responder instantaneamente, em vez de aguardar a conclusão da coleta de dados para poder iniciar o processamento.

---

## Pergunta 14

**Qual é a forma de pagamento de instâncias EC2 que pode ser utilizada quando estima-se a utilização das instâncias por mais de 1 ano e que pode gerar uma economia de mais de 72% comparada ao on-demand (sob demanda)?**

- Spot
    - O Spot pode chegar a 90% de desconto se comparado com o OnDemand.

- **✅** Reserved
    - O modelo Reserved apresenta mais de 72% de economia em relação ao On-Demand, muito útil quando você tem a dimensão do processamento que vai utilizar. Também é útil quando a sua aplicação tem uma utilização que já te permite projetar o uso de máquina. Pode ser utilizada nas estimativas de 1 ou de 3 anos.

- On Demand
    - On-Demand é pago pelo uso, não precisa de reserva, é o modelo mais caro.

- Dedicated Host
    - O Dedicated Host pode chegar a 70% de desconto se comparado com o OnDemand.

> **Explicação geral**:  
> O modelo Reserved da AWS oferece mais de 72% de economia em comparação com o modelo On-Demand, sendo ideal para workloads previsíveis e estáveis. É especialmente útil quando você já conhece a dimensão do processamento necessário, permitindo planejar e comprometer-se com a capacidade de máquina a longo prazo. Com opções de reserva para períodos de 1 ou 3 anos, as Reserved Instances proporcionam custos significativamente reduzidos, garantindo economia para aplicações com utilização contínua. Além disso, ajuda a melhorar o planejamento financeiro e a gestão de recursos ao prever com precisão os custos futuros.

---

## Pergunta 15

**Todos os objetos do S3 são privados por default. Qual das opções abaixo é uma forma de permitir que pessoas ou aplicações consigam acessar esses objetos durante um período pré-determinado de tempo?**

- Alterando a propriedade do objeto para público
    - Uma forma de disponibilizar os arquivos na internet é deixando o bucket público, mas não é possível especificar o tempo para cada arquivo/objeto. Ficará público até que se configure o bucket.

- **✅** Gerando URLs pré assinadas
    - Gerando Presigned Urls você disponibiliza a url para um acesso específico, por um período específico. As URLs pré-assinadas do Amazon S3 são URLs temporárias geradas com base em chaves de acesso e segredos, permitindo acesso controlado a objetos no S3.

- Migrando o objeto para a classe Glacier do S3
    - A classe Glacier é utilizada para armazenar os arquivos com pouco uso, não está relacionado ao processo de acesso ao arquivo.

- Utilizando o Transfer Accelerator do S3
    - O Transfer Accelerator serve para otimizar o tempo de resposta de recuperação entre o usuário e o bucket através da infraestrutura de borda da AWS.

> **Explicação geral**:  
> URLs pré-assinadas do Amazon S3 são URLs temporárias geradas com base em chaves de acesso e segredos, permitindo acesso controlado a objetos no S3. Elas concedem permissões específicas por um período limitado, úteis para compartilhar conteúdo sem expor credenciais. Essas URLs são usadas para acesso seguro a recursos, como downloads ou uploads, sem a necessidade de autenticação direta. Elas são ideais para casos como compartilhamento de arquivos com clientes ou parceiros, uploads de arquivos por usuários externos e acesso temporário a recursos protegidos sem abrir mão da segurança.

---

## Pergunta 16

**Qual é a principal função do AWS Resource Access Manager (AWS RAM) em um ambiente onde sua empresa gerencia múltiplas contas e recursos na AWS?**

- Monitorar o tráfego de rede em tempo real na AWS.
    - Não monitora o tráfego de rede em tempo real.

- **✅** Compartilhar recursos com segurança entre contas da AWS e organizações.
    - A principal função do AWS Resource Access Manager (AWS RAM) é permitir o compartilhamento seguro e eficiente de recursos da AWS entre múltiplas contas dentro de uma organização. Isso facilita a colaboração e otimização de recursos, garantindo que diferentes contas possam acessar os recursos necessários de forma controlada e econômica.

- Controlar o acesso físico aos data centers da AWS.
    - Não controla o acesso físico aos data centers.

- Gerenciar recursos de computação na AWS.
    - Não é utilizado para gerenciar recursos de computação, mas para compartilhar recursos.

> **Explicação geral**:  
> O AWS Resource Access Manager (RAM) é um serviço da Amazon Web Services que permite compartilhar recursos com segurança entre contas da AWS e organizações. Ele simplifica o processo de compartilhamento de recursos, como instâncias do Amazon EC2, buckets do Amazon S3 e tabelas do Amazon DynamoDB, ao centralizar o gerenciamento de permissões e o controle de acesso em um único painel de controle. O RAM ajuda as organizações a otimizar o uso de recursos e a colaborar de maneira eficiente em ambientes de nuvem da AWS.

---

## Pergunta 17

**Qual serviço da AWS é ideal para realizar transferências de dados seguras e eficientes, sincronizando grandes volumes de dados entre ambientes on-premises e serviços de armazenamento na nuvem da AWS?**

- AWS DMS
    - O AWS DMS - Data Migration Service é utilizado para migrar banco de dados mantendo a disponibilidade e consistências dos mesmos.

- AWS Glue
    - O AWS Glue é o serviço utilizado para realizar ETL (Extrair, Tranformar e Carregar arquivos) na AWS.

- **✅** AWS DataSync
    - O AWS DataSync é um serviço online seguro que automatiza e acelera a movimentação de dados entre serviços de armazenamento on-premises e da AWS.

- AWS Glacier
    - O AWS Glacier é uma categoria de armazenamento do S3 utilizado para dados armazenar dados que são poucas vezes acessados e que permitem um tempo de resposta menos otimizado na sua recuperação.

> **Explicação geral**:  
> O AWS DataSync é um serviço online seguro que automatiza e acelera a movimentação de dados entre serviços de armazenamento on-premises e da AWS. O DataSync pode copiar dados entre compartilhamentos do Network File System (NFS), Server Message Block (SMB), Sistema de Arquivos Distribuídos do Hadoop (HDFS), armazenamento de objetos autogerenciado, AWS Snowcone, buckets do Amazon Simple Storage Service (Amazon S3), sistemas de arquivos do Amazon Elastic File System (Amazon EFS), sistemas de arquivos do Amazon FSx for Windows File Server, sistemas de arquivos do Amazon FSx for Lustre e sistema de arquivos do Amazon FSz for OpenZFS.

---

## Pergunta 18

**Quais mecanismos de segurança são usados para controlar o tráfego de entrada e saída de instâncias EC2, permitindo definir regras específicas para aumentar a proteção contra acessos não autorizados?**

- AWS IAM
    - O IAM é utilizado para gerenciar usuários, grupos e acesso a serviços.

- **✅** AWS Security Groups
    - Um grupo de segurança (security groups) atua como firewall virtual para as instâncias do EC2 visando controlar o tráfego de entrada e de saída. As regras de entrada controlam o tráfego de entrada para a instância e as regras de saída controlam o tráfego de saída da instância.

- AWS IAM Groups
    - o IAM Groups é utilizado para criar grupos de usuários para melhor gestão de acessos.

- AWS Auto Scalling Groups
    - Um Auto Scaling Group (ASG) gerencia o número de instâncias EC2 para manter a performance e a disponibilidade do aplicativo, ajustando automaticamente a capacidade conforme necessário. Ele difere dos security groups, que atuam como firewalls virtuais para controlar o tráfego de entrada e saída das instâncias EC2.

> **Explicação geral**:  
> Um grupo de segurança (security group) atua como um firewall virtual para instâncias EC2 dentro de uma VPC, controlando o tráfego de entrada e saída. As regras de entrada definem o tráfego permitido para a instância, enquanto as regras de saída determinam o tráfego permitido a sair da instância. Ao lançar uma instância EC2, você pode especificar um ou mais grupos de segurança; se nenhum for especificado, o grupo de segurança padrão é aplicado. Grupos de segurança são stateful, o que significa que respostas a tráfegos permitidos de entrada são automaticamente permitidas para sair, independentemente das regras de saída. Sub-redes dentro de uma VPC organizam instâncias EC2, e cada instância pode ter diferentes grupos de segurança, proporcionando controle granular e flexível da segurança do tráfego na rede.

---

## Pergunta 19

**Quando é dado o acesso a um usuário pelo IAM, qual dos seguintes princípios deve ser aplicado na concessão de acessos?**

- Princípio do alto privilégio
    - Enquanto "altos privilégios" implica em permissões extensas e abrangentes, o princípio dos Privilégios Mínimos no AWS IAM é o oposto. Este princípio consiste em conceder aos usuários apenas as permissões estritamente necessárias para suas funções específicas.

- Princípio do maior privilégio
    - Embora "maiores privilégios" impliquem em permissões extensas e abrangentes, o princípio dos Privilégios Mínimos no AWS IAM é o oposto. Este princípio consiste em conceder aos usuários apenas as permissões estritamente necessárias para suas funções específicas.

- Princípio de baixo privilégio
    - Embora "baixos privilégios" implique em permissões limitadas, o princípio dos Privilégios Mínimos no AWS IAM é mais específico. Ele consiste em conceder aos usuários apenas as permissões estritamente necessárias para suas funções específicas.

- **✅** Princípio do menor privilégio
    - O usuário deve começar sem nenhum acesso e ir recebendo os mesmos de acordo com a necessidade dele e da empresa, sempre com os menores privilégios e apenas para fazer o que realmente precisa.

> **Explicação geral**:
> No AWS Identity and Access Management (IAM), a abordagem de Privilégios Mínimos garante que os usuários começam sem nenhum acesso e recebem permissões específicas conforme necessário para suas funções. As permissões são concedidas através de políticas de acesso baseadas em função, ajustadas regularmente para assegurar que os usuários não tenham mais acesso do que o necessário. Permissões temporárias podem ser usadas para tarefas específicas, com monitoramento contínuo via ferramentas como AWS CloudTrail para revisar atividades e ajustar acessos. Educar os usuários sobre a importância dessa abordagem é crucial para manter a segurança e a conformidade​

---

## Pergunta 20

**Considerando a ampla gama de tipos de instâncias EC2 oferecidas pela AWS, qual das seguintes categorias não é uma opção disponível ao configurar uma instância na plataforma AWS?**

- Computação Acelerada
    - Accelerated Computing: Usam hardware especializado, como FPGAs, para acelerar tarefas específicas.

- **✅** Propósitos Específicos
    - Propósitos Específicos NÃO faz parte das categorias ofertadas para instâncias EC2.

- Computação Otimizada
    - Compute Optimized: Projetadas para cargas de trabalho intensivas em computação, como servidores web de alto desempenho e processamentos de lote.

- Propósitos Gerais
    - General Purpose: Equilibram recursos de computação, memória e rede, adequadas para uma variedade de cargas de trabalho.

> **Explicação geral**:  
> As categorias de instâncias EC2 oferecidas pela AWS são:
> 
> - General Purpose: Equilibram recursos de computação, memória e rede, adequadas para uma variedade de cargas de trabalho.
>   - Exemplos: T3, T3a, T2, M5, M5a, M4.
> 
> - Compute Optimized: Projetadas para cargas de trabalho intensivas em computação, como servidores web de alto desempenho e processamentos de lote.
>   - Exemplos: C5, C5n, C4.
> 
> - Memory Optimized: Para cargas de trabalho que processam grandes conjuntos de dados na memória, como bancos de dados de alta performance.
>   - Exemplos: R5, R5a, R4, X1, X1e, z1d.
> 
> - Storage Optimized: Oferecem alta capacidade de armazenamento, ideal para grandes bancos de dados e data warehouses.
>   - Exemplos: I3, I3en, D2, H1.
> 
> - GPU Instances: Projetadas para cargas de trabalho que requerem processamento paralelo massivo, como machine learning e computação científica.
>   - Exemplos: P3, P2, G3, G4.
> 
> - Accelerated Computing: Usam hardware especializado, como FPGAs, para acelerar tarefas específicas.
>   - Exemplos: F1, Inf1.
> 
> - High Memory: Fornecem grandes quantidades de memória para bancos de dados em memória, como SAP HANA.
>   - Exemplos: u-6tb1.metal, u-9tb1.metal, u-12tb1.metal.

---

## Pergunta 21

**Sua empresa estimou um gasto de US$ 12.000,00 por mês com infraestrutura AWS. Qual é o serviço que te auxilia, enviando mensagem, quando o consumo estiver atingindo um percentual pré-configurado deste valor?**

- AWS Pricing Calculator
    - O AWS Pricing Calculator é utilizado para estimar custo de uma infraestrutura que será implementada.

- **✅** AWS Budgets
    - O AWS Budgets ajuda a monitorar os gastos com infraestrutura AWS e envia notificações quando o consumo atinge um percentual pré-configurado do orçamento. Ele permite definir orçamentos específicos e configurar alertas por e-mail ou SMS para acompanhar e gerenciar os custos de forma eficiente.

- AWS Organizations
    - O AWS Organizations é utilizado para agrupar contas para a integração de serviços e gestão de custo.

- AWS Cost Explorer
    - O AWS Cost Explorer permite que você acompanhe os custos no detalhe, entretanto não tem a função e orçamentos e envio de email.

> **Explicação geral**:  
> O AWS Budgets/Orçamentos da AWS permite a definição de orçamentos personalizados para rastrear seu custo e uso, desde os casos de uso mais simples aos mais complexos. Com esse serviço, você pode escolher ser alertado por e-mail ou notificação SNS quando o custo real ou previsto e o uso excederem o limite do seu orçamento ou quando a utilização ou a cobertura reais de seus Savings Plans e RI cair abaixo do limite desejado. Com o AWS Budget Actions, você também pode configurar ações específicas para responder ao custo e ao status de uso em suas contas, de modo que se o seu custo ou uso exceder ou estiver previsto para exceder seu limite, as ações poderão ser executadas automaticamente ou com sua aprovação para reduzir o gasto em excesso não intencional.

---

## Pergunta 22

**Qual é o serviço gerenciado na nuvem AWS com o qual é possível configurar, gerenciar e dimensionar uma solução de pesquisa, de forma simples e econômica, para o seu site ou aplicativo?**

- Amazon ElasticSearchService
    - O ElasticSearchService fornece uma alta capacidade de armazenamento de dados de logs de serviços para permitir a análise de problemas e falhas de forma automatizada na sua infraestrutura.

- Amazon Athena
    - O Amazon Athena permite é um serviço serveless que permite a consulta através de queries SQL em dados armazenados em Bucket do S3.

- **✅** Amazon CloudSearch
    - O Amazon CloudSearch é um serviço gerenciado na nuvem AWS com o qual é possível configurar, gerenciar e dimensionar uma solução de pesquisa para o seu site ou aplicativo de forma simples e econômica.

- Amazon ElasticCache
    - O Amazon ElasticCache é um serviço que oferece uma solução de armazenamento de informações em cache de forma escalável.

> **Explicação geral**:  
> O Amazon CloudSearch é um serviço gerenciado na nuvem AWS que permite configurar, gerenciar e dimensionar uma solução de pesquisa para seu site ou aplicativo de forma simples e econômica. Suportando 34 idiomas, ele oferece recursos populares de pesquisa, como destaques, autopreenchimento e pesquisa geoespacial. CloudSearch pode ser integrado em sites e aplicativos através de APIs RESTful, permitindo que os desenvolvedores enviem dados de pesquisa e consultem o serviço para obter resultados de pesquisa relevantes. Ele também suporta indexação automática de dados, o que facilita a atualização e manutenção dos índices de pesquisa, garantindo que os usuários finais sempre recebam informações precisas e atualizadas. Essa integração permite que sites e aplicativos ofereçam funcionalidades de pesquisa avançadas, melhorando a experiência do usuário e aumentando a eficiência na recuperação de informações.

---

## Pergunta 23

**O que é um Bucket?**

- um banco de dados RDS
    - Amazon RDS (Relational Database Service) é um serviço gerenciado de banco de dados que facilita a configuração, operação e escalabilidade de bancos de dados na nuvem. Seus componentes principais incluem instâncias de banco de dados, snapshots, réplicas de leitura e grupos de parâmetros.

- Um container de microserviços no ECS
    - O Amazon ECS (Elastic Container Service) é um serviço gerenciado de orquestração de contêineres que facilita a execução, parada e gerenciamento de contêineres Docker em clusters. Seus componentes principais incluem clusters, serviços, tarefas e contêineres, além de integração com o AWS Fargate para execução sem gerenciamento de servidores.

- **✅** Um container de objetos do S3
    - Um bucket na Amazon S3 (Simple Storage Service) é um contêiner virtual para armazenar objetos, que podem ser arquivos, imagens, vídeos, documentos etc.

- Um container de arquivos do EFS
    - Amazon EFS (Elastic File System) é um serviço de armazenamento de arquivos totalmente gerenciado que fornece armazenamento escalável e elástico para uso com instâncias do Amazon EC2. Seus componentes principais incluem sistemas de arquivos, montagens de destino e políticas de acesso, permitindo compartilhamento de dados entre várias instâncias com baixa latência e alta durabilidade.

> **Explicação geral**:  
> Um bucket na Amazon S3 (Simple Storage Service) é um contêiner virtual para armazenar objetos, como arquivos, imagens, vídeos e documentos, cada um identificado de forma única por uma chave. Buckets S3 oferecem escalabilidade, durabilidade e segurança para armazenamento e acesso eficiente a grandes volumes de dados. Usos comuns incluem backup e recuperação de dados, hospedagem de sites estáticos e armazenamento para análises. Restrições incluem a necessidade de nomes de buckets únicos globalmente, limites de 100 buckets por conta (com possibilidade de aumento), e políticas de controle de acesso para segurança. O desempenho e os custos também variam conforme a região de armazenamento escolhida.

---

## Pergunta 24

**Qual serviço permite configurar múltiplos orçamentos para monitorar e controlar os custos de sua conta, alertando por e-mail quando os gastos se aproximam dos limites definidos, garantindo assim uma gestão financeira proativa e eficiente?**

- **✅** AWS Budgets
    - O AWS Budgets permite definir orçamentos para monitorar custos e uso, enviando alertas por e-mail ou SMS quando os limites são atingidos. Ele suporta até 10 endereços de e-mail para notificações, ajudando na gestão financeira proativa e eficiente.

- AWS Organization
    - O AWS Organizations permite consolidar diversas contas de uma organização para acompanhar seus custos e outras tarefas.

- AWS Billing Conductor
    - O AWS Billing Conductor é um serviço que permite às organizações personalizar, consolidar e alocar custos e faturas da AWS para unidades de negócios específicas, departamentos ou projetos. Ele facilita a criação de faturas personalizadas e a atribuição de custos detalhados, proporcionando uma visão mais precisa e granular dos gastos.

- AWS Cost Explorer
    - O AWS Cost Explorer permite que você explore os gastos detalhados da sua conta, porém não envia a notificação automática.

> **Explicação geral**:  
> O serviço da AWS que permite configurar múltiplos orçamentos para monitorar e controlar os custos de sua conta é o AWS Budgets. Com o AWS Budgets, você pode definir orçamentos específicos para custos e uso, e o serviço enviará alertas por e-mail ou SMS quando os gastos se aproximarem ou excederem os limites definidos. Isso ajuda a garantir uma gestão financeira proativa e eficiente, permitindo que você tome medidas antes de ultrapassar os orçamentos estabelecidos. Além disso, o AWS Budgets oferece uma interface intuitiva para acompanhar o progresso dos seus gastos em relação aos seus limites orçamentários, fornecendo insights valiosos para otimização de custos. É uma ferramenta essencial para manter o controle sobre os custos na nuvem, evitando surpresas indesejadas e facilitando o planejamento financeiro. O AWS Budgets permite enviar alertas para até 10 endereços de e-mail, garantindo que as partes interessadas relevantes sejam notificadas oportunamente.

---

## Pergunta 25

**Sua equipe desenvolveu uma aplicação para enviar um e-mail para os seus clientes avisando que a assinatura de um serviço anual irá vencer nos próximos 2 meses. Essa aplicação não precisa de alta disponibilidade e pode ser executada em qualquer horário do dia. Qual é a forma de uso de instâncias EC2 mais indicada para economizar custos nesta solução?**

- Dedicated Hosts
    - Os Dedicated Hosts são significativamente mais caros que as instâncias Spot, pois oferecem servidores físicos exclusivos para o seu uso, enquanto as instâncias Spot utilizam capacidade ociosa da AWS com grandes descontos, ideal para workloads flexíveis.

- Reserved
    - O Reserved oferece cargas de trabalho (work load) reservada permitindo que sua aplicação tenha uma alta disponibilidades dos recursos reservados para qualquer tipo de uso. Recomendado quando existe uma estimativa de uso entre 1 e 3 anos. Também é um plano que traz muita economia de recursos.

- **✅** Spot
    - O Spot permite que você economize custos usando alguns recursos quando ficam ociosos na AWS.  É recomendado para aplicativos que têm períodos de início e de término flexíveis, como o caso apresentado, pois os e-mails poderão ser enviados apenas quando existirem recursos disponíveis.

- On-Demand
    - O On-Demand oferece carga de trabalho (work load) para aplicações que não possuem uma carga de trabalho previsível, mas que requer alta disponibilidade.

> **Explicação geral**:  
> O Amazon EC2 Spot permite economizar custos utilizando capacidade ociosa da AWS, oferecendo instâncias com grandes descontos. É ideal para aplicativos com períodos de início e término flexíveis, como processamento de dados em lote, análises, CI/CD e renderização de mídia. No caso apresentado, e-mails podem ser enviados apenas quando os recursos Spot estão disponíveis, aproveitando a capacidade não utilizada sem comprometer a operação. Essa abordagem maximiza a eficiência e reduz significativamente os custos operacionais.

---

## Pergunta 26

**Você é o responsável por criar os microsserviços do seu time e escolheu utilizar o ECS para conteneirizar o ambiente e a aplicação. Agora você deseja criar uma imagem e compartilhar com o seu time e com a organização. Qual é o serviço da AWS recomendado para registrar e compartilhar essa imagem?**

- EC2
    - O EC2 - Elastic Computing Cloud é serviço que fornece várias opções de capacidades computacionais para você implementar uma grande variedade de aplicações e soluções.

- EMR
    - O EMR é a plataforma de Big Data em nuvem ofertado pela AWS.

- **✅** ECR
    - O Amazon Elastic Container Registry (ECR) é um serviço de registro de contêineres altamente escalável da AWS. Ele permite armazenar, gerenciar e implantar imagens de contêineres de maneira segura e eficiente.

- EKS
    - O EKS - Elastic Kubernetes Services é utilizado para orquestrar containers na sua arquitetura AWS.

> **Explicação geral**:  
> Para registrar e compartilhar imagens de contêineres na AWS, o serviço recomendado é o Amazon Elastic Container Registry (ECR). O Amazon ECR é um repositório de contêineres gerenciado que facilita o armazenamento, gerenciamento e implantação de imagens de contêineres. Ele oferece gerenciamento seguro de imagens com suporte a políticas de IAM, além de ser escalável para atender a qualquer demanda de aplicação. ECR se integra facilmente com pipelines de CI/CD, como AWS CodePipeline e AWS CodeBuild, e fornece alta disponibilidade e baixa latência para acesso às imagens. Usar o Amazon ECR com o ECS permite desenvolver, testar e implantar aplicativos de contêiner de forma rápida e eficiente, compartilhando imagens de maneira segura com seu time e organização.

---

## Pergunta 27

**A utilização de 750h por mês do EC2 faz parte de qual tipo de uso do nível gratuito (Free Tier)?**

- Always free (sempre livre)
    - O uso do EC2 não faz parte do modelo sempre livre.

- Trial (Experimentação Livre)
    - O uso do EC2 não faz parte do modelo experimentação livre.

- Spot
    - As instâncias Spot são uma opção de pagamento para EC2 que oferece economia significativa ao utilizar capacidade ociosa da AWS, com possibilidade de interrupção. Elas são distintas do nível gratuito, que oferece recursos limitados sem custo para novos usuários.

- **✅** 12 months free (12 meses livre)
    - O uso da EC2 neste formato só possui gratuidade nos 12 primeiros meses.

> **Explicação geral**:  
> O uso da EC2 neste formato só possui gratuidade nos 12 primeiros meses.
> 
> A free tier (nível gratuito) está disponível em 3 modelos:
> 
> - Serviços para uso em 12 meses
> - Experimentação livre
> - Serviços sempre gratuitos.

---

## Pergunta 28

**Sua equipe de desenvolvimento está montando um pipeline de integração contínua e deseja implementar algum serviço para gerenciamento de código. Por questões jurídicas, as opções mais usuais do mercado foram descartadas. Qual é o serviço da AWS que fornece repositórios gits privados para o gerenciamento de código?**

- AWS Checkout
    - Este não é um serviço ofertado pela AWS.

- AWS CodeBuild
    - O AWS CodeBuild pode ser utilizado para compilar e testar a sua aplicação na pipeline de CI/CD.

- **✅** AWS CodeCommit
    - O AWS CodeCommit é um serviço de controle de origem gerenciado seguro e altamente dimensionável que hospeda repositórios privados do Git. Ele torna mais fácil para as equipes colaborarem com segurança no código com contribuições criptografadas em trânsito e em repouso.

- AWS Git
    - Este não é um serviço ofertado pela AWS.

> **Explicação geral**:  
> O AWS CodeCommit é um serviço de controle de versão gerenciado, seguro e altamente escalável que hospeda repositórios privados do Git. Ele facilita a colaboração segura nas equipes, com contribuições criptografadas em trânsito e em repouso. Com o CodeCommit, não é necessário gerenciar seu próprio sistema de controle de versão ou se preocupar com o dimensionamento da infraestrutura. O serviço pode armazenar qualquer tipo de item, desde código-fonte até binários. Além disso, por ser compatível com as funcionalidades padrão do Git, ele se integra perfeitamente com as ferramentas baseadas em Git já existentes, garantindo uma transição e operação suaves para os desenvolvedores.

---

## Pergunta 29

**Para publicar um site estático com custo mínimo e alta escalabilidade, qual serviço da AWS você deve utilizar, considerando que ele oferece durabilidade de 99,999999999%, suporta hospedagem de arquivos estáticos, e é amplamente integrado com outros serviços AWS para entrega eficiente de conteúdo?**

- Amazon EFS
    - EFS - Elastic File System - permite a hospedagem de um site, mas terá a necessidade de associação a uma máquina EC2, o que aumentará bastante o custo da implementação.

- Amazon EC2 rodando Windows
    - EC2 - Elastic Computing Cloud permite a hospedagem de um site, mas o custo será maior, pois haverá provisionamento de disco, processamento, memória e redes.

- **✅** Amazon S3
    - Um dos recursos do S3 é a hospedagem de um site estático de forma rápida e barata, sem servidor. Para isso é necessário criar um bucket, configurá-lo para ser um site estático e então fazer o upload dos arquivos html, css, js, etc.

- Amazon EC2 rodando Linux
    - EC2 - Elastic Computing Cloud permite a hospedagem de um site, mas o custo será maior, pois haverá provisionamento de disco, processamento, memória e redes.

> **Explicação geral**:  
> Um dos recursos do Amazon S3 é a hospedagem de um site estático de forma rápida e barata, sem necessidade de servidor. Para isso, é necessário criar um bucket no S3 e configurá-lo para a hospedagem de site estático. Depois, faça o upload dos arquivos HTML, CSS, JS e outros recursos do site. Configure as permissões do bucket para permitir o acesso público aos arquivos, e especifique os documentos de índice e erro. O S3 gerará um endpoint que pode ser utilizado para acessar o site. Essa abordagem proporciona alta durabilidade e disponibilidade com um custo mínimo, ideal para sites estáticos.

---

## Pergunta 30

**Qual é o serviço que coleta dados de monitoramento e operações na forma de logs, métricas e eventos e os exibe usando painéis automatizados para que você tenha uma visão unificada dos recursos, aplicativos e serviços executados na AWS e em servidores locais?**

- **✅** AWS CloudWatch
    - O Amazon CloudWatch monitora os recursos da Amazon Web Services (AWS) e as aplicações executadas na AWS em tempo real. Você pode usar o CloudWatch para coletar e monitorar métricas, que são as variáveis que é possível medir para avaliar seus recursos e suas aplicações.

- AWS GuardDuty
    - O Amazon GuardDuty é um serviço de detecção de ameaças que monitora continuamente atividades mal-intencionadas e comportamentos não autorizados para proteger suas contas, cargas de trabalho e dados da AWS armazenados no Amazon S3.

- AWS Macie
    - O Amazon Macie é um serviço de segurança e privacidade de dados totalmente gerenciado que usa machine learning e correspondência de padrões para descobrir e proteger seus dados confidenciais na AWS.

- AWS Inspector
    - O Amazon Inspector é um serviço de avaliação de segurança automático que ajuda a melhorar a segurança e a conformidade dos aplicativos implantados na AWS. O Amazon Inspector avalia automaticamente aplicativos em busca de exposições, vulnerabilidades ou discrepâncias em relação às melhores práticas.

> **Explicação geral**:  
> O Amazon CloudWatch monitora os recursos da Amazon Web Services (AWS) e as aplicações executadas na AWS em tempo real. Você pode usar o CloudWatch para coletar e monitorar métricas, que são as variáveis que é possível medir para avaliar seus recursos e suas aplicações. A página inicial do CloudWatch exibe automaticamente métricas sobre cada produto da AWS usado. Também crie painéis personalizados para exibir métricas sobre os aplicativos personalizados e exibir coleções personalizadas de métricas escolhidas. É possível criar alarmes que observem métricas e enviem notificações ou façam alterações automaticamente nos recursos que você está monitorando quando um limite é violado.

---

## Pergunta 31

**Sobre o gerenciamento de Grupos no AWS IAM, podemos afirmar que:**

(Selecione 3 alternativas)

- **✅** Um Grupo pode conter diversos usuários
    - Um grupo no AWS IAM pode conter vários usuários, facilitando o gerenciamento de permissões coletivas para esses usuários. Isso simplifica a atribuição e a gestão de acesso aos recursos da AWS de forma centralizada.

- **✅** Os grupos não pode ser aninhados, eles só podem conter usuários
    - Os grupos no AWS IAM não podem ser aninhados; eles só podem conter usuários. Isso significa que não é possível criar uma hierarquia de grupos dentro de outros grupos. Para gerenciar permissões, você deve criar grupos diferentes para cada necessidade específica e adicionar os usuários diretamente a esses grupos.

- O número e o tamanho dos grupos do AWS IAM são virtualmente ilimitados.
    - O número e o tamanho dos grupos no AWS IAM não são virtualmente ilimitados. Existem limites específicos estabelecidos:
        - Número de Grupos: Você pode criar até 300 grupos IAM por conta AWS.
        - Usuários por Grupo: Um grupo IAM pode conter até 1.000 usuários.
        - Grupos por Usuário: Cada usuário IAM pode ser membro de até 10 grupos.

- Você não pode criar grupos de usuário padrão e incluir todos os usuários da conta da AWS
    - Você pode sim criar grupos no AWS IAM e adicionar todos os usuários da conta a esses grupos. Isso facilita a aplicação de permissões e políticas de acesso comuns a todos os usuários. No entanto, é necessário respeitar os limites de IAM, como o máximo de 1.000 usuários por grupo e 10 grupos por usuário. Essas restrições são importantes para garantir a eficiência e a segurança na gestão de identidades e acessos na AWS.

- **✅** Um usuário pode pertencer a vários grupos
    - Um usuário no AWS IAM pode pertencer a vários grupos simultaneamente, permitindo a combinação de permissões de diferentes grupos para esse usuário. Isso facilita a gestão de acessos, permitindo atribuir permissões de forma flexível e modular.

> **Explicação geral**:  
> O IAM Groups é um recurso do AWS IAM que permite criar grupos de usuários para gerenciar permissões e acesso a serviços dentro da sua conta AWS. Por exemplo, você pode criar um grupo de desenvolvedores (DEVs) com acesso apenas a serviços como CodeCommit e CodeBuild, ou um grupo de administradores de banco de dados (DBAs) com acesso apenas a RDS e DynamoDB. Um grupo pode conter vários usuários, e um usuário pode pertencer a mais de um grupo simultaneamente. No entanto, para cada necessidade específica, é necessário criar um grupo separado.

---

## Pergunta 32

**Qual das opções abaixo é um serviço Amazon para gerenciar pacotes de softwares e suas dependências?**

- AWS CodeCommit
    - O CodeCommit para gerenciar o código fonte baseado em git.

- AWS CodeBuild
    - O CodeBuild é para compilar e testar as aplicações.

- AWS CodeDeploy
    - O CodeDeploy para implantar os aplicativos em seus destinos, servidores e serviços.

- **✅** AWS CodeArtifact
    - O AWS CodeArtifact é um serviço de gerenciamento e armazenamento de pacotes de software que facilita o compartilhamento, controle de versões e segurança de artefatos de desenvolvimento, como bibliotecas de código e dependências.

> **Explicação geral**:  
> O AWS CodeArtifact é um serviço de gerenciamento e armazenamento de pacotes de software que facilita o compartilhamento, controle de versões e segurança de artefatos de desenvolvimento, como bibliotecas de código e dependências. Ele oferece um repositório centralizado e seguro para armazenar e compartilhar pacotes, integrando-se a ferramentas populares de desenvolvimento e permitindo que equipes colaborem eficientemente. O CodeArtifact ajuda a reduzir a complexidade na gestão de pacotes, melhorando a escalabilidade e a confiabilidade no ciclo de desenvolvimento de software na AWS.

---

## Pergunta 33

**Qual é o serviço da AWS que permite criar uma imagem a partir de uma EC2 configurada para ser utilizada em serviços como Auto Scaling, DR, entre outros?**

- **✅** AMI
    - Com o AMI você pode salvar imagens de suas instância EC2 configuradas para fazer uso em Auto Scalling, DR, entre outros. A AWS Amazon Machine Image (AMI) é uma imagem pré-configurada usada para criar instâncias de máquinas virtuais na nuvem.

- AWS Workspaces
    - O AWS Workspaces é um serviço que fornece desktops windows e linux de forma virtualizada.

- AWS Config
    - O AWS Config é um serviço para gerenciar e monitorar as configurações de diversos serviços da AWS.

- AWS Image
    - O AWS Image não é um serviço existente na AWS.

> **Explicação geral**:  
> A AWS Amazon Machine Image (AMI) é uma imagem pré-configurada usada para criar instâncias de máquinas virtuais na nuvem, incluindo sistema operacional e software pré-instalado. Com o AMI, você pode salvar imagens de suas instâncias EC2 configuradas para uso em Auto Scaling, recuperação de desastres (DR) e outros fins. Isso agiliza o processo de implantação e permite a replicação consistente de ambientes, essencial para o rápido provisionamento de recursos na AWS. As AMIs facilitam a criação de instâncias consistentes, melhorando a eficiência operacional e a gestão de infraestrutura na nuvem.

---

## Pergunta 34

**Qual é a plataforma líder do setor para processamento de big data, análise interativa e machine learning na nuvem, que utiliza estruturas de código aberto na AWS?**

- **✅** Amazon EMR
    - O Amazon Elastic MapReduce (EMR) é um serviço de big data da AWS, líder do setor, que simplifica o processamento e análise de grandes conjuntos de dados. Ele utiliza frameworks como Hadoop e Spark para distribuir e processar tarefas em clusters de máquinas virtuais. O EMR é ideal para tarefas de processamento intensivo, mineração de dados e análises avançadas, permitindo dimensionamento flexível e eficiente.

- Amazon DataSync
    - O AWS DataSync é um serviço de transferência de dados on-line que simplifica, automatiza e acelera a movimentação de dados entre os sistemas de armazenamento on-premises e os serviços de armazenamento da AWS.

- Amazon Redshift
    - O Amazon Redshift é o serviço de data warehouse voltado para BI.

- Amazon DMS
    - O Amazon DMS é o serviço para migração de bancos de dados.

> **Explicação geral**:  
> A plataforma líder do setor para processamento de big data, análise interativa e machine learning na nuvem que utiliza estruturas de código aberto na AWS é o Amazon EMR. O Amazon EMR facilita a execução de frameworks como Apache Hadoop, Spark, HBase e Presto, permitindo o processamento e análise de grandes volumes de dados de maneira escalável e econômica. Ele integra-se com outros serviços da AWS, como S3, RDS e DynamoDB, para oferecer uma solução completa e eficiente para big data. Com o Amazon EMR, é possível realizar análises complexas, transformar dados em larga escala e aplicar machine learning de forma otimizada.

---

## Pergunta 35

**Qual é o serviço que monitora os aplicativos e que ajusta automaticamente a capacidade de instâncias para manter um desempenho constante e previsível pelo menor custo possível?**

- AWS Fargate
    - O AWS Fargate é um mecanismo de computação sem servidor para contêineres que funciona com o ECS e com o EKS. O Fargate facilita a sua concentração no desenvolvimento de aplicativos. O Fargate elimina a necessidade de provisionar e gerenciar servidores, permite que você especifique e pague pelos recursos por aplicativo, além de aumentar a segurança ao conceber aplicativos isolados.

- AWS Elastic Container Service
    - O Amazon Elastic Container Service (Amazon ECS) é um serviço totalmente gerenciado de orquestração de contêineres que ajuda a implantar, gerenciar e escalar facilmente aplicações conteinerizadas. Ele se integra completamente ao restante da plataforma AWS para fornecer uma solução segura e fácil de usar para a execução de workloads de contêiner na nuvem.

- **✅** AWS Auto Scaling Group
    - O AWS Auto Scaling é o serviço mais importante para que a escalabilidade ocorra e traga redução de custos e aumento de disponibilidade e performance no uso das instâncias EC2. Permite ajustar automaticamente a capacidade de instâncias EC2 com base na demanda em tempo real.

- AWS Elastic Load Balancer
    - O Elastic Load Balancing distribui automaticamente o tráfego de entrada de aplicações entre diversos destinos, como instâncias do Amazon EC2, contêineres, endereços IP, funções do Lambda e dispositivos virtuais.

> **Explicação geral**:  
> O AWS Auto Scaling é o serviço mais importante para que a escalabilidade ocorra e traga redução de custos e aumento de disponibilidade e performance no uso das instâncias EC2. Permite ajustar automaticamente a capacidade de instâncias EC2 com base na demanda em tempo real. Com ele, é possível definir políticas de dimensionamento que controlam a adição ou remoção de instâncias, garantindo que a aplicação sempre tenha a quantidade adequada de recursos para lidar com a carga de trabalho. O Auto Scaling Group monitora métricas de utilização, como CPU, para tomar decisões inteligentes sobre o escalonamento. Além disso, ele suporta a configuração de diferentes zonas de disponibilidade para garantir alta disponibilidade da aplicação. Esse serviço é fundamental para otimizar o desempenho e a eficiência dos ambientes na nuvem AWS.

---

## Pergunta 36

**Você precisa migrar uma grande quantidade de dados do seu ambiente on-premise para armazenamento no S3 de forma automática e periódica, liberando a capacidade da sua infraestrutura particular. Qual serviço pode ser utilizado para essa finalidade?**

- AWS VPN
    - Virtual Private Network - As soluções do AWS Virtual Private Network estabelecem conexões seguras entre redes locais, escritórios remotos, dispositivos de clientes e a rede global da AWS.

- AWS DMS
    - O AWS Database Migration Service (AWS DMS) ajuda a migrar bancos de dados para a AWS com facilidade, segurança e baixo custo.

- AWS DirectConnect
    - O AWS Direct Connect é uma solução de serviço de nuvem que facilita o estabelecimento de uma conexão de rede dedicada entre suas instalações e a AWS. Usando o AWS Direct Connect, você cria uma conexão privada entre a AWS e seu datacenter, escritório ou ambiente de localização.

- **✅** AWS DataSync
    - O AWS DataSync é um serviço da AWS que facilita a transferência de dados entre sistemas de armazenamento locais e a nuvem de maneira rápida e segura. Ele oferece transferências otimizadas, agendamento flexível e criptografia para mover dados entre ambientes, como servidores locais e armazenamento Amazon S3 ou Amazon EFS.

> **Explicação geral**:  
> Para migrar uma grande quantidade de dados do seu ambiente on-premises para o Amazon S3 de forma automática e periódica, liberando a capacidade da sua infraestrutura particular, você pode utilizar o AWS DataSync. O AWS DataSync é um serviço gerenciado que automatiza e acelera a transferência de dados entre sistemas de armazenamento on-premises e os serviços de armazenamento da AWS, como S3, EFS e FSx. Com o AWS DataSync, você pode configurar tarefas de transferência de dados periódicas, definindo a frequência e as janelas de tempo para que as transferências ocorram automaticamente. O serviço utiliza mecanismos de otimização para garantir que as transferências sejam rápidas e seguras, incluindo a capacidade de transferir dados criptografados em trânsito e validar a integridade dos dados transferidos. DataSync é ideal para mover grandes volumes de dados de maneira eficiente, reduzindo a carga na sua infraestrutura local.

---

## Pergunta 37

**Sua empresa deseja implementar um sistema que leia normas internas e as reproduzam através de falas humanas com aparência natural para auxiliar pessoas com baixa ou nenhuma condição de leitura. Qual serviço pode auxiliar a construção deste sistema através de Machine Learning?**

- Amazon Transcribe
    - O Amazon Transcribe é um serviço da AWS que permite aos clientes converter facilmente discurso em texto. Usando a tecnologia Automatic Speech Recognition (ASR – Reconhecimento automático de fala), os clientes podem optar por usar o Amazon Transcribe em uma variedade de aplicativos de negócios, incluindo a transcrição de chamadas de voz do atendimento ao cliente, a geração de legendas em conteúdo de áudio/vídeo e a realização de análise de conteúdo (baseada em texto) de áudio/vídeo.

- Amazon Translate
    - O Amazon Translate é um serviço de tradução automática neural que fornece traduções de idiomas com rapidez, alta qualidade, acessíveis e personalizáveis. A tradução automática neural é um tipo de automação de tradução de idiomas que usa modelos de aprendizado profundo para entregar traduções que soam mais precisas e naturais do que as oferecidas por algoritmos de tradução tradicionais estatísticos e baseados em regras.

- **✅** Amazon Polly
    - Para implementar um sistema que leia normas internas e as reproduza com fala natural, ajudando pessoas com baixa ou nenhuma condição de leitura, utilize o Amazon Polly. Amazon Polly converte texto em fala realista usando Machine Learning, oferecendo várias vozes e idiomas para criar uma experiência auditiva clara e acessível.

- Amazon Lex
    - O Amazon Lex é um serviço da AWS para a criação de interfaces de conversa para qualquer aplicativo que usa voz e texto. Com o Amazon Lex, o mesmo mecanismo de conversa da plataforma do Amazon Alexa agora está disponível para todos os desenvolvedores, permitindo que você crie chatbots sofisticados em linguagem natural em aplicativos novos e existentes.

> **Explicação geral**:  
> O Amazon Polly é um serviço que transforma texto em falas realistas, permitindo que você crie aplicativos que falam e desenvolva categorias totalmente inéditas de produtos compatíveis com fala. O serviço de conversão de texto em fala (TTS) do Polly usa tecnologias avançadas de aprendizagem profunda para sintetizar falas humanas com aparência natural. Com dezenas de vozes realistas em vários idiomas, você pode criar aplicativos com recursos integrados de fala que funcionam em vários países diferentes.

---

## Pergunta 38

**Qual dos itens abaixo fazem parte do Well-Architected-Framework?**

(Selecione duas alternativas)

- **✅** Segurança
    - Este item faz parte de um dos 6 pilares do Framework.

- **✅** Performance Eficiente
    - Este item faz parte de um dos 6 pilares do Framework.

- Desacoplamento
    - Desacoplamento, embora importante, não é listado separadamente entre os seis pilares da AWS porque é um princípio arquitetônico que está incluído em Excelência Operacional e Desempenho Eficiente. Ele contribui para a construção de sistemas mais robustos e escaláveis, que são objetivos desses pilares, garantindo que os componentes possam ser gerenciados e escalados independentemente.

- Monitoramento
    - Monitoramento, embora crucial, não é listado separadamente entre os seis pilares da AWS porque está integrado dentro de Excelência Operacional e Confiabilidade. Esses pilares abrangem a importância de monitorar e otimizar sistemas continuamente para garantir desempenho eficiente e detectar problemas rapidamente, contribuindo para a robustez e eficiência geral dos serviços.

- Resiliência
    - Resiliência, apesar de importante, não é listada separadamente entre os seis pilares da AWS porque seus aspectos são incorporados em pilares como Confiabilidade e Segurança. A Confiabilidade já abrange a capacidade de recuperação rápida de falhas, enquanto a Segurança contribui para a continuidade dos serviços. Portanto, resiliência é tratada como parte integral desses conceitos.

> **Explicação geral**:  
> Os pilares da AWS são fundamentais para criar uma infraestrutura de TI robusta e eficiente.
> 
> - Excelência Operacional envolve a execução e monitoramento dos sistemas para entregar valor de negócio.
> - Segurança abrange a proteção de informações e sistemas através de medidas rigorosas de controle de acesso e criptografia.
> - Confiabilidade assegura que os sistemas possam se recuperar rapidamente de falhas e continuar operando.
> - Desempenho Eficiente refere-se ao uso eficiente dos recursos para manter um desempenho ideal.
> - Otimização de Custos envolve o gerenciamento de recursos para minimizar custos sem comprometer a performance.
> - Sustentabilidade foca em minimizar o impacto ambiental ao utilizar práticas e tecnologias eco-friendly.

---

## Pergunta 39

**Quais dos seguintes bancos de dados são totalmente gerenciados pela AWS?**

(Escolha 3 alternativas)

- **✅** Redshift
    - Amazon Redshift é um serviço de data warehouse totalmente gerenciado pela AWS, projetado para análise de grandes volumes de dados com alta performance e escalabilidade. Ele utiliza técnicas como armazenamento em colunas e processamento paralelo, oferecendo uma relação custo-benefício superior para cargas de trabalho analíticas em petabytes de dados.

- **✅** Aurora
    - Amazon Aurora é um banco de dados relacional totalmente gerenciado pela AWS, compatível com MySQL e PostgreSQL. Ele oferece alta performance, escalabilidade automática, e armazenamento distribuído tolerante a falhas, proporcionando até cinco vezes a performance do MySQL e três vezes a do PostgreSQL.

- MySQL
    - Quando utilizado com o RDS é totalmente gerenciado pela AWS, quando instalado em uma instância EC2 requer gerenciamento manual, incluindo instalação, manutenção e backups.

- Oracle
    - Quando utilizado com o RDS é totalmente gerenciado pela AWS, quando instalado em uma instância EC2 requer gerenciamento manual, incluindo instalação, manutenção e backups.

- **✅** DynamoDB
    - Amazon DynamoDB é um banco de dados NoSQL totalmente gerenciado pela AWS, projetado para oferecer performance rápida e previsível com escalabilidade automática.

> **Explicação geral**:  
> Bancos de dados totalmente gerenciados pela AWS, como Amazon Aurora, DynamoDB e Redshift, automatizam tarefas administrativas, incluindo provisionamento, backups e atualizações, garantindo alta disponibilidade e escalabilidade. Amazon RDS também gerencia bancos como MySQL e Oracle, oferecendo uma solução simplificada para esses sistemas. Em contraste, quando MySQL e Oracle são instalados em instâncias EC2, o gerenciamento é manual, exigindo que o usuário cuide de todas as tarefas administrativas, como instalação, manutenção e backups. A escolha entre soluções gerenciadas e não gerenciadas depende das necessidades específicas de controle versus conveniência operacional.

---

## Pergunta 40

**Você iniciou um trabalho de estimativa de custos de uma infraestrutura que precisa implementar para sua empresa na AWS. Qual dos serviços abaixo pode te apoiar?**

- AWS Organizations
    - O AWS Organizations ajuda a gerenciar e controlar múltiplas contas da AWS.

- AWS Cost Explorer
    - O AWS Cost Explorer é utilizado para a consulta dos custos já associados aos serviços já utilizados na sua conta.

- AWS Budgets
    - O AWS Budgets é utilizado para a definição, controle e monitoramento de orçamentos.

- **✅** AWS Pricing Calculator
    - O AWS Pricing Calculator é uma ferramenta online da Amazon Web Services que permite estimar os custos associados ao uso de serviços em sua plataforma de nuvem. Ele ajuda os usuários a planejar e prever despesas, fornecendo uma visão detalhada dos preços de serviços, recursos e regiões.

> **Explicação geral**:  
> O AWS Pricing Calculator é uma ferramenta online da Amazon Web Services que permite estimar os custos associados ao uso de serviços em sua plataforma de nuvem. Ele é especialmente útil para quem ainda não utiliza a AWS e deseja migrar suas cargas de trabalho, pois ajuda a planejar e prever despesas de forma detalhada. A ferramenta fornece uma visão clara dos preços dos serviços, recursos e regiões, permitindo que os usuários ajustem parâmetros para modelar diferentes cenários. Isso facilita a tomada de decisões informadas sobre a infraestrutura e os serviços mais adequados às necessidades específicas, garantindo uma migração eficiente e econômica.

---

## Pergunta 41

**O que o Amazon EKS adiciona ao Amazon ECS?**

- Computação sem servidor
    - O serviço responsável por computação sem servidor na AWS é o AWS Lambda ou Fargate, que permitem executar código em resposta a eventos sem a necessidade de provisionar ou gerenciar servidores.

- Registro de imagem de contêiner
    - O serviço responsável por registro de imagem de contêiner na AWS é o Amazon Elastic Container Registry (ECR), que facilita o armazenamento, gerenciamento e implantação de imagens de contêiner Docker de forma segura e escalável.

- **✅** Orquestração de contêineres usando Kubernetes
    - O Amazon EKS (Elastic Kubernetes Service) adiciona ao Amazon ECS (Elastic Container Service) a capacidade de orquestrar contêineres usando Kubernetes, uma plataforma de código aberto amplamente adotada para automação de implantação, escalonamento e operações de contêineres.

- Distribuição de Carga
    - O serviço responsável por distribuição de carga na AWS é o Elastic Load Balancing (ELB), que distribui automaticamente o tráfego de entrada através de várias instâncias, garantindo alta disponibilidade e resiliência das aplicações.

> **Explicação geral**:  
> O Amazon EKS (Elastic Kubernetes Service) adiciona ao Amazon ECS (Elastic Container Service) a capacidade de orquestrar contêineres usando Kubernetes, uma plataforma de código aberto amplamente utilizada. Enquanto o ECS é nativo da AWS para orquestração de contêineres, o EKS permite a automação de implantação, escalonamento e operações de contêineres com Kubernetes. EKS facilita a migração de workloads Kubernetes para a AWS, aproveitando a padronização e portabilidade do Kubernetes. Ele também oferece integração com o ecossistema de ferramentas Kubernetes, proporcionando flexibilidade adicional para os usuários escolherem entre ECS e EKS conforme suas necessidades específicas.

---

## Pergunta 42

**Seu website vem apresentando indisponibilidades devido a ataques DDoS que tem sofrido com frequência. Quais serviços listados abaixo podem ser utilizados para evitá-los?**

(selecione 2 alternativas)

- AWS GuardDuty
    - O AWS GuardDuty não é especificamente projetado para evitar ataques DDoS, mas sim para fornecer detecção inteligente de ameaças e monitoramento contínuo de atividades maliciosas e comportamentos anômalos em contas AWS. GuardDuty analisa logs de DNS, VPC Flow Logs e CloudTrail para identificar potenciais ameaças, enquanto o AWS Shield é focado diretamente na mitigação e proteção contra ataques DDoS, utilizando técnicas automatizadas e em tempo real para filtrar e limitar tráfego malicioso, garantindo a disponibilidade dos serviços na AWS.

- AWS Detective
    - O AWS Detective não é especificamente projetado para evitar ataques DDoS, mas sim para facilitar a investigação de ameaças e identificar a causa raiz de problemas de segurança. Ele analisa e visualiza dados de log da AWS para ajudar a entender a natureza e o impacto de atividades suspeitas. Enquanto o AWS Shield oferece proteção automatizada e em tempo real contra ataques DDoS, mitigando diretamente o tráfego malicioso e garantindo a disponibilidade dos serviços, o Detective é mais focado em análise pós-incidente e investigação de segurança.

- **✅** AWS CloudFront
    - O Amazon CloudFront evita ataques DDoS usando o AWS Shield, que oferece proteção automática contra ataques de negação de serviço distribuída, e implementa técnicas de mitigação como limitação de taxa e filtragem de tráfego malicioso. Isso protege a infraestrutura e mantém a disponibilidade dos serviços.

- **✅** AWS Shield
    - O AWS Shield evita ataques DDoS ao fornecer proteção contínua com detecção automatizada e mitigação em tempo real, filtrando tráfego malicioso e limitando a taxa de solicitações para manter a disponibilidade dos serviços. Ele integra-se perfeitamente com Amazon CloudFront e outros serviços da AWS para fornecer uma defesa robusta contra DDoS.

- AWS CLI
    - O AWS CLI (Command Line Interface) não é utilizado diretamente para evitar ataques DDoS porque ele é uma ferramenta de linha de comando para gerenciar e interagir com os serviços da AWS, não uma ferramenta de segurança.

> **Explicação geral**:  
> O AWS Shield é um serviço gerenciado que protege contra ataques DDoS, disponível em versões Standard e Advanced. Ele oferece mitigação automática contra os ataques mais comuns e monitoramento contínuo. Integrado com o Amazon CloudFront, Shield absorve e distribui tráfego malicioso, reduzindo o impacto dos ataques. Ele também se integra com serviços como Elastic Load Balancing e Amazon Route 53 para aumentar a resiliência. O Shield Advanced, junto com AWS WAF, permite a criação de regras personalizadas para bloquear tráfego malicioso, proporcionando uma defesa robusta e multi-camadas para garantir a segurança e disponibilidade dos serviços na nuvem.

---

## Pergunta 43

**Ao hospedar 10 instâncias EC2, qual serviço da AWS você deve utilizar para monitorar detalhadamente a utilização da CPU e outros recursos dessas instâncias, garantindo visibilidade e controle sobre o desempenho delas?**

- Amazon CloudTrail
    - O AWS CloudTrail é um serviço que registra e monitora as chamadas de API realizadas na sua conta AWS, fornecendo um histórico detalhado das ações executadas. Isso ajuda a realizar auditorias de segurança, conformidade e solucionar problemas operacionais ao rastrear todas as atividades na sua infraestrutura na nuvem.

- Amazon AMI
    - Uma Amazon Machine Image (AMI) é uma imagem pré-configurada que contém um sistema operacional, configurações do sistema e aplicativos necessários para lançar instâncias no Amazon EC2. Ela permite criar instâncias de forma rápida e consistente, facilitando a replicação e escalabilidade dos recursos na nuvem.

- **✅** Amazon CloudWatch
    - O Amazon CloudWatch é um serviço de monitoramento e observabilidade, fornece dados e insights úteis para monitorar suas instâncias, responder às mudanças de performance de todo o sistema e otimizar a utilização de recursos. O CloudWatch coleta dados operacionais e de monitoramento na forma de logs, métricas e eventos.

- Amazon Log
    - Amazon Log não existe, entretanto, o AWS CloudWatch Logs é um serviço que permite monitorar, armazenar e acessar arquivos de log de instâncias do Amazon EC2, AWS CloudTrail, e outros recursos da AWS. Ele ajuda a solucionar problemas, analisar o desempenho e manter a segurança dos seus aplicativos e infraestruturas na nuvem.

> **Explicação geral**:  
> O Amazon CloudWatch é um serviço de monitoramento e observabilidade que fornece dados e insights úteis para monitorar suas aplicações, responder às mudanças de performance de todo o sistema e otimizar a utilização de recursos. O CloudWatch coleta dados operacionais e de monitoramento na forma de logs, métricas e eventos. Ele permite detectar comportamentos anômalos nos seus ambientes, definir alarmes, visualizar logs e métricas lado a lado, executar ações automatizadas, solucionar problemas e descobrir insights. Com CloudWatch, você pode manter suas aplicações em execução contínua, melhorar a performance e reduzir os custos operacionais através de uma análise detalhada dos recursos utilizados.

---

## Pergunta 44

**No modelo de responsabilidade compartilhada, qual é o papel do cliente?**

- proteger os softwares que executam os serviços de base da nuvem
    - Proteger os softwares de base da infraestrutura geral é responsabilidade da AWS.

- **✅** proteger e configurar instâncias EC2 contra invasões
    - Proteger e configurar instâncias EC2 contra invasões é responsabilidade do cliente no modelo de responsabilidade compartilhada da AWS. É crucial monitorar e gerenciar o tráfego de entrada e saída de dados nas instâncias, garantindo a segurança nas implementações dos recursos computacionais alocados.

- proteger os hardwares que executam os serviços da nuvem
    - Proteger os dispositivos de hardware é responsabilidade da AWS.

- proteger os data centers físicos
    - Proteger os data centers é responsabilidade da AWS.

> **Explicação geral**:  
> Proteger e configurar instâncias EC2 contra invasões é responsabilidade do cliente no modelo de responsabilidade compartilhada da AWS. É essencial que o cliente gerencie cuidadosamente o tráfego de entrada e saída de dados nas instâncias, implementando regras de firewall apropriadas e monitorando acessos. Além disso, configurações de segurança como grupos de segurança, listas de controle de acesso (ACLs) e o uso de chaves SSH devem ser aplicadas para proteger os recursos computacionais alocados.

---

## Pergunta 45

**Seu CEO deseja implementar módulos do SAP para gerenciar todos os departamentos da sua empresa de forma integrada na AWS. Qual é o serviço adequado para prover a infraestrutura necessária para essa finalidade?**

- AWS Device Farm
    - O AWS Device Farm é projetado para permitir testes automatizados de aplicativos móveis em uma ampla variedade de dispositivos reais e virtuais, garantindo a qualidade e a compatibilidade dos aplicativos em várias plataformas e dispositivos móveis. Isso ajuda a identificar e corrigir problemas antes do lançamento, melhorando a experiência do usuário e a confiabilidade dos aplicativos móveis.

- AWS Compute Optimizer
    - O Compute Optimizer da AWS tem como finalidade otimizar a infraestrutura de computação dos clientes, recomendando o dimensionamento adequado das instâncias EC2 para melhorar o desempenho, reduzir custos e otimizar a utilização de recursos de computação na nuvem.

- **✅** AWS Launch Wizard
    - O AWS Launch Wizard simplifica o processo de configuração de ambientes SAP, permitindo que você especifique os requisitos de SAP HANA e outros módulos SAP e então provisiona automaticamente os recursos AWS apropriados.

- AWS Migration Hub
    - O AWS Migration Hub é uma plataforma que ajuda as empresas a planejar, monitorar e gerenciar migrações de cargas de trabalho para a nuvem AWS. Ele fornece uma visão unificada das migrações em andamento, facilitando o acompanhamento do progresso, a resolução de problemas e o gerenciamento eficiente de todo o processo de migração para a nuvem.

> **Explicação geral**:  
> O AWS Launch Wizard oferece uma maneira guiada de dimensionar, configurar e implantar recursos da AWS para aplicações de terceiros, como Microsoft SQL Server Always On e sistemas SAP baseados em HANA, sem a necessidade de identificar e provisionar manualmente recursos individuais da AWS. O serviço apresenta uma estimativa de custo da implantação e permite que você modifique seus recursos a fim de visualizar instantaneamente uma avaliação atualizada dos custos. Depois que você aprova os recursos da AWS, o serviço provisiona e configura automaticamente os recursos selecionados, proporcionando a criação de uma aplicação totalmente funcional e pronta para entrar em produção. O serviço também cria modelos do CloudFormation que podem servir como a linha de base para acelerar implantações posteriores.

---

## Pergunta 46

**Quais são os mecanismos de bancos de dados suportados pelo Amazon RDS?**

- Amazon Aurora, PostgreSQL, MySQL, MariaDB, Oracle Database e DB2.
    - O Amazon RDS não oferece suporte nativo ao IBM Db2 como um dos mecanismos de banco de dados disponíveis.

- **✅** Amazon Aurora, PostgreSQL, MySQL, MariaDB, Oracle Database e SQL Server.
    - O Amazon RDS suporta estes seis principais mecanismos de bancos de dados.

- DynamoDB, Key Spaces, Neptune, Amazon Aurora, PostgreSQL e MySQL.
    - Amazon DynamoDB, Amazon Keyspaces (Cassandra) e Amazon Neptune não são mecanismos suportados pelo Amazon RDS. DynamoDB é um banco NoSQL gerenciado com baixa latência e escalabilidade automática. Keyspaces é compatível com Cassandra e gerencia cargas de trabalho Cassandra. Neptune é um banco de dados gráfico otimizado para consultas de grafos.

- JanusGraph, MongoDB, MariaDB, Oracle Database, MySQL e SQL Server.
    - JanusGraph e MongoDB não são mecanismos suportados pelo Amazon RDS. JanusGraph é um banco de dados gráfico distribuído para consultas de grafos, enquanto MongoDB é um banco de dados NoSQL orientado a documentos, conhecido por sua flexibilidade e escalabilidade.

> **Explicação geral**:  
> O Amazon RDS oferece suporte a seis principais mecanismos de banco de dados: Amazon Aurora, MySQL, MariaDB, PostgreSQL, Oracle e Microsoft SQL Server.
> 
> - Amazon Aurora é compatível com MySQL e PostgreSQL, oferecendo alta performance e disponibilidade.
> - MySQL é popular por sua flexibilidade e facilidade de uso.
> - MariaDB é um fork do MySQL com melhorias em desempenho e segurança.
> - PostgreSQL é conhecido por sua robustez e suporte a características avançadas.
> - Oracle oferece opções de licenciamento BYOL ou LI.
> - Microsoft SQL Server suporta várias edições, desde Express até Enterprise, integrando-se bem com serviços Microsoft.

---

## Pergunta 47

**Qual serviço da AWS permite criar uma esteira de CI/CD englobando demais serviços para controlar todo o workflow de integração e entrega?**

- AWS Step Functions
    - O AWS Step Functions é um serviço de fluxo de trabalho visual que utiliza pouco código, usado para orquestrar serviços da AWS, automatizar processos de negócios e criar aplicações sem servidor. Os fluxos de trabalho gerenciam falhas, novas tentativas, paralelização, integrações de serviços e observabilidade, de modo que os desenvolvedores possam se concentrar na lógica de negócios com maior valor.

- **✅** AWS CodePipeline
    - O AWS CodePipeline é um serviço gerenciado de entrega contínua que ajuda a automatizar pipelines de liberação para oferecer atualizações rápidas e confiáveis de aplicativos e infraestruturas. O CodePipeline automatiza as fases de compilação, teste e implantação do processo de liberação sempre que ocorre uma mudança no código, de acordo com o modelo de liberação que você definiu.

- AWS Workflow
    - O AWS Workflow não é um serviço ofertado pela AWS.

- AWS CodeCommit
    - O AWS CodeCommit é um serviço de controle de origem gerenciado seguro e altamente dimensionável que hospeda repositórios privados do Git. Ele torna mais fácil para as equipes colaborarem com segurança no código com contribuições criptografadas em trânsito e em repouso.

> **Explicação geral**:  
> O AWS CodePipeline é um serviço de integração e entrega contínuas (CI/CD) que automatiza o processo de construção, teste e implantação de aplicações. Ele se integra com o CodeCommit para monitorar repositórios e detectar mudanças no código, iniciando automaticamente o pipeline. Com o CodeBuild, CodePipeline compila e testa o código, garantindo que apenas versões estáveis avancem. Após a compilação, CodePipeline utiliza o CodeDeploy para automatizar a implantação em diversas instâncias de computação, como EC2, Lambda ou servidores on-premises. Essas integrações permitem um fluxo de trabalho contínuo e eficiente, facilitando a entrega rápida e confiável de novas funcionalidades e correções.

---

## Pergunta 48

**Quais ferramentas específicas da AWS adaptam as orientações do AWS Well-Architected Framework para domínios como machine learning (ML), análise de dados, tecnologia sem servidor, HPC, IoT, SAP, mídia de streaming, indústria de jogos, redes híbridas e serviços financeiros?**

- 6 Rs Lenses (Lentes)
    - Os 6 Rs são estratégias de migração para a nuvem na AWS: Rehost (migrar sem alterações), Replatform (pequenas otimizações), Repurchase (substituir por SaaS), Refactor/Re-architect (reestruturar para nuvem), Retire (descontinuar aplicações desnecessárias) e Retain (manter no ambiente atual ou decidir posteriormente).

- AWS Well-Architected Pillar (Pilares)
    - Os pilares do AWS Well-Architected Framework fornecem princípios gerais aplicáveis a todas as arquiteturas na AWS, enquanto os Well-Architected Lenses oferecem orientações específicas para domínios industriais e tecnológicos.

- **✅** AWS Well-Architected Lenses (Lentes)
    - Os AWS Well-Architected Lenses são extensões do AWS Well-Architected Framework que fornecem orientações específicas para diferentes indústrias e tecnologias, garantindo práticas recomendadas para eficiência, segurança e escalabilidade.

- 6 Rs Pillar (Pilares)
    - Os 6 Rs são estratégias de migração para a nuvem na AWS: Rehost (migrar sem alterações), Replatform (pequenas otimizações), Repurchase (substituir por SaaS), Refactor/Re-architect (reestruturar para nuvem), Retire (descontinuar aplicações desnecessárias) e Retain (manter no ambiente atual ou decidir posteriormente).

> **Explicação geral**:  
> Os AWS Well-Architected Lenses são extensões do AWS Well-Architected Framework que fornecem práticas recomendadas e orientações específicas para diferentes indústrias e tecnologias. Cada lens oferece insights detalhados sobre como aplicar os princípios do framework a cenários específicos, como machine learning (ML), análise de dados, tecnologia sem servidor, HPC, IoT, SAP, mídia de streaming, indústria de jogos, redes híbridas e serviços financeiros. Esses lenses ajudam as organizações a construir arquiteturas otimizadas para suas necessidades particulares, garantindo eficiência, segurança, escalabilidade e conformidade com as melhores práticas da AWS.

---

## Pergunta 49

**Ao configurar manualmente um banco de dados em uma instância EC2, qual serviço de armazenamento durável e de alta performance deve ser utilizado para armazenar os arquivos de instalação e os dados do banco de dados, garantindo disponibilidade e persistência dos dados?**

- Aurora
    - O Amazon Aurora não é ideal para a instalação manual de um banco de dados em uma instância EC2 porque é um serviço de banco de dados relacional gerenciado pela AWS.

- DynamoDB
    - O Amazon DynamoDB não é adequado para a instalação manual de um banco de dados em uma instância EC2 porque é um banco de dados NoSQL gerenciado pela AWS, otimizado para armazenamento e recuperação de dados em formato de chave-valor e documentos.

- RDS
    - Amazon RDS não é ideal para instalação manual de um banco de dados em uma instância EC2 porque é um serviço gerenciado pela AWS que automatiza tarefas administrativas.

- **✅** EBS
    - O Amazon EBS é ideal para armazenar dados e arquivos de instalação ao configurar manualmente um banco de dados em uma instância EC2 porque oferece durabilidade e persistência dos dados, alto desempenho e flexibilidade na configuração. EBS também permite backups e recuperação de dados via snapshots, proporcionando controle total sobre o armazenamento.

> **Explicação geral**:  
> O Amazon Elastic Block Store (EBS) é um serviço de armazenamento em bloco que fornece volumes duráveis e de alta performance para instâncias EC2, funcionando como discos virtuais. EBS permite armazenamento persistente e seguro, ideal para bancos de dados e aplicações que requerem acesso a armazenamento de baixa latência. Ele oferece diferentes tipos de volumes para várias necessidades de desempenho e custo. Os volumes EBS são replicados automaticamente dentro da zona de disponibilidade, garantindo resiliência contra falhas de hardware. Além disso, você pode criar snapshots para backup e recuperação de dados. Os volumes EBS podem ser facilmente anexados e desanexados de instâncias EC2, proporcionando flexibilidade na gestão de armazenamento.

---

## Pergunta 50

**Quais são as considerações importantes sobre a utilização de endereços IPv4 públicos na AWS?**

- São limitados a 10 por conta por região
    - Endereços IPv4 públicos na AWS são limitados a 5 por conta por região, não a 10.

- São limitados a 5 por conta por zona de disponibilidade
    - Endereços IPv4 públicos na AWS são limitados a 5 por conta por região, não por zona de disponibilidade.

- **✅** São limitados a 5 por conta por região
    - Endereços IPv4 públicos na AWS são limitados a 5 por conta por região para incentivar o uso eficiente dos recursos de IP, evitando a exaustão dos endereços IPv4 disponíveis globalmente. Essa limitação também ajuda a gerenciar os endereços de forma justa entre os usuários da AWS.

- São limitados a 10 por conta por zona de disponibilidade
    - Endereços IPv4 públicos na AWS são limitados a 5 por conta por região, não a 10 por zona de disponibilidade.

> **Explicação geral**:  
> A criação de endereços IPv4 públicos na AWS é inicialmente limitada a 5 por conta por região. Esta limitação incentiva o uso eficiente dos endereços IPv4 e ajuda a evitar a exaustão global desses recursos limitados. Cada endereço IPv4 público é um recurso valioso, e essa restrição garante uma alocação justa entre todos os usuários da AWS.
> 
> Se uma organização precisar de mais endereços IPv4 públicos, ela pode solicitar um aumento desse limite por meio de um pedido de suporte à AWS. Esse processo geralmente envolve uma análise das necessidades e justificativas para o aumento, garantindo que os recursos adicionais sejam usados de maneira eficiente e responsável.
> 
> Além disso, é importante considerar a adoção de endereços IPv6, que são praticamente ilimitados e podem ajudar a mitigar as restrições de IPv4. A AWS oferece suporte robusto para IPv6, permitindo uma transição suave e garantindo a continuidade das operações à medida que os endereços IPv4 se tornam mais escassos.

---

## Pergunta 51

**Qual é o serviço de Pub/Sub utilizado para desacoplar sistemas, filtrar e enviar mensagens para diversos serviços como SQS, E-mail, Kinesis, entre outros?**

- Amazon RDS
    - O Amazon Relational Database Service (Amazon RDS) facilita a configuração, a operação e a escalabilidade de bancos de dados relacionais na nuvem. O serviço oferece capacidade econômica e redimensionável e automatiza tarefas demoradas de administração, como provisionamento de hardware, configuração de bancos de dados, aplicação de patches e backups.

- **✅** Amazon SNS
    - SNS tem diversos usos possíveis na arquitetura de sistemas, a principal característica é essa função Pub/Sub que traz diversas possibilidades para o desenvolvimento das aplicações que precisam gerar mensagens ou eventos para outras consumirem e serem integradas de forma rápida através da leitura dos tópicos.

- Amazon EC2
    - O Amazon Elastic Compute Cloud (Amazon EC2) é um serviço Web que disponibiliza capacidade computacional segura e redimensionável na nuvem. Ele foi projetado para facilitar a computação em nuvem na escala da web para os desenvolvedores. O Amazon EC2 oferece a maior e mais abrangente plataforma de computação com a possibilidade de escolha de processador, armazenamento, rede, sistema operacional e modelo de compra.

- Amazon Topic
    - Este serviço não existe.

> **Explicação geral**:  
> O Amazon SNS (Simple Notification Service) é um serviço de mensagens gerenciado que suporta o modelo de publicação/assinatura (pub/sub). Nesse modelo, publicadores enviam mensagens que são recebidas por múltiplos assinantes, permitindo o desacoplamento dos sistemas e facilitando a manutenção e escalabilidade. SNS é altamente escalável, entregando milhões de mensagens por dia em tempo real. Ele oferece flexibilidade com suporte a diversos protocolos (HTTP/HTTPS, e-mail, SMS, Amazon SQS) e garante alta disponibilidade com integração ao Amazon CloudWatch. Essa arquitetura permite a rápida integração de novos sistemas e serviços, tornando a comunicação eficiente e robusta.

---

## Pergunta 52

**Sua empresa deseja migrar todos os seus aplicativos do ambiente on premises para a AWS. Qual é o principal benefício de utilizar o AWS Migration Hub neste contexto?**

- Criação automática de políticas de segurança personalizadas.
    - O Migration Hub não cria automaticamente políticas de segurança.

- Integração nativa com todos os principais sistemas operacionais.
    - O AWS Migration Hub não se concentra na integração com sistemas operacionais.

- **✅** Centralização de informações e visibilidade consolidada em tempo real das migrações.
    - O AWS Migration Hub é uma ferramenta da Amazon Web Services projetada para simplificar a gestão de migrações de aplicativos para a nuvem. Sua função principal é oferecer uma visão centralizada e em tempo real de todo o processo de migração, permitindo que as empresas coordenem, acompanhem e gerenciem eficientemente várias migrações em diferentes ambientes.

- Automatização completa de todo o processo de migração.
    - O AWS Migration Hub simplifica a gestão, mas não automatiza completamente todo o processo de migração.

> **Explicação geral**:  
> Os benefícios do AWS Migration Hub incluem economia de tempo e recursos, uma vez que elimina a necessidade de usar várias ferramentas para monitorar migrações. Além disso, oferece visibilidade aprofundada, o que facilita a identificação de possíveis problemas e a tomada de decisões informadas.
> 
> Casos de uso comuns do Migration Hub incluem migrações de aplicativos legados para a nuvem, consolidação de centros de dados, migração de cargas de trabalho para a nuvem AWS e aprimoramento da eficiência na gestão de migrações em ambientes complexos. Em resumo, o AWS Migration Hub simplifica e otimiza o processo de migração, tornando-o uma ferramenta valiosa para organizações que buscam adotar a computação em nuvem de forma eficaz.

---

## Pergunta 53

**Qual é o termo usado para descrever a capacidade de adicionar ou remover automaticamente máquinas para executar aplicações conforme a demanda, garantindo eficiência e economia de recursos?**

- Performance
    - Performance refere-se à eficiência e rapidez com que um sistema ou aplicação executa suas tarefas, incluindo processamento de dados, tempo de resposta e utilização de recursos. Na AWS, otimizar a performance envolve escolhas arquiteturais e serviços que garantam alta velocidade e eficiência operacional.

- Disponibilidade
    - Disponibilidade refere-se à capacidade de um sistema, serviço ou recurso estar operacional e acessível quando necessário. Na AWS, isso implica garantir que os recursos estejam continuamente acessíveis e funcionais, minimizando o tempo de inatividade através de redundâncias e mecanismos de recuperação.

- **✅** Elasticidade
    - A capacidade de adicionar ou remover automaticamente máquinas para executar aplicações conforme a demanda é denominada elasticidade. Isso garante eficiência operacional e economia de recursos ao ajustar a infraestrutura conforme as necessidades variam.

- Desacoplamento
    - Desacoplamento refere-se à prática de projetar sistemas ou componentes de software de forma que eles sejam independentes uns dos outros, facilitando a manutenção, escalabilidade e evolução. Na AWS, isso é alcançado usando serviços como SQS e SNS para permitir comunicação assíncrona entre componentes.

> **Explicação geral**:  
> A elasticidade na AWS envolve vários serviços que permitem ajustar automaticamente a quantidade de recursos conforme a demanda. Amazon EC2 Auto Scaling ajusta o número de instâncias EC2 em resposta a mudanças na carga. AWS Elastic Load Balancing (ELB) distribui automaticamente o tráfego de entrada entre várias instâncias EC2. AWS Lambda executa código em resposta a eventos e escala automaticamente sem necessidade de servidores. Amazon RDS Auto Scaling ajusta a capacidade de armazenamento e de leitura para bancos de dados. Amazon DynamoDB Auto Scaling ajusta a capacidade de leitura e gravação conforme a demanda, garantindo performance e eficiência de custo. Esses serviços trabalham juntos para proporcionar uma operação eficiente e econômica, adaptando-se às necessidades em tempo real.

---

## Pergunta 54

**Qual serviço da AWS é ideal para armazenar grandes volumes de dados não estruturados, como arquivos de dados, filmes e música, em um formato de objeto, oferecendo escalabilidade, durabilidade e acessibilidade?**

- Amazon EC2
    - O Amazon Elastic Compute Cloud (Amazon EC2) é um serviço Web que disponibiliza capacidade computacional segura e redimensionável na nuvem. Ele foi projetado para facilitar a computação em nuvem na escala da web.

- Amazon Elastic Cache
    - Com o Amazon ElastiCache, você pode configurar, executar e escalar repositórios de dados na memória compatíveis com código aberto na nuvem, melhorando a performance de aplicações com alta taxa de transferência e baixa latência. É ideal para casos de uso em tempo real, como armazenamento em cache, sessões, jogos, serviços geoespaciais, análises em tempo real e filas.

- Amazon DynamoDb
    - O Amazon DynamoDB é um banco de dados de valores-chave e documentos que oferece desempenho em milissegundos de um dígito em qualquer escala.

- **✅** Amazon S3
    - O serviço da AWS ideal para armazenar grandes volumes de dados não estruturados, como arquivos de dados, filmes e música, em formato de objeto, oferecendo escalabilidade, durabilidade e acessibilidade, é o Amazon S3 (Simple Storage Service).

> **Explicação geral**:  
> O Amazon S3 (Simple Storage Service) é o serviço da AWS ideal para armazenar grandes volumes de dados não estruturados, como arquivos de dados, filmes e música, em formato de objeto. Ele oferece escalabilidade praticamente ilimitada, permitindo que você armazene qualquer quantidade de dados e acesse-os de qualquer lugar. S3 garante durabilidade de 99,999999999% (11 noves) dos objetos armazenados e alta disponibilidade. O serviço também fornece opções de armazenamento com diferentes classes, como S3 Standard, S3 Intelligent-Tiering e S3 Glacier, para otimização de custos conforme a frequência de acesso aos dados. Além disso, S3 suporta controle de acesso granular, integração com outras ferramentas AWS para processamento e análise, e recursos de segurança avançados, como criptografia de dados em trânsito e em repouso. Essas características fazem do Amazon S3 uma solução robusta e versátil para armazenamento de dados.

---

## Pergunta 55

**Qual é o serviço gerenciado de proteção contra DDoS (Negação de serviço distribuída) que protege os aplicativos executados na AWS?**

- Amazon Macie
    - O Amazon Macie é um serviço de segurança e privacidade de dados totalmente gerenciado que usa machine learning e correspondência de padrões para descobrir e proteger seus dados confidenciais na AWS.

- Amazon Inspector
    - O Amazon Inspector é um serviço de avaliação de segurança automático que ajuda a melhorar a segurança e a conformidade dos aplicativos implantados na AWS. O Amazon Inspector avalia automaticamente aplicativos em busca de exposições, vulnerabilidades ou discrepâncias em relação às melhores práticas.

- Amazon GuardDuty
    - O Amazon GuardDuty é um serviço de detecção de ameaças que monitora continuamente atividades mal-intencionadas e comportamentos não autorizados para proteger suas contas, cargas de trabalho e dados da AWS armazenados no Amazon S3.

- **✅** Amazon Shield
    - O AWS Shield é um serviço gerenciado de proteção contra DDoS (Negação de serviço distribuída) que protege os aplicativos executados na AWS. O AWS Shield oferece de detecção e mitigações em linha automáticas e sempre ativas que minimizam o tempo de inatividade e a latência dos aplicativos, fornecendo proteção contra DDoS sem necessidade de envolver o AWS Support.

> **Explicação geral**:  
> O AWS Shield é um serviço gerenciado que protege aplicações na AWS contra ataques DDoS (Negação de Serviço Distribuída). Ele fornece detecção e mitigação automáticas e sempre ativas, minimizando o tempo de inatividade e a latência dos aplicativos. Isso permite obter proteção robusta sem envolver o suporte da AWS. Shield integra-se com serviços como Amazon CloudFront para proteger conteúdo distribuído, Elastic Load Balancing (ELB) para defender instâncias EC2, Amazon Route 53 para proteger DNS, e AWS WAF para proteção adicional na camada de aplicação. Essas integrações garantem uma abordagem de segurança em profundidade, protegendo as aplicações contra uma ampla gama de ataques DDoS.

---

## Pergunta 56

**No modelo de responsabilidade compartilhada, qual dos itens abaixo não é papel da AWS?**

- **✅** Gerenciamento de permissão de acesso a dados de aplicativos dos clientes.
    - Gerenciamento de permissão de acesso a dados de aplicativos dos clientes é de responsabilidade única e exclusivamente do cliente. A AWS dispõe dos serviços para esse gerenciamento, entretanto, quem faz a manutenção dos usuários é o cliente.

- Conhecimentos e treinamentos
    - Conhecimentos e treinamentos: a AWS treina funcionários da AWS, mas o cliente deve treinar seus próprios funcionários.

- Gerenciamento de configuração
    - Gerenciamento de configuração: a AWS mantém a configuração dos dispositivos de infraestrutura, mas o cliente é responsável pela configuração dos seus próprios bancos de dados, aplicativos e sistemas operacionais convidados.

- Gerenciamento de patches
    - Gerenciamento de patches: a AWS é responsável pela aplicação de patches e pela correção de falhas na infraestrutura, mas os clientes são responsáveis pela aplicação de patches em seu SO convidado e nos seus aplicativos.

> **Explicação geral**:  
> O gerenciamento de permissões de acesso a dados de aplicativos dos clientes é responsabilidade exclusiva do cliente no modelo de responsabilidade compartilhada da AWS. Embora a AWS forneça serviços como AWS Identity and Access Management (IAM) e AWS Organizations para ajudar no gerenciamento de permissões, a configuração, manutenção e monitoramento dos acessos são de responsabilidade do cliente. O cliente deve criar políticas de IAM para controlar quem pode acessar os recursos, implementar a autenticação multifator (MFA) para segurança adicional, e realizar auditorias regulares usando serviços como AWS CloudTrail para rastrear atividades e detectar possíveis violações. Além disso, a configuração de grupos de segurança e listas de controle de acesso (ACLs) é crucial para gerenciar o tráfego de rede de maneira segura.

---

## Pergunta 57

**Qual serviço da AWS pode ser utilizado se você deseja hospedar aplicações web de várias camadas e estabelecer o acesso e as restrições de segurança entre seus servidores web, aplicações e bancos de dados?**

- NACL
    - NACL / ACL - Network Access Control List é uma espécie de firewall opcional para controlar a entrada ou saída de dados de uma Sub Rede dentro de uma VPC - Virtual Private Cloud.

- VPN
    - VPN - As soluções do AWS Virtual Private Network estabelecem conexões seguras entre redes locais, escritórios remotos, dispositivos de clientes e a rede global da AWS.

- **✅** VPC
    - O Amazon Virtual Private Cloud (Amazon VPC) oferece controle total sobre seu ambiente de redes virtual, incluindo posicionamento de recursos, conectividade e segurança. O Amazon VPC facilita a personalização da configuração de rede da VPC. Você pode criar uma sub-rede voltada ao público para seus servidores Web que têm acesso à Internet. Também é possível colocar seus sistemas backend, como bancos de dados ou servidores de aplicações, em uma sub-rede privada, sem acesso à Internet.

- Security Group
    - Security Group é um serviço para controlar o tráfego de dados numa camada lógica da sua rede. Camada de servidores de aplicação, camada de servidores de dados, etc.

> **Explicação geral**:  
> A Amazon VPC (Virtual Private Cloud) permite criar um ambiente de rede isolado na nuvem da AWS para hospedar aplicações em uma arquitetura de três camadas, incluindo front-end, back-end e banco de dados. Para isso, você pode criar sub-redes separadas dentro da VPC:
> 
> - Camada Front-end: Hospede a interface de usuário em uma sub-rede pública, utilizando instâncias EC2 e balanceadores de carga (ELB) para distribuir o tráfego de entrada. Essa sub-rede pública tem acesso à internet para atender aos usuários finais.
> - Camada Back-end: Coloque a lógica de aplicação em uma sub-rede privada, protegendo os servidores de aplicação do acesso direto à internet. Essa sub-rede pode se comunicar com a sub-rede front-end, mas não é acessível diretamente da internet, aumentando a segurança.
> - Camada de Banco de Dados: Armazene os dados em uma sub-rede privada separada, utilizando serviços como Amazon RDS ou instâncias EC2 configuradas com bancos de dados como MySQL ou PostgreSQL. Esta camada só deve ser acessível pela camada de aplicação, garantindo que os dados sejam protegidos de acessos externos.
> 
> Essas sub-redes são conectadas e gerenciadas através de tabelas de roteamento e gateways, como o Internet Gateway para acesso à internet e o NAT Gateway para permitir que instâncias em sub-redes privadas façam atualizações e conexões seguras para fora. Esta configuração proporciona alta segurança, escalabilidade e separação de responsabilidades entre as diferentes camadas da aplicação.

---

## Pergunta 58

**Qual plano de suporte é recomendado se você tem cargas de trabalho empresariais e/ou de missão crítica na AWS?**

- Business
    - O Business é recomendado para quem tem workloads essenciais à produção ou aos negócios na AWS.

- Developer
    - O Developer é recomendado para quem está experimentando ou testando a AWS.

- Basic
    - O Basic não possui uma recomendação explicita no site da AWS.

- **✅** Enterprise
    - Apenas o Enterprise oferece suporte para aplicações de missão crítica. O Enterprise on-Ramp também é recomendado para quem tem workloads essenciais à produção ou aos negócios na AWS.

> **Explicação geral**:  
> A AWS oferece cinco planos de suporte:
> 
> - Basic: Incluído gratuitamente para todos os clientes AWS, oferecendo acesso 24/7 a atendimento ao cliente, documentação e AWS Trusted Advisor. Não possui uma recomendação explicita no site da AWS.
> - Developer: Recomendado para desenvolvimento e testes, com suporte técnico durante horário comercial e tempos de resposta de até 12 horas para problemas gerais.
> - Business: Ideal para ambientes de produção, fornecendo suporte 24/7, tempos de resposta de até 1 hora para problemas críticos e acesso completo ao AWS Trusted Advisor.
> - Enterprise On-Ramp: Destinado a empresas em crescimento com cargas de trabalho críticas, oferece suporte 24/7, tempos de resposta de até 30 minutos para problemas críticos e acesso a um gerente de conta técnica (TAM).
> - Enterprise: Para operações empresariais com missões críticas, oferecendo suporte 24/7, tempos de resposta de até 15 minutos para problemas críticos, TAM dedicado, análises proativas e workshops de arquitetura.

---

## Pergunta 59

**Qual é o serviço que tem uma relação preço-performance até 3x melhor do que outros data warehouses na nuvem, e onde a vantagem dessa relação preço-performance aumenta à medida que seu data warehouse cresce de gigabytes para hexabytes?**

- **✅** Amazon Redshift
    - O serviço da AWS que oferece uma relação preço-performance até 3x melhor do que outros data warehouses na nuvem é o Amazon Redshift.

- Amazon QuickSight
    - O Amazon QuickSight é o serviço utilizado para gerar Dashboards e gerar insights para tomadas de decisão.

- Amazon RDS
    - O RDS - Relational Database Service é o serviço utilizado para a implementação de diversos bancos de dados relacionais na AWS.

- Amazon EMR
    - O Amazon EMR é o serviço gerenciado da AWS para implementar frameworks de Big Data, como Apache Hadoop e Spark, permitindo processamento e análise de grandes volumes de dados de forma escalável e econômica.

> **Explicação geral**:  
> O Amazon Redshift é um serviço de data warehouse totalmente gerenciado da AWS, projetado para análise rápida e eficiente de grandes volumes de dados. Ele armazena dados em colunas, utiliza compressão avançada e distribui a carga de trabalho entre nós de computação para processamento paralelo. Essas técnicas resultam em consultas analíticas muito rápidas. Redshift também escala automaticamente capacidade de computação e armazenamento conforme necessário, otimizando custos e performance. Além disso, implementa caching inteligente para acelerar consultas repetitivas. Essas características permitem que Redshift ofereça uma relação preço-performance até 3x melhor do que outros data warehouses na nuvem, especialmente à medida que o volume de dados cresce.

---

## Pergunta 60

**Qual é o serviço que permite que os desenvolvedores adicionem, diretamente ou usando o AWS SDK, funcionalidades de criptografia ou assinatura digital ao código de aplicativos?**

- CodeCommit
    - O AWS CodeCommit é um serviço de controle de origem gerenciado seguro e altamente dimensionável que hospeda repositórios privados do Git. Ele torna mais fácil para as equipes colaborarem com segurança no código com contribuições criptografadas em trânsito e em repouso. Com o CodeCommit, você não precisa gerenciar seu próprio sistema de controle de origem nem se preocupar com o dimensionamento da sua infraestrutura.

- Certificate Manager
    - O AWS Certificate Manager é um serviço que permite provisionar, gerenciar e implantar facilmente certificados Secure Sockets Layer (SSL)/Transport Layer Security (TLS) para uso com os serviços da AWS e os recursos internos conectados. Os certificados SSL/TLS são usados para proteger comunicações de rede e estabelecer a identidade de sites na Internet e de recursos em redes privadas. O AWS Certificate Manager elimina processos manuais demorados como compra, upload e renovação de certificados SSL/TLS.

- CodePipeline
    - O AWS CodePipeline é um serviço gerenciado de entrega contínua que ajuda a automatizar pipelines de liberação para oferecer atualizações rápidas e confiáveis de aplicativos e infraestruturas. O CodePipeline automatiza as fases de compilação, teste e implantação do processo de liberação sempre que ocorre uma mudança no código, de acordo com o modelo de liberação que você define.

- **✅** KMS
    - O AWS Key Management Service (KMS) facilita a criação e o gerenciamento de chaves criptográficas e o controle do seu uso em uma ampla variedade de serviços da AWS e nas suas aplicações. É um serviço seguro e resiliente que usa módulos de segurança de hardware validados ou em processo de validação pelo FIPS 140-2 para proteger suas chaves.

> **Explicação geral**:  
> O AWS Key Management Service (KMS) facilita a criação e o gerenciamento de chaves criptográficas, além de controlar seu uso em diversos serviços da AWS e aplicações dos clientes. É um serviço seguro e resiliente que utiliza módulos de segurança de hardware (HSMs) validados ou em processo de validação pelo FIPS 140-2 para proteger suas chaves. O AWS KMS integra-se com serviços como S3, EBS e RDS para criptografia de dados, permitindo gerenciamento centralizado de chaves. Ele oferece recursos como rotação automática de chaves, políticas de controle de acesso detalhadas e logs de auditoria com AWS CloudTrail, garantindo segurança e conformidade robustas.

---

## Pergunta 61

**Sua empresa é dividida em 6 departamentos e cada um deles tem uma conta própria na AWS. Qual serviço abaixo permite a consolidação dos custos e a integração de outros serviços?**

- AWS Cost Calculator
    - O AWS Cost Calculator não é um serviço existente na AWS.

- AWS Budgets
    - O Budgets da AWS permite que você defina orçamentos personalizados que enviam alertas quando o uso ou os custos excedem (ou tendem a exceder) o valor orçado.

- **✅** AWS Organizations
    - O AWS Organizations te ajuda a gerenciar e controlar seu ambiente de maneira centralizada à medida que os negócios e seus recursos da AWS expandem. Você pode criar novas contas da AWS e alocar recursos, agrupar contas para organizar seus fluxos de trabalho, aplicar políticas a contas ou grupos para governança e simplificar o faturamento usando um único método de pagamento para todas as suas contas.

- AWS Cost Explorer
    - O AWS Cost Explorer tem uma interface fácil de usar que permite visualizar, entender e gerenciar os custos e o uso da AWS ao longo do tempo.

> **Explicação geral**:  
> O AWS Organizations ajuda a gerenciar e controlar seu ambiente AWS de maneira centralizada à medida que os negócios e recursos expandem. Usando o AWS Organizations, você pode criar novas contas AWS e alocar recursos de forma eficiente. Ele permite agrupar contas para organizar fluxos de trabalho e aplicar políticas centralizadas para governança, como restrições de serviço e permissões. Além disso, o AWS Organizations simplifica o faturamento consolidando várias contas sob um único método de pagamento. Exemplos de uso incluem grandes empresas que desejam segregar contas por departamento, aplicar políticas de segurança de maneira uniforme e gerenciar orçamentos de forma consolidada.

---

## Pergunta 62

**Por que na AWS temos mais economia do que em data centers tradicionais, quando executamos aplicações que têm necessidades computacionais variadas, ao longo de um determinado período?**

- Porque a aplicação pode ser projetada em mais de uma zona de disponibilidade para atender essa variação
    - Projetar a aplicação em mais de uma zona de disponibilidade aumenta a resiliência da aplicação, não reduz custos.

- Porque o custo do hardware da AWS é muito mais barato.
    - O custo do hardware para a AWS não é de conhecimento público e não é a única justificativa para economizar com cargas variadas. Além do hardware, variáveis como segurança, eletricidade, refrigeração e manutenção são consideradas para manter um data center eficiente e seguro. Esses fatores influenciam significativamente os custos operacionais totais.

- Porque os custos de processamento são compartilhados com os demais clientes.
    - O custo do processamento não é compartilhado com os demais clientes, a infraestrutura física sim.

- **✅** Porque podemos utilizar os recursos sob-demanda e pagarmos somente pelo uso.
    - Você paga somente pelo uso, sem a necessidade de aquisição de hardware e data centers para suportar períodos de pico de processamento. Numa solução on-premises, onde o data center é particular, seria necessário comprar todas as máquinas necessárias para suportar os períodos de pico e deixá-las ociosas em momentos de baixa utilização.

> **Explicação geral**:  
> Com cargas variadas, pagar sob demanda na AWS melhora os custos de utilização das instâncias e processamento. Você paga somente pelo uso, sem necessidade de adquirir hardware ou manter data centers para suportar picos de processamento. Em uma solução on-premises, seria necessário comprar todas as máquinas para suportar picos, resultando em ociosidade durante períodos de baixa utilização. Isso não só aumenta os custos iniciais, mas também os gastos contínuos com manutenção, eletricidade e refrigeração, tornando a abordagem da AWS mais econômica e flexível para diferentes cargas de trabalho.

---

## Pergunta 63

**O Amazon DocumentDB é um serviço que pode ser utilizado em qual dos cenários abaixo?**

- **✅** Armazenamento de dados baseado em documentos JSON.
    - O Amazon DocumentDB é um serviço de banco de dados escalável, altamente durável e totalmente gerenciado para operar workloads do MongoDB de missão crítica. Como um tipo de banco de dados NoSQL, o Amazon DocumentDB facilita a inserção, a consulta, a indexação e a execução de agregações em dados JSON.

- Armazenamento de dados relacionais com forte consistência de dados.
    - Essa é a função de serviços como o RDS.

- Armazenamento de dados em grafos para redes sociais
    - Essa é a função do serviço Neptune.

- Armazenamento de dados em documentos e execução de MapReduce
    - Essa é a função da plataforma EMR.

> **Explicação geral**:  
> O Amazon DocumentDB é um serviço de banco de dados NoSQL escalável, altamente durável e totalmente gerenciado, projetado para operar workloads do MongoDB de missão crítica. Ele facilita a inserção, consulta, indexação e execução de agregações em dados JSON, proporcionando uma experiência semelhante ao MongoDB. DocumentDB oferece escalabilidade automática, backups contínuos e recuperação pontual, além de alta disponibilidade com réplicas em múltiplas zonas de disponibilidade (AZs). Esse serviço é ideal para aplicações que exigem baixa latência e alta performance, tornando o gerenciamento de dados JSON eficiente e seguro na AWS.

---

## Pergunta 64

**Sua empresa precisa realizar backups de diversos serviços de sua infraestrutura virtual e do seu ambiente on-premises. Qual é o serviço que, através da CLI, APIs e Console, permite automatizar e consolidar tarefas de backup e remove a necessidade de criar scripts personalizados e processos manuais?**

- **✅** AWS Backup
    - O serviço que permite automatizar e consolidar tarefas de backup para sua infraestrutura virtual e ambiente on-premises, através da CLI, APIs e Console, é o AWS Backup. Ele remove a necessidade de criar scripts personalizados e processos manuais, facilitando a gestão centralizada de backups.

- Amazon EBS
    - O EBS fornece volumes para persistência de dados para instâncias EC2.

- AWS Storage Gateway
    - O Storage Gateway permite armazenar volumes do ambiente on-premises na AWS.

- Amazon S3
    - O S3 armazena os snapshots dos backups.

> **Explicação geral**:  
> AWS Backup é um serviço totalmente gerenciado que facilita a centralização e a automação da proteção de dados na nuvem e no local. Usando este serviço, você pode configurar políticas de backup e monitorar a atividade para seus recursos de AWS em um só lugar. O ponto principal aqui é o gerenciamento e automação. Os outros serviços podem estar envolvidos no processo, mas não têm esses recursos.

---

## Pergunta 65

**Sua empresa precisa alocar temporariamente um time de 300 colaboradores terceirizados para a conclusão de um grande projeto. De que maneira o AWS Workspaces Web pode auxiliá-la?**

- Fornecendo um serviço para criação de ambientes de desenvolvimento.
    - Ambientes de desenvolvimento podem ser provisionados com o CloudFormation, Elastic Beanstalk para implementar serviços computacionais com o EC2, ECS e Lambdas, voltados para esse tipo de ambiente.

- Fornecendo um serviço para hospedagem de bancos de dados.
    - Os bancos de dados podem ser provisionados com o RDS, DynamoDB, dependendo do tipo de estrutura que precisar.

- **✅** Fornecendo um serviço de desktop na nuvem com acesso a aplicativos e dados a partir de um navegador web.
    - O AWS Workspaces Web é um serviço de desktop virtual que permite às organizações criar ambientes de trabalho na nuvem, oferecendo acesso remoto seguro a desktops e aplicativos através de qualquer dispositivo com um navegador web.

- Fornecendo uma plataforma de criação de sites e aplicativos web.
    - A criação de sites pode ser realizada com as SDKs e IDEs do Cloud9.

> **Explicação geral**:  
> O AWS Workspaces Web é um serviço de desktop virtual da Amazon Web Services (AWS) que permite às organizações criar ambientes de trabalho na nuvem. Ele oferece acesso remoto seguro a desktops e aplicativos a partir de qualquer dispositivo com um navegador web, possibilitando que os usuários acessem seus ambientes de trabalho e dados de qualquer lugar, promovendo mobilidade e flexibilidade. O Workspaces Web simplifica a administração de desktops, facilitando o provisionamento, gerenciamento e escalabilidade dos ambientes de trabalho. Essa solução é valiosa para empresas que precisam fornecer acesso remoto a aplicativos e desktops de forma segura e eficiente, eliminando a necessidade de comprar máquinas físicas para uso temporário.

---