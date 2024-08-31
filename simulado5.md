## Pergunta 1

**Numa implementação na AWS você precisa definir um serviço para hospedar seus servidores de aplicação e de bancos de dados dentro de uma rede virtual isolada. Qual é o serviço responsável por isso?**

- AWS Trusted Advisor
    - O AWS Trusted Advisor faz recomendações que ajudam você a seguir as melhores práticas da AWS. O Trusted Advisor avalia a sua conta através de verificações. Essas verificações identificam formas de otimizar sua infraestrutura da AWS, aumentar a segurança e o desempenho, reduzir os custos gerais e monitorar as cotas do serviço.

- AWS ASG
    - O Auto Scaling Group (ASG) gerencia automaticamente a escala de instâncias EC2 para atender à demanda de carga de trabalho. Ele ajusta a quantidade de instâncias em execução com base em políticas de escalonamento predefinidas, garantindo alta disponibilidade e desempenho.

- **✅** AWS VPC
    - Para hospedar servidores de aplicação e bancos de dados dentro de uma rede virtual isolada na AWS, você deve usar o Amazon Virtual Private Cloud (VPC). O VPC permite criar uma rede privada na nuvem, onde você pode definir sub-redes, tabelas de roteamento, gateways e configurações de segurança para isolar e gerenciar o tráfego entre os recursos.

- AWS Elastic Load Balancer
    - O Elastic Load Balancing distribui automaticamente o tráfego de entrada de aplicações entre diversos destinos, como instâncias do Amazon EC2, contêineres, endereços IP, funções do Lambda e dispositivos virtuais.

> **Explicação geral**:  
> O Amazon Virtual Private Cloud (Amazon VPC) oferece controle total sobre seu ambiente de redes virtual, incluindo posicionamento de recursos, conectividade e segurança. Comece a usar configurando sua VPC no console de serviço AWS. Em seguida, adicione recursos a ela, como instâncias do Amazon Elastic Compute Cloud (EC2) e Amazon Relational Database Service (RDS). Por fim, defina como suas VPCs se comunicam entre si, entre contas, zonas de disponibilidade (AZs) ou Regiões da AWS. No exemplo abaixo, o tráfego de rede está sendo compartilhado entre duas VPCs em cada região.

---

## Pergunta 2

**Para manter uma arquitetura híbrida, uma empresa precisa integrar sistemas legados que utilizam serviços tradicionais de mensagens no ambiente on-premises com serviços desacoplados na AWS. Qual serviço de mensageria permite essa integração?**

- Amazon MSK
    - Amazon MSK é excelente para integração de sistemas com necessidades de streaming de dados em tempo real. No entanto, não é ideal para sistemas de mensagens tradicionais porque usa protocolos específicos de Kafka, um modelo de mensageria baseado em logs e é mais complexo de configurar e gerenciar. Sistemas tradicionais como JMS ou AMQP não são suportados nativamente, dificultando a integração direta.

- **❌** Amazon SQS
    - O Simple Queue Service é um serviço de mensageria para troca de mensagens e desacoplamento para arquiteturas AWS.

- Amazon SNS
    - O Simple Notification Service é utilizado para a troca de mensagens através do esquema de Pub/Sub e tópicos, na AWS.

- **✅** Amazon MQ
    - O Amazon MQ é um serviço gerenciado de mensagens baseado no Apache ActiveMQ, ideal para integrar sistemas on-premises com a AWS. Ele suporta protocolos padrão da indústria, como MQTT e AMQP, facilitando a troca de mensagens entre diferentes sistemas. Essa flexibilidade torna o Amazon MQ a escolha mais adequada para integrar sistemas de mensagens tradicionais com serviços na nuvem da AWS.

> **Explicação geral**:  
> O Amazon MQ é um serviço gerenciado de mensagens baseado em Apache ActiveMQ que permite a integração entre sistemas on-premises e sistemas na AWS. Ele oferece protocolos padrão da indústria, como MQTT e AMQP, para troca de mensagens. Ao criar uma instância do Amazon MQ, você pode configurar filas e tópicos para comunicação entre aplicativos em sua infraestrutura local e na nuvem. Isso possibilita a comunicação assíncrona e escalável, permitindo que dados e informações sejam trocados de maneira confiável e eficiente entre ambientes híbridos, mantendo a integridade da troca de informações entre sistemas diferentes.

---

## Pergunta 3

**Uma empresa está desenvolvendo uma plataforma de Machine Learning e requer a transformação de dados provenientes de arquivos de diversas fontes antes de serem analisados. Quais processos precisam ser implementados para alcançar esse objetivo?**

- Extração, transformação e carregamento de dados com o AWS Redshift
    - Amazon Redshift é um serviço de data warehouse que permite consultas e análises de grandes volumes de dados. Embora seja excelente para armazenar e consultar dados, não é ideal para ETL porque não possui funcionalidades nativas de transformação e movimentação de dados.

- Extração, transformação e carregamento de dados com o AWS Athena
    - Amazon Athena é um serviço de consultas interativas que permite analisar dados diretamente no Amazon S3 usando SQL. Embora seja eficaz para consultas ad-hoc e análise de dados, não é ideal para ETL porque não realiza transformações de dados complexas nem movimentação automatizada; é mais adequado para análise e leitura de dados já preparados.

- Extração, transformação e carregamento de dados com o AWS EMR
    - Amazon EMR é um serviço para processamento de grandes volumes de dados usando Hadoop e Spark em clusters gerenciados. Embora poderoso, não é o mais indicado para ETL devido à complexidade de configuração e manutenção.

- **✅** Extração, transformação e carregamento de dados com o AWS Glue
    - O AWS Glue é um serviço gerenciado para integração de dados, facilitando o processo de ETL (Extração, Transformação e Carga) antes de serem consumidos por outros serviços.

> **Explicação geral**:  
> O AWS Glue é um serviço gerenciado para integração de dados, facilitando o processo de ETL (Extração, Transformação e Carga). Ele extrai dados de várias fontes, os transforma usando Python ou Scala para limpeza e formatação, e os carrega em destinos finais como data warehouses. O ETL é crucial porque melhora a qualidade dos dados, permite integração de informações diversas e prepara dados para análise eficiente. Automatiza processos, reduzindo intervenções manuais e acelerando o fluxo de trabalho. O AWS Glue simplifica a movimentação e integração de dados, otimizando o uso para análises e desenvolvimento de aplicações.

---

## Pergunta 4

**Uma empresa precisa integrar APIs de um software desenvolvido no Salesforce com APIs de aplicativos de negócios desenvolvidos internamente. Como realizar essa integração de maneira mais eficiente?**

- Com uso do Amazon SNS. Configure fluxos de integração, mapeie dados e implemente segurança, facilitando a transferência eficiente de dados de forma automatizada.
    - O Amazon Simple Notification Service (Amazon SNS) é um serviço de mensagens totalmente gerenciado para a comunicação de aplicação para aplicação (A2A) e de aplicação para pessoa (A2P). A funcionalidade pub/sub de A2A fornece tópicos para sistemas de mensagens de alta taxa de transferência baseados em push e de muitos para muitos entre sistemas distribuídos, microserviços e aplicativos sem servidor orientados por eventos.

- Com uso do Amazon DMS. Configure fluxos de integração, mapeie dados e implemente segurança, facilitando a transferência eficiente de dados de forma automatizada.
    - O AWS Database Migration Service (AWS DMS) ajuda você a migrar bancos de dados para a AWS de modo rápido e seguro. O banco de dados de origem permanece totalmente operacional durante a migração, minimizando o tempo de inatividade de aplicações que dependem do banco de dados.

- Com uso do Amazon EventBridge. Configure fluxos de integração, mapeie dados e implemente segurança, facilitando a transferência eficiente de dados de forma automatizada.
    - O Amazon EventBridge é um barramento de eventos sem servidor que torna mais fácil a criação de aplicações orientadas por eventos em escala usando eventos gerados com base em suas aplicações, aplicações integradas de software como serviço (SaaS) e serviços da AWS.

- **✅** Com uso do AWS AppFlow. Configure fluxos de integração, mapeie dados e implemente segurança, facilitando a transferência eficiente de dados de forma automatizada.
    - O AWS AppFlow simplifica a integração de dados entre serviços da AWS e aplicativos de SaaS, eliminando a necessidade de criar conectores personalizados. Diferentemente de métodos tradicionais que demandam esforço significativo e uma equipe qualificada, o AppFlow facilita o intercâmbio de dados, permitindo configurações simples e ágeis.

> **Explicação geral**:  
> O AWS AppFlow simplifica a integração de dados entre serviços da AWS e aplicativos SaaS, eliminando a necessidade de criar conectores personalizados. Em vez de gastar tempo e recursos com métodos tradicionais, que exigem equipes qualificadas e esforços significativos, o AppFlow oferece uma solução rápida e intuitiva. Ele permite configurações ágeis e automação do intercâmbio de dados, reduzindo o tempo de desenvolvimento e assegurando uma integração eficiente. Com o AppFlow, você obtém uma solução escalável e fácil de usar, sem a complexidade de desenvolver conectores de API manualmente.

> **Nota**:  
> Salesforce é uma plataforma de software em nuvem (não é da AWS) que oferece serviços de gerenciamento de relacionamento com o cliente (CRM). Ela permite às empresas organizar, automatizar e analisar interações com clientes e leads. O Salesforce é amplamente utilizado para melhorar o engajamento e a eficiência nas operações comerciais. No contexto da pergunta, poderia ser utilizado qualquer software de terceiro fornecido através de SaaS.

---

## Pergunta 5

**Como é possível aprimorar o desempenho de uploads de arquivos em uma aplicação que enfrenta problemas de performance devido a congestionamentos no tráfego da internet?**

- Habilitando o AWS Snowball
    - O Snowball é um dispositivo físico para migrar grandes quantidades de dados entre data centers.

- Habilitando o Amazon Elastic File System (EFS)
    - O Amazon Elastic File System (EFS) é um serviço de armazenamento de arquivos escalável e totalmente gerenciado que pode ser montado em várias instâncias EC2 simultaneamente. Embora o EFS seja ideal para armazenar e compartilhar dados entre instâncias, ele não é projetado especificamente para otimizar o processo de upload de arquivos para a nuvem.

- **✅** Habilitando o AWS Global Accelerator
    - O AWS Global Accelerator pode otimizar a rota do tráfego de rede para sua aplicação, reduzindo a latência e melhorando a performance de upload ao redirecionar o tráfego para a região mais próxima e com melhor desempenho.

- Habilitando o AWS DataSync
    - O AWS DataSync é utilizado para automatizar e otimizar processos de sincronização de dados entre Data Centers.

> **Explicação geral**:  
> O AWS Global Accelerator é um serviço de rede que melhora a disponibilidade e a performance de aplicativos globais. Ele utiliza a infraestrutura da Amazon Web Services para fornecer dois endereços IP estáticos que atuam como pontos de entrada fixos para a aplicação, distribuindo o tráfego de rede de forma otimizada através da rede global da AWS. O Global Accelerator aumenta a resiliência ao redirecionar automaticamente o tráfego de rede para a região mais próxima e com melhor desempenho, além de reduzir a latência e melhorar a experiência do usuário final. Quando a Internet está congestionada, otimiza o caminho para sua aplicação manter a perda de pacotes, o jitter e a latência consistentemente baixos. Fornece IPs estáticos como pontos únicos de entrada para a otimização da performance.

---

## Pergunta 6

**Uma empresa tem uma extensa base de dados, tanto estruturados quanto não estruturados, e busca processá-la por meio de ferramentas de Big Data. Qual serviço da AWS você recomendaria para essa finalidade?**

- **✅** Amazon EMR
    - O Amazon EMR (Elastic MapReduce) é uma solução de Big Data em nuvem líder no setor para processamento de dados em grande escala, análise interativa e machine learning.

- Amazon RedShift
    - O Redshift é um serviço utilizado para BI (Business Intelligence).

- Amazon Kinesis
    - O Kinesis é um serviço de transferência de dados em tempo real em streaming de diversos serviços e aplicativos para repositórios da AWS.

- Amazon Hadoop
    - O Amazon Hadoop não existe, mas o "Apache Hadoop" é um framework disponível dentro da plataforma EMR, de código aberto para processamento e armazenamento distribuído de grandes volumes de dados em clusters de computadores.

> **Explicação geral**:  
> O Amazon EMR (Elastic MapReduce) é uma solução de Big Data em nuvem líder no setor para processamento de dados em grande escala, análise interativa e machine learning. Ele facilita a execução de frameworks de código aberto como Apache Spark, Apache Hive, Presto e Apache Hadoop. O Hadoop, em particular, é utilizado para processamento distribuído de grandes conjuntos de dados, aproveitando o modelo de programação MapReduce. Com o EMR, as empresas podem facilmente escalar seus clusters para atender à demanda, executar tarefas complexas de análise de dados, e integrar-se com outros serviços da AWS, como S3, para armazenamento e gerenciamento de dados. Isso torna o EMR uma escolha poderosa e flexível para diversas aplicações de Big Data e machine learning.

---

## Pergunta 7

**Uma aplicação necessita de três bases de dados estruturadas para armazenar e relacionar informações sobre clientes, pedidos e itens de pedidos. Qual serviço você recomendaria para essa finalidade?**

- Data Migration Service (DMS)
    - O AWS Database Migration Service (AWS DMS) ajuda você a migrar bancos de dados para a AWS de modo rápido e seguro.

- **✅** Relational Database Service (RDS)
    - O Amazon Relational Database Service (RDS) é uma coleção de serviços gerenciados que facilita a configuração, operação e escalabilidade de bancos de dados estruturados e relacionais na nuvem.

- DynamoDB
    - O Amazon DynamoDB é um banco de dados NoSQL que oferece desempenho de alta velocidade e baixa latência, ideal para aplicações que requerem escalabilidade e performance em larga escala. No entanto, ele não é um banco de dados relacional e não é recomendado para aplicações que exigem relacionamentos complexos entre tabelas, como joins e transações ACID que são comuns em bancos de dados relacionais. DynamoDB é mais adequado para aplicativos que precisam de uma estrutura flexível de dados e alta disponibilidade.
- Keys Management Service (KMS)
    - O AWS Key Management Service (KMS) facilita a criação e o gerenciamento de chaves criptográficas e o controle do seu uso em uma ampla variedade de serviços da AWS e em seus aplicativos.

> **Explicação geral**:  
> O Amazon Relational Database Service (RDS) é um serviço gerenciado que simplifica a configuração, operação e escalabilidade de bancos de dados relacionais na nuvem. Ele permite que você se concentre em suas aplicações, enquanto o RDS cuida da administração de banco de dados, como backups, atualizações e manutenção. O serviço suporta diversos mecanismos de banco de dados, incluindo Amazon Aurora compatível com MySQL e PostgreSQL, MySQL, MariaDB, PostgreSQL, Oracle e SQL Server. Cada um desses mecanismos oferece opções flexíveis de armazenamento e desempenho para atender a diferentes necessidades e preferências de aplicações. O RDS facilita a escalabilidade automática e o gerenciamento de cargas de trabalho, otimizando o desempenho e a disponibilidade dos bancos de dados.

---

## Pergunta 8

**Para evitar ameaças na sua infraestrutura, você deseja verificar continuamente arquivos que possam ter algum malware criando comportamento suspeito em cargas de trabalho em instâncias ou contêineres. Qual é o serviço que utiliza inteligência artificial para realizar esse tipo de verificação em dados no EBS e em outros serviços da sua plataforma?**

- AWS Shield
    - O AWS Shield é um serviço gerenciado de proteção contra DDoS (Negação de serviço distribuída) que protege os aplicativos executados na AWS. O AWS Shield oferece de detecção e mitigações em linha automáticas e sempre ativas que minimizam o tempo de inatividade e a latência dos aplicativos, fornecendo proteção contra DDoS sem necessidade de envolver o AWS Support.

- AWS WAF
    - O AWS WAF (Web Application Firewall) protege aplicações web contra ameaças e ataques na camada de aplicação, como injeção de SQL e XSS. Ele permite definir regras personalizadas para filtrar e monitorar tráfego HTTP/HTTPS. Integrado com serviços como CloudFront e Application Load Balancer, oferece uma camada adicional de segurança.

- AWS Macie
    - O Amazon Macie é um serviço de segurança e privacidade de dados totalmente gerenciado que usa machine learning e correspondência de padrões para descobrir e proteger seus dados confidenciais na AWS. À medida que as organizações gerenciam volumes crescentes de dados, identificar e proteger seus dados confidenciais em escala pode se tornar cada vez mais complexo, caro e demorado.

- **✅** AWS GuardDuty
    - O AWS GuardDuty usa inteligência artificial para analisar dados de eventos armazenados no S3 e detectar atividades maliciosas, como malware. Ele protege sua infraestrutura identificando e respondendo a ameaças em tempo real.

> **Explicação geral**:  
> O AWS GuardDuty é um serviço de detecção de ameaças que utiliza inteligência artificial para analisar dados de eventos de vários serviços AWS e armazenados no S3. Ele monitora continuamente atividades em sua infraestrutura para identificar comportamentos suspeitos e potenciais ameaças, como malware e atividades maliciosas. O GuardDuty gera alertas em tempo real sobre possíveis incidentes de segurança, permitindo uma resposta rápida. Ele usa machine learning e análise de comportamentos para detectar ameaças que podem não ser visíveis através de métodos tradicionais. Assim, ajuda a proteger suas aplicações e dados contra ataques e violações.

---

## Pergunta 9

**Uma aplicação sem servidor demanda que cada serviço orquestrado produza logs e os armazene temporariamente para verificações e suporte. Que serviço pode ser adotado para essa finalidade?**

- CloudTrail
    - O CloudTrail é utilizado para logar ações de usuários em APIs de serviços da AWS, muito utilizado em auditorias de uso das contas.

- Storage Gateway
    - O AWS Storage Gateway é um serviço que conecta seu ambiente local a serviços de armazenamento na nuvem da AWS. Ele fornece uma interface de armazenamento híbrido, permitindo que você use armazenamento na nuvem da AWS como uma extensão do armazenamento local.

- CloudLogs
    - Este serviço não existe.

- **✅** CloudWatch Logs
    - Você pode usar o Amazon CloudWatch Logs para monitorar, armazenar e acessar seus arquivos de log em suas instâncias do Amazon Elastic Compute Cloud (Amazon EC2), no AWS CloudTrail, no Route 53 ou em outras origens.

> **Explicação geral**:  
> O CloudWatch Logs permite centralizar os logs de todos os sistemas, aplicações e produtos da AWS que você usa em um único serviço altamente escalável. Você pode facilmente visualizá-los, pesquisá-los por códigos de erro ou padrões específicos, filtrá-los com base em campos específicos ou arquivá-los com segurança para análise futura.

---

## Pergunta 10

**Uma aplicação fará uso de uma base de dados no modelo chave e valor. A chave será o CPF e o valor será um arquivo Json não estruturado, com diversas informações associadas ao CPF do cliente. Qual é o banco de dados adequado para atender esse cenário?**

- **✅** Amazon DynamoDB
    - O Amazon DynamoDB é o banco de dados adequado, pois usa o modelo de chave e valor e suporta o armazenamento de arquivos JSON não estruturados associados a chaves, como o CPF.

- Amazon Aurora
    - O Amazon Aurora é um banco de dados relacional e não é ideal para dados no formato chave e valor e arquivos JSON não estruturados. Ele é projetado para consultas SQL e modelos de dados relacionais.

- Amazon Neptune
    - O Amazon Neptune é um banco de dados de grafos, projetado para modelar e consultar relações complexas entre dados em grafos. Não é adequado para o cenário descrito, que envolve armazenamento de dados no formato chave e valor e arquivos JSON não estruturados.

- Amazon KeySpaces
    - O Amazon Keyspaces (para Apache Cassandra) é um banco de dados NoSQL gerenciado que é otimizado para modelos de dados em colunas, não para o armazenamento de dados no formato chave e valor e arquivos JSON não estruturados.

> **Explicação geral**:  
> O Amazon DynamoDB é o banco de dados adequado para esse cenário. Ele é um banco de dados NoSQL que utiliza o modelo de chave e valor, permitindo armazenar e recuperar informações associadas a chaves, como o CPF no seu caso. DynamoDB é ideal para armazenar arquivos JSON não estruturados e fornece alta disponibilidade, escalabilidade e desempenho em milissegundos. Esse banco não exige uma estrutura de dados fixa dos dados, ele permite a utilização de tabelas com os campos chave e valor, onde chave é uma identificação do registro e o campo valor pode ser um arquivo json com vários dados não estruturados.

---

## Pergunta 11

**Um cientista de dados está criando um modelo para prevenção a fraudes em cartões de crédito. Qual serviço oferece uma plataforma completa com recursos para implementar modelos de aprendizado de máquina para diversas necessidades de negócio?**

- Amazon RedShift
    - O Amazon Redshift não é ideal para criar modelos de aprendizado de máquina como o Amazon SageMaker, pois é um data warehouse projetado para consultas analíticas e processamento de grandes volumes de dados.

- **✅** Amazon SageMaker
    - O Amazon SageMaker oferece uma plataforma completa com recursos para implementar modelos de aprendizado de máquina, incluindo treinamento, ajuste e implantação, atendendo a diversas necessidades de negócios, como a prevenção de fraudes em cartões de crédito.

- EMR
    - O Amazon EMR (Elastic MapReduce) não é a melhor escolha para criar e gerenciar modelos de aprendizado de máquina porque é um serviço de processamento de big data que se concentra na análise e processamento de grandes volumes de dados usando frameworks como Apache Hadoop e Apache Spark.

- Amazon Step Function
    - O AWS Step Functions não é adequado para criar e treinar modelos de aprendizado de máquina porque é um serviço de orquestração de workflows que coordena a execução de diferentes serviços e funções na AWS. Ele é ideal para organizar e automatizar processos complexos envolvendo vários serviços.

> **Explicação geral**:  
> O Amazon SageMaker oferece uma ampla gama de ferramentas para machine learning na AWS, facilitando o desenvolvimento e a implantação de modelos. Ele permite personalizar soluções e é compatível com a implantação rápida de modelos com um clique. O SageMaker suporta o ajuste fino de mais de 150 modelos de código aberto populares, abrangendo áreas como processamento de linguagem natural, detecção de objetos e classificação de imagem. Com essas funcionalidades, ele proporciona flexibilidade e eficiência no desenvolvimento de modelos de ML.

---

## Pergunta 12

**Uma plataforma de rede social precisa implementar uma solução para impedir que usuários carreguem imagens com conteúdo inadequado em suas páginas. Qual serviço, utilizando inteligência artificial, pode auxiliar nessa tarefa?**

- Amazon SageMaker
    - Amazon SageMaker é um serviço de Machine Learning totalmente gerenciado. Com o SageMaker, cientistas de dados e desenvolvedores podem criar e treinar modelos de Machine Learning com rapidez e facilidade e, depois, implantá-los diretamente em um ambiente hospedado pronto para produção.

- Amazon Images
    - Amazon Images não é um serviço válido, o serviço mais próximo é o Amazon Machine Image (AMI) que não tem relação alguma a processamento de arquivos de imagens. Uma Imagem de máquina da Amazon (AMI) é uma imagem suportada e mantida pela AWS que fornece as informações necessárias para iniciar uma instância de EC2.

- Amazon Polly
    - O Amazon Polly é um serviço de nuvem que converte texto em fala realista.

- **✅** Amazon Rekognition
    - O serviço que pode ajudar a impedir o carregamento de imagens com conteúdo inadequado é o Amazon Rekognition. Esse serviço de inteligência artificial analisa imagens e vídeos para detectar e classificar objetos, atividades e conteúdo impróprio, permitindo a filtragem e moderação automática de imagens carregadas pelos usuários.

> **Explicação geral**:  
> O Amazon Rekognition usa inteligência artificial para analisar imagens e vídeos, identificando conteúdo inadequado como nudidade e violência. Ele automatiza a moderação de imagens em plataformas de redes sociais, garantindo que o conteúdo esteja de acordo com as diretrizes. O serviço oferece análises precisas e em tempo real, reduzindo a necessidade de moderação manual e mantendo o ambiente seguro para os usuários.

---

## Pergunta 13

**Antes de iniciar o desenvolvimento de uma aplicação, um programador deseja verificar se algo similar já foi criado e está disponível para comercialização na AWS. Como é possível realizar essa verificação?**

- **✅** Pesquisando no AWS Marketplace
    - O Amazon Marketplace é uma plataforma onde os fornecedores podem listar, vender e fornecer aplicativos prontos e soluções de software diretamente aos clientes da AWS.

- Pesquisando no AWS OpsWorks
    - O AWS OpsWorks é um serviço de gerenciamento de configurações que oferece instâncias gerenciadas do Chef e do Puppet. O Chef e o Puppet são plataformas de automação que permitem usar código para automatizar a configuração de servidores. O OpsWorks permite usar o Chef e o Puppet para automatizar a forma como os servidores são configurados, implantados e gerenciados em instâncias do Amazon EC2 ou ambientes de computação no local.

- Pesquisando no AWS MFA
    - O AWS MFA - Multi Factor Authentication adiciona uma camada a mais no processo de autenticação no login pelo Console.

- Pesquisando no AWS AMI
    - O AWS AMI - Amazon Machine Images (AMIs) são pré-configurações de uma lista de sistemas operacionais para a instalação instantânea em instâncias EC2.

> **Explicação geral**:  
> O Amazon Marketplace é uma plataforma onde os fornecedores podem listar, vender e fornecer aplicativos prontos e soluções de software diretamente aos clientes da AWS. Os clientes podem procurar e adquirir esses aplicativos, que variam desde software empresarial até soluções de análise de dados e segurança. O processo de compra envolve selecionar um aplicativo, revisar detalhes e preços, e aceitar os termos. A implantação é simplificada por meio de integrações com serviços AWS, facilitando a implementação e a configuração de aplicativos prontos para uso.

---

## Pergunta 14

**Uma organização transferiu diversos arquivos de histórico para um bucket no Amazon S3, e esses arquivos não precisam ser recuperados imediatamente quando solicitados. Qual classe de armazenamento é recomendada para minimizar os custos com essa solução?**

- **✅** S3 Glacier Deep Archive
    - O S3 Glacier Deep Archive é a opção mais econômica de armazenamento no Amazon S3, ideal para dados de longo prazo que são acessados raramente.

- S3 Glacier Instant Retrieval
    - O S3 Glacier Instant Retrieval oferece armazenamento de baixo custo para dados de longa duração, com recuperação quase instantânea. Permite economizar até 68% em comparação com outras classes de armazenamento quando os dados são acessados trimestralmente. Ideal para arquivos que exigem acesso imediato, como imagens médicas ou mídia de notícias.

- S3 Standard
    - O S3 Standard oferece um armazenamento de objetos com altos níveis de resiliência, disponibilidade e performance para dados acessados com frequência. Como fornece baixa latência e alto throughput, o S3 Standard é adequado para uma grande variedade de casos de uso, como aplicações na nuvem, sites dinâmicos, distribuição de conteúdo, aplicações móveis e de jogos e análise de big data.

- S3 Intelligent-Tiering
    - O S3 Intelligent-Tiering é uma solução de armazenamento em nuvem que otimiza automaticamente os custos ao mover os dados para o nível de acesso mais econômico, com base na frequência de uso, sem comprometer o desempenho ou a recuperação dos dados. Oferece alta velocidade de transferência e baixa latência, independentemente da frequência de acesso dos dados. Essa solução possui três níveis de acesso e pode ser aplicada em uma ampla gama de cargas de trabalho, incluindo data lakes, análise de dados e conteúdo gerado pelo usuário.

> **Explicação geral**:  
> O S3 Glacier Deep Archive é a opção mais econômica de armazenamento no Amazon S3, ideal para dados de longo prazo que são acessados raramente. É adequado para organizações que precisam manter dados por períodos prolongados para conformidade regulatória. Além disso, é uma alternativa acessível e fácil de gerenciar para backup e recuperação de desastres, embora o tempo de recuperação possa ser de até 12 horas.

---

## Pergunta 15

**Uma repartição pública estabeleceu parcerias com a Microsoft e Adobe para a utilização de diversos softwares licenciados. Qual serviço da AWS pode auxiliá-la no controle do uso destas e de outras licenças?**

- Certificate Manager
    - O Certificate Manager é utilizado para gerenciar certificados digitais para criptografar os dados trafegados entre os usuários e servidores.

- Control Tower
    - O AWS Control Tower facilita a configuração e governança de ambientes multi-conta na AWS, oferecendo uma visão centralizada e automatizada das políticas de segurança e conformidade. Ele ajuda a implementar práticas recomendadas e a gerenciar contas de forma eficiente.

- Parameter Store
    - O AWS Systems Manager Parameter Store é um serviço para armazenar e gerenciar dados de configuração e segredos, como strings e valores de parâmetros. Oferece armazenamento seguro, com acesso controlado e criptografado, para facilitar a gestão de configurações e credenciais em suas aplicações.

- **✅** License Manager
    - O License Manager permite maior visibilidade e controle sobre como as licenças de software são utilizadas e evite o mau uso. Aumenta a economia de dinheiro com a máxima utilização de licenças, incluindo como rastrear e gerenciar as licenças. Reduz os riscos de não conformidade fortalecendo os limites de uso de licença, bloqueando novos lançamentos e usando outros controles.

> **Explicação geral**:  
> O AWS License Manager oferece visibilidade e controle sobre a utilização de licenças de software, ajudando a evitar o mau uso e a maximizar a economia com a utilização eficiente das licenças. Permite rastrear e gerenciar licenças de forma centralizada, reduzindo o risco de não conformidade ao reforçar os limites de uso e bloquear novos lançamentos não autorizados. Além disso, proporciona controles adicionais para garantir que as licenças sejam usadas conforme os termos acordados, promovendo um gerenciamento mais eficiente e seguro.

---

## Pergunta 16

**A estrutura de uma aplicação utiliza o ASG para incorporar novas instâncias EC2 à medida que o número de usuários e a demanda computacional aumentam. De que maneira o ELB poderia ser integrado nesta solução?**

- **✅** Distribuindo o tráfego de dados entre todas as instâncias, existentes e novas.
    - Conforme a demanda aumenta, o ASG dimensiona as instâncias para cima, enquanto o ELB distribui o tráfego de maneira uniforme, permitindo uma escalabilidade suave e eficiente.

- Configurando o sistema operacional e demais recursos das novas instâncias.
    - O ELB não gerencia ou configura o sistema operacional das instâncias; essa responsabilidade é do Auto Scaling ou scripts de configuração, que são usados para iniciar e configurar instâncias conforme necessário.

- Criando um cluster de máquinas dentro da mesma zona de disponibilidade
    - O ELB é utilizado para balancear a carga entre várias zonas de disponibilidade, garantindo alta disponibilidade e resiliência. Ele não cria um cluster de máquinas, mas sim direciona o tráfego entre as instâncias existentes para assegurar uma distribuição eficiente da carga.

- Instanciando uma nova máquina quando uma das máquinas apresenta falha
    - O ELB (Elastic Load Balancer) não é responsável por iniciar uma nova instância em caso de falha; sua função é parar de direcionar o tráfego para a instância problemática e distribuir a carga apenas entre as instâncias saudáveis e disponíveis.

> **Explicação geral**:  
> Para distribuir o tráfego de forma eficiente entre as instâncias em execução, o Amazon Elastic Load Balancer (ELB) é usado. Ele equilibra a carga entre as instâncias para otimizar o desempenho e a disponibilidade do aplicativo. Conforme a demanda aumenta, o ASG dimensiona as instâncias para cima, enquanto o ELB distribui o tráfego de maneira uniforme, permitindo uma escalabilidade suave e eficiente, garantindo alta disponibilidade e desempenho em ambientes dinâmicos e em constante mudança. No contexto de escalabilidade na AWS, esses três serviços desempenham papéis complementares. O Amazon EC2 (Elastic Compute Cloud) fornece instâncias virtuais escaláveis que hospedam os aplicativos. As instâncias são gerenciadas automaticamente através de grupos de autoatendimento (ASG), onde o Amazon Auto Scaling Group (ASG) monitora a carga e ajusta automaticamente o número de instâncias em execução para corresponder à demanda.

---

## Pergunta 17

**Quando se cria uma ou mais instâncias EC2 dentro de uma VPC, é necessário associá-las a um Security Group. Qual é a finalidade desse serviço?**

- Garantir que as instâncias realizem o escalonamento automático.
    - O escalonamento automático é realizado pelo ASG (Auto Scaling Group).

- Manter uma rede virtual entre as zonas de disponibilidade.
    - Essa função é do serviço VPC (Virtual Private Cloud).

- **✅** Controlar o tráfego de entrada e saída de dados das instâncias agrupadas.
    - O Security Group é uma espécie de firewall para as máquinas de uma VPC. Você pode utilizá-lo para agrupar diversas máquinas com a mesma função, como banco de dados, aplicação, também pode ser utilizado no lançamento de novas máquinas para receber as mesmas configurações de entrada e saída de dados do grupo.

- Agrupar as instâncias para a gestão de custos.
    - Os custos são gerenciados pelo AWS Cost Explorer.

> **Explicação geral**:  
> O Security Group é um recurso de segurança na AWS que atua como um firewall virtual para controlar o tráfego de rede das instâncias dentro de uma VPC (Virtual Private Cloud). Ele permite definir regras de entrada e saída para gerenciar quais tipos de tráfego são permitidos ou bloqueados para as instâncias associadas. Você pode usar o Security Group para agrupar instâncias com funções semelhantes, como bancos de dados ou servidores de aplicações, e aplicar configurações de segurança consistentes a elas. Quando você lança novas instâncias, pode associá-las a um Security Group existente para garantir que elas herdem automaticamente as mesmas regras de segurança. Isso facilita a gestão e a escalabilidade das configurações de segurança em sua infraestrutura na AWS.

---

## Pergunta 18

**Um sistema de comércio eletrônico utiliza microsserviços independentes e desacoplados, permitindo escalabilidade independente para cada um deles. Como os microsserviços podem ser integrados e comunicar entre si de maneira eficaz?**

- Com funções Lambda
    - O Lambda é utilizado para a implementação de funções sem servidor.

- **❌** Com mensagens do SNS
    - O Amazon SNS (Simple Notification Service) é um serviço de Pub/Sub que facilita o envio de notificações e mensagens para múltiplos destinos, como e-mails, SMS e endpoints HTTP. Ele permite que aplicações enviem mensagens de forma escalável e confiável para uma ampla audiência.

- **✅** Com filas SQS
    - O Amazon Simple Queue Service (SQS) é um serviço de filas de mensagens gerenciado que permite o desacoplamento e a escalabilidade de microsserviços, sistemas distribuídos e aplicações sem servidor.

- Com funções do Fargate
    - O Fargate é utilizado para o uso de container sem servidor.

> **Explicação geral**:  
> O Amazon Simple Queue Service (SQS) é um serviço gerenciado que oferece filas de mensagens para desacoplar e escalar microsserviços, sistemas distribuídos e aplicações sem servidor. Ele permite que as aplicações enviem e recebam mensagens de forma assíncrona, facilitando a comunicação entre componentes de sistemas sem que eles precisem interagir diretamente. O SQS elimina a necessidade de gerenciar infraestrutura de middleware, como servidores de mensagens, reduzindo a complexidade e a sobrecarga operacional.

---

## Pergunta 19

**A equipe de DevOps de uma empresa desenvolveu uma pipeline de integração e entrega contínua (CI/CD) utilizando serviços da AWS. Qual serviço é encarregado pela compilação e pelos testes automatizados neste processo?**

- AWS CodeCommit
    - O AWS CodeCommit é o serviço para gerenciar o código fonte gerado pelos desenvolvedores.

- AWS CodeDeploy
    - O AWS CodeDeploy é o serviço utilizado para implantar e distribuir a aplicação compilada pelo AWS CodeBuild em algum serviço, instâncias EC2, ECS, S3, etc.

- **✅** AWS CodeBuild
    - O AWS CodeBuild é um serviço de integração contínua totalmente gerenciado que compila o código-fonte, realiza testes e produz pacotes de software prontos para implantação.

- AWS Pipeline
    - O AWS Pipeline não existe, entretanto, existe um serviço chamado AWS CodePipeline que é utilizado para montar a esteira que integra todos esses serviços fornecendo funções de CI/CD para desenvolvimento e entrega contínua: CodeCommit, CodeBuild e CodeDeploy.

> **Explicação geral**:  
> O AWS CodeBuild é um serviço de integração contínua totalmente gerenciado que compila o código-fonte, realiza testes e produz pacotes de software prontos para implantação. Com o CodeBuild, você não precisa provisionar, gerenciar e escalar seus próprios servidores de compilação. O CodeBuild escala continuamente e processa múltiplas compilações ao mesmo tempo, o que evita que elas fiquem esperando em uma fila. Você pode começar a usar rapidamente com ambientes de compilação pré-definidos ou criar ambientes de compilação personalizados com suas próprias ferramentas de compilação.

---

## Pergunta 20

**Um desenvolvedor front-end desenvolveu um site estático e gostaria de hospedá-lo na infraestrutura da AWS. Qual é a maneira mais rápida e econômica de publicar esse site na internet?**

- **✅** Com um bucket do S3 habilitado para hospedar um site estático
    - Com o S3 é possível implementar de forma rápida um bucket como host de páginas estáticas. Através de uma configuração simples é possível transformar o bucket e um host e disponibilizar os arquivos através de links através da internet.

- Com uma pasta virtual no EC2 habilitada para hospedar um site estático
    - O Amazon Elastic Compute Cloud (Amazon EC2) é um serviço Web que disponibiliza capacidade computacional segura e redimensionável na nuvem. Ele foi projetado para facilitar a computação em nuvem na escala da web, mas não é a maneira mais fácil e econômica para a implementação do site estático.

- Com o site em cache no ElastiCache
    - O Amazon ElastiCache permite configurar e escalar repositórios de dados na memória na nuvem, compatíveis com código aberto. Ele melhora a performance de aplicativos ao fornecer armazenamento em cache de alta taxa de transferência e baixa latência. É ideal para casos de uso em tempo real, como cache, armazenamento de sessão e análises rápidas.

- Com um Json no DynamoDb para ser carregado com um site estático
    - O Amazon DynamoDB é um banco de dados de chave-valor, não tem a finalidade de armazenar páginas de sites.

> **Explicação geral**:  
> O Amazon S3 (Simple Storage Service) permite criar um bucket para hospedar páginas estáticas de forma rápida e fácil. Você pode configurar o bucket para servir como um site estático, simplesmente carregando seus arquivos HTML, CSS e JavaScript para o bucket. Após a configuração, o S3 fornece um endpoint da web que você pode usar para acessar os arquivos diretamente pela internet. Essa abordagem é ideal para sites estáticos devido à sua simplicidade e escalabilidade. Além disso, o S3 oferece alta disponibilidade e durabilidade dos arquivos armazenados.

---

## Pergunta 21

**Uma empresa busca integrar sua rede local (on-premises) a uma rede virtual na AWS, buscando a menor latência possível. Qual serviço deve ser empregado para atingir esse objetivo?**

- AWS API Gateway
    - O AWS API Gateway é um serviço projetado para criar, publicar e gerenciar APIs RESTful, e não para conectar redes on-premises a redes virtuais na AWS. Ele não oferece conexões de rede direta ou reduz a latência entre infraestruturas de rede, como o AWS Direct Connect faz.

- AWS DataSync
    - O AWS DataSync é um serviço destinado a mover grandes volumes de dados de maneira eficiente entre sistemas de armazenamento, mas não é projetado para estabelecer uma conexão de rede contínua entre infraestruturas. Ele é ideal para migrações de dados e sincronização de sistemas de armazenamento, mas não substitui serviços como o AWS Direct Connect para conectividade de rede dedicada e consistente com baixa latência.

- **✅** AWS Direct Connect
    - AWS Direct Connect oferece uma conexão de baixa latência, crucial para aplicações que requerem respostas rápidas e consistentes. Ao estabelecer um link dedicado entre sua infraestrutura e a AWS, o serviço evita o tráfego na Internet pública, reduzindo significativamente o tempo de ida e volta dos dados (round-trip time).

- AWS VPN
    - O AWS VPN não é a melhor opção para obter a menor latência possível porque utiliza a Internet pública para transmitir dados, o que pode introduzir variações e aumentos na latência. Além disso, o AWS VPN oferece menor largura de banda comparado ao AWS Direct Connect, que proporciona uma conexão dedicada e mais estável.

> **Explicação geral**:  
> O AWS Direct Connect utiliza a infraestrutura global da AWS para otimizar a conexão entre suas redes e os recursos na nuvem. Este serviço oferece um caminho direto e dedicado para acessar seus serviços na AWS, evitando o tráfego pela Internet pública. Como resultado, todo o tráfego de rede permanece dentro da rede segura e altamente redundante da AWS, garantindo uma conexão mais rápida e confiável. Essa abordagem minimiza o risco de gargalos e variações inesperadas de latência, proporcionando uma experiência de rede mais estável e previsível. Além disso, o AWS Direct Connect pode ser configurado para oferecer maior largura de banda, atendendo às necessidades específicas de desempenho e segurança de sua empresa.

---

## Pergunta 22

**Uma startup em expansão está contratando novos colaboradores com bastante frequência. Como os acessos às contas da AWS devem ser concedidos a esses novos colaboradores?**

- Incluindo os novos colaboradores no EC2
    - O Amazon EC2 (Elastic Compute Cloud) é um serviço que fornece instâncias de máquinas virtuais para executar aplicativos e cargas de trabalho na nuvem. Ele não é utilizado para gerenciar acessos ou permissões de usuários.

- Incluindo os novos colaboradores no S3
    - O Amazon S3 (Simple Storage Service) é utilizado para armazenar e gerenciar dados, como arquivos e backups, não para gerenciar acessos e permissões de usuários.

- **✅** Incluindo os novos colaboradores no IAM
    - Para gerenciar acessos às contas da AWS, a startup deve usar o AWS Identity and Access Management (IAM). O IAM permite criar e gerenciar usuários e grupos, definir permissões de acesso e aplicar políticas de segurança. Com ele, é possível fornecer acesso adequado aos novos colaboradores com base em suas funções.

- Incluindo os novos colaboradores no CloudFront
    - O Amazon CloudFront é um serviço de CDN (Content Delivery Network) usado para distribuir conteúdo de forma rápida e segura para os usuários finais. Ele melhora a performance de entrega de dados e reduz a latência, mas não é usado para gerenciar acessos ou permissões de usuários na AWS.

> **Explicação geral**:  
> Para incluir novos colaboradores em uma empresa com o AWS Identity and Access Management (IAM), siga estes passos:
> 1. Crie um usuário IAM para cada novo colaborador, atribuindo um nome de usuário e permissões apropriadas com base em suas funções.
> 2. Defina políticas de permissão IAM que determinem quais recursos cada usuário pode acessar e quais ações eles podem realizar.
> 3. Atribua os usuários a grupos IAM, se possível, para facilitar a gestão das permissões e consistência nas políticas.
> 4. Se necessário, configure autenticação multifator (MFA) para reforçar a segurança nas contas dos colaboradores.
> 5. Comunique as credenciais de acesso (nome de usuário, senha e, se aplicável, informações MFA) aos novos colaboradores.
> Dessa forma, você garante que os novos membros da equipe tenham acesso apropriado e seguro aos recursos da AWS de acordo com suas funções e responsabilidades.

---

## Pergunta 23

**Para compor uma aplicação, seu time desenvolveu microsserviços e gostaria de implementá-los numa plataforma computacional baseada em contêineres. Qual serviço deve ser utilizado para essa finalidade?**

- Auto Scaling Group
    - O AWS Auto Scaling monitora os aplicativos e ajusta automaticamente a capacidade para manter um desempenho constante e previsível pelo menor custo possível.

- EC2
    - O Amazon Elastic Compute Cloud (Amazon EC2) é um serviço Web que disponibiliza capacidade computacional segura e redimensionável na nuvem.

- **✅** ECS
    - O Amazon ECS é um serviço de orquestração de contêineres totalmente gerenciado que facilita a implantação, o gerenciamento e a escala de aplicações em contêineres.

- ECR
    - O Amazon Elastic Container Registry (Amazon ECR) é um registro de contêiner totalmente gerenciado que facilita o armazenamento, o gerenciamento, o compartilhamento e a implantação de imagens e artefatos de contêiner em qualquer lugar.

> **Explicação geral**:  
> O Amazon ECS (Elastic Container Service) é um serviço gerenciado que simplifica a execução e a gestão de aplicações em contêineres na AWS. Ele permite a implantação de aplicações em contêineres Docker, facilitando o gerenciamento do ciclo de vida desses contêineres, incluindo escalabilidade e balanceamento de carga. O ECS oferece integração com outros serviços AWS, como IAM e CloudWatch, para fornecer uma solução completa para monitoramento e segurança. Ele suporta tanto o gerenciamento de clusters em instâncias EC2 quanto o uso do AWS Fargate para execução de contêineres sem gerenciar servidores.

---

## Pergunta 24

Para garantir a segurança das suas cargas de trabalho, você precisa implementar processos adicionais de criptografia em algumas aplicações. Qual serviço pode te ajudar nesta implementação? 

- AWS Config
    - O AWS Config é um serviço que permite acessar, auditar e avaliar as configurações dos recursos da AWS. O Config monitora e grava continuamente registros das configurações de recursos da AWS e lhe permite automatizar a avaliação das configurações registradas com base nas configurações desejadas.

- AWS IAM
    - O IAM (Identity and Access Management) é usado para gerenciar usuários e controlar o acesso a recursos na AWS.

- **✅** AWS KMS
    - Com o AWS Key Management Service (AWS KMS), você pode criar, gerenciar e controlar chaves criptográficas nas suas aplicações e em mais de 100 serviços da AWS.

- ACM
    - O AWS Certificate Manager (ACM) facilita a provisionamento, gerenciamento e implantação de certificados SSL/TLS para proteger a comunicação entre usuários e suas aplicações na AWS. Ele automatiza a emissão e renovação de certificados, simplificando a configuração de HTTPS e aumentando a segurança dos dados em trânsito.

> **Explicação geral**:  
> Com o KMS, você pode gerar chaves de criptografia, definir políticas de acesso e rotacionar chaves automaticamente para atender aos requisitos de segurança e conformidade. O serviço integra-se facilmente com outros serviços da AWS, como S3, RDS e EBS, garantindo que dados sejam criptografados e protegidos em repouso e em trânsito. O KMS também fornece auditoria e rastreamento de uso das chaves, ajudando a monitorar e gerenciar a segurança de suas operações criptográficas.

---

## Pergunta 25

Em um projeto de migração, o Diretor de uma empresa requisitou uma projeção de custos para a infraestrutura que será necessária para execução dos sistemas da sua área de negócio na AWS. Qual serviço pode ajudar com essa solicitação?

- **✅** Pricing Calculator
    - AWS Pricing Calculator é uma ferramenta para estimar os custos futuros de serviços AWS com base em configurações e uso planejado. Permite criar cenários personalizados e obter uma previsão detalhada dos custos antes de iniciar a migração ou implementação. (projeção)

- Budget
    - Permite definir e monitorar orçamentos para seus serviços e recursos AWS. Envia alertas e notificações quando os custos ou o uso se aproximam ou excedem os limites estabelecidos, ajudando a controlar gastos.

- Cost Explorer
    - Oferece visualização interativa e análise dos custos e uso atuais da AWS de uma conta já em uso. Ajuda a explorar dados históricos, identificar tendências e realizar previsões para gerenciamento proativo de despesas.

- Billing Conductor
    - O AWS Billing Conductor personaliza custos de infraestrutura ou contas compartilhadas, criando grupos de cobrança para departamentos como financeiro, RH e marketing. Define regras de preços e distribui créditos com base no consumo real, gerando relatórios detalhados para facilitar a gestão do orçamento de cada departamento.

> **Explicação geral**:  
> Com a Pricing Calculator (calculadora de preços) da AWS é possível estimar o custo para sua solução de arquitetura que ainda não foi implementada. Note que a pergunta está relacionada a migração e projeção, não há cargas já em execução na AWS. Configure uma estimativa de custo exclusivo que atenda às suas necessidades de negócios ou pessoais com produtos e serviços da AWS. Veja a matemática por trás do preço das configurações do seu serviço. Veja os preços por serviço ou por grupo de serviços para analisar os custos de sua arquitetura.

---

## Pergunta 26

Uma organização enfrenta desafios de desempenho em suas aplicações críticas devido a lentidão nos acessos aos bancos de dados relacionais MySQL. Qual seria uma abordagem para solucionar essa situação?

- Migrar os bancos de dados para o Neptune
    - O Neptune é um banco de dados totalmente gerenciado pela AWS, noSQL e baseado em Grafos.

- **✅** Migrar os bancos de dados para o Aurora
    - O Amazon Aurora é até cinco vezes mais rápido que bancos de dados MySQL padrão e três vezes mais rápido que bancos de dados PostgreSQL padrão.

- Migrar os bancos de dados para o MariaDb
    - O MariaDb é um banco de dados totalmente gerenciado pela AWS quando utilizado no RDS e não gerenciado quando instalado diretamente numa instância EC2, é relacional mas não é 5x mais rápido que o MySQL.

- Migrar os bancos de dados para o DynamoDb
    - O DynamoDb é um banco de dados totalmente gerenciado pela AWS, noSQL, baseado em chave e valor, não é relacional e nem compatível com o MySQL.

> **Explicação geral**:  
> O Amazon Aurora é até cinco vezes mais rápido que bancos de dados MySQL padrão e três vezes mais rápido que bancos de dados PostgreSQL padrão. O serviço oferece a segurança, a disponibilidade e a confiabilidade de bancos de dados comerciais por um décimo do custo. O Amazon Aurora é gerenciado pelo RDS, que automatiza tarefas administrativas demoradas como provisionamento de hardware, configuração do banco de dados, aplicação de patches e backups.

---

## Pergunta 27

Uma aplicação web necessita de um mecanismo de busca para identificar páginas contendo informações específicas. Como esse recurso pode ser habilitado de maneira simples?

- Crie um domínio no Amazon Athena, configure opções de indexação e integre as APIs a aplicação web.
    - O Amazon Athena permite é um serviço serveless que permite a consulta através de queries SQL em dados armazenados em Bucket do S3.

- Crie um domínio no Amazon ElasticCache, configure opções de indexação e integre as APIs a aplicação web.
    - O Amazon ElasticCache é um serviço que oferece uma solução de armazenamento de informações em cache de forma escalável.

- **✅** Crie um domínio no Amazon CloudSearch, configure opções de indexação e integre as APIs a aplicação web.
    - O Amazon CloudSearch é um serviço gerenciado na nuvem AWS com o qual é possível configurar, gerenciar e dimensionar uma solução de pesquisa para o seu site ou aplicativo de forma simples e econômica.

- Crie um domínio no Amazon ElasticSearchService, configure opções de indexação e integre as APIs a aplicação web.
    - O ElasticSearchService fornece uma alta capacidade de armazenamento de dados de logs de serviços para permitir a análise de problemas e falhas de forma automatizada na sua infraestrutura.

> **Explicação geral**:  
> O Amazon CloudSearch é um serviço gerenciado na nuvem AWS com o qual é possível configurar, gerenciar e dimensionar uma solução de pesquisa para o seu site ou aplicativo de forma simples e econômica. O Amazon CloudSearch oferece suporte para 34 idiomas e recursos populares de pesquisa, como destaques, autopreenchimento e pesquisa geoespacial. Para implementar o Amazon CloudSearch, acesse o console AWS e crie um novo domínio de pesquisa. Configure o domínio definindo tipo e capacidade. Defina o esquema de dados, especifique os campos a serem indexados e carregue seus dados. Ajuste as opções de pesquisa, como facetas e relevância, e crie o endpoint. Configure a segurança para controlar o acesso e, finalmente, monitore o desempenho ajustando as configurações conforme necessário.

---

## Pergunta 28

Um líder técnico precisa identificar o usuário responsável pela exclusão de um bucket no S3. Qual serviço possibilita esse tipo de verificação?

- AWS Systems Manager Parameter Store
    - O AWS Systems Manager Parameter Store é um serviço seguro para armazenar e gerenciar informações de configuração e segredos, como strings de conexão de banco de dados, senhas e outros valores de configuração.

- **✅** AWS CloudTrail
    - O AWS CloudTrail é um serviço de auditoria e monitoramento que registra eventos de atividade em sua conta da AWS. Ele pode ser usado para rastrear quem deletou um bucket do Amazon S3 ao registrar as ações realizadas por usuários.

- O AWS Trusted Advisor
    - O AWS Trusted Advisor é um serviço que oferece recomendações personalizadas para otimizar a infraestrutura da AWS. Ele analisa as contas e recursos em busca de oportunidades para melhorar segurança, reduzir custos, aumentar a performance, melhorar a tolerância a falhas e otimizar o uso de serviços, ajudando a alinhar a utilização da AWS às melhores práticas.

- AWS IAM
    - O AWS IAM gerencia permissões de acesso a recursos da AWS, permitindo ou restringindo ações específicas. No entanto, não controla as ações específicas que os usuários realizam dentro desses recursos. Para monitorar e registrar essas ações, são necessários serviços adicionais como o AWS CloudTrail.

> **Explicação geral**:  
> O AWS CloudTrail é um serviço de auditoria e monitoramento que registra eventos de atividade em sua conta da AWS. Ele pode ser usado para rastrear quem deletou um bucket do Amazon S3 ao registrar as ações realizadas por usuários, incluindo operações de criação, modificação ou exclusão de recursos. Ao habilitar o CloudTrail, você pode acessar os logs de eventos para analisar as ações específicas realizadas e identificar o autor da ação de exclusão do bucket. Isso ajuda a rastrear e auditar atividades, melhorando a segurança e a conformidade na nuvem.

---

## Pergunta 29

Você precisa permitir que os seus clientes acessem a sua aplicação web através de um domínio amigável com o nome da sua empresa. Como isso pode ser implementado?

- Com o registro no ACL
    - Uma ACL (Access Control List) é uma camada opcional de segurança na AWS que pode ser configurada como um firewall para uma Virtual Private Cloud (VPC). Ela permite definir regras de controle de tráfego de entrada e saída para sub-redes dentro da VPC, oferecendo um nível adicional de proteção e controle sobre o acesso à sua rede.

- **✅** Com o registro no Route53
    - Para permitir que seus clientes acessem sua aplicação web através de um domínio amigável, registre um nome de domínio e configure o DNS usando o Amazon Route 53. O Route 53 permite associar seu domínio personalizado ao endpoint da sua aplicação. Isso direciona o tráfego para sua aplicação web usando um endereço fácil de lembrar.

- Com o registro no ELB
    - O Elastic Load Balancing distribui automaticamente o tráfego de entrada de aplicações entre diversos destinos, como instâncias do Amazon EC2, contêineres, endereços IP, funções do Lambda e dispositivos virtuais.

- Com o registro no AWS Auto Scaling
    - O AWS Auto Scaling monitora os aplicativos e ajusta automaticamente a capacidade para manter um desempenho constante e previsível pelo menor custo possível.

> **Explicação geral**:  
> Você pode registrar um domínio diretamente no Amazon Route 53, que oferece um processo simples e integrado para registrar e gerenciar domínios. Se você comprar um domínio através de outros registradores, como o Registro.br, pode usá-lo com o Route 53 configurando os servidores de nomes fornecidos pelo Route 53 no painel do registrador. Isso permite que você mantenha a gestão de DNS e outros serviços relacionados ao domínio no Route 53, aproveitando suas funcionalidades de escalabilidade e integração com outros serviços da AWS.

---

## Pergunta 30

Uma empresa mantém arquivos contendo dados financeiros em um bucket do S3. Como é viável consultar informações nestes arquivos utilizando a linguagem SQL?

- Com o EMR
    - O EMR é a plataforma para uso de Big Data.

- Com o Amazon Query Analyzer
    - Este serviço não existe.

- Com o Amazon Elastic Search
    - O Amazon Elasticsearch é um serviço totalmente gerenciado com o qual você pode pesquisar, analisar e visualizar seus dados de log de maneira econômica, em escala de petabytes.

- **✅** Com o Athena
    - O Amazon Athena é um serviço de análise interativo que permite consultar e analisar grandes volumes de dados armazenados no Amazon S3 usando a linguagem SQL padrão.

> **Explicação geral**:  
> O Amazon Athena é um serviço de análise interativo que permite consultar e analisar grandes volumes de dados armazenados no Amazon S3 usando a linguagem SQL padrão. Ele elimina a necessidade de configuração de infraestrutura e pré-processamento de dados, permitindo que os usuários executem consultas diretamente nos dados brutos. Usando a linguagem SQL, os usuários podem escrever consultas SELECT, JOINs, filtros e agregações para extrair insights dos dados. O Athena processa consultas sob demanda e retorna resultados quase em tempo real, tornando a análise de big data mais acessível e ágil.

---

## Pergunta 31

Uma empresa deseja capturar e enviar todas as interações dos usuários em um site, utilizando esses dados para gerar insights em tempo real para campanhas de vendas. Qual serviço pode ser empregado para esse tipo de transmissão de dados em tempo real?

- Amazon SQS
    - O Amazon Simple Queue Service é um serviço de filas de mensagens gerenciado que permite o desacoplamento e a escalabilidade de microsserviços, sistemas distribuídos e aplicações sem servidor.

- **✅** Amazon Kinesis
    - O Amazon Kinesis facilita a coleta, o processamento e a análise de dados de streaming em tempo real, permitindo que você obtenha insights oportunos e reaja rapidamente às novas informações.

- Amazon EventBridge
    - O Amazon EventBridge é um barramento de eventos sem servidor que torna mais fácil a criação de aplicações orientadas por eventos em escala usando eventos gerados com base em suas aplicações, aplicações integradas de software como serviço (SaaS) e serviços da AWS.

- Amazon SNS
    - O Amazon Simple Notification Service é um serviço de mensagens totalmente gerenciado para a comunicação de aplicação para aplicação (A2A) e de aplicação para pessoa (A2P). A funcionalidade pub/sub de A2A fornece tópicos para sistemas de mensagens de alta taxa de transferência baseados em push e de muitos para muitos entre sistemas distribuídos, microsserviços e aplicativos sem servidor orientados por eventos.

> **Explicação geral**:  
> O Amazon Kinesis facilita a coleta, o processamento e a análise de dados de streaming em tempo real, permitindo que você obtenha insights oportunos e reaja rapidamente às novas informações. O Amazon Kinesis oferece recursos essenciais para processar dados de streaming em qualquer escala de forma econômica, além da flexibilidade de escolher as ferramentas mais adequadas aos requisitos dos aplicativos. Com o Amazon Kinesis, você pode consumir dados em tempo real como vídeo, áudio, logs de aplicativos, clickstreams de sites e dados de telemetria de IoT para machine learning, análises e outros aplicativos. O Amazon Kinesis permite processar e analisar dados assim que são recebidos e responder instantaneamente, em vez de aguardar a conclusão da coleta de dados para poder iniciar o processamento.

---

## Pergunta 32

Uma empresa planeja migrar para a AWS diversas aplicações com requisitos computacionais variáveis. Que serviço deve ser empregado para executar essas aplicações?

- EBS
    - EBS é o serviço utilizado como armazenamento para diversas funcionalidades em complemento ao EC2, como instalação de banco de dados IaaS, entre outras.

- **✅** EC2
    - O Amazon EC2 (Elastic Compute Cloud) é um serviço de computação em nuvem da AWS que oferece instâncias de máquinas virtuais escaláveis, permitindo aos usuários executar diversos tipos de cargas de trabalho. Existem diversos tipos de instâncias EC2, cada um otimizado para diferentes casos de uso. Isso inclui instâncias de propósito geral, otimizadas para computação, memória, armazenamento e GPU.

- EFS
    - O EFS é o Elastic File System que pode ser utilizado para fornecer sistema de arquivos para uma ou mais instâncias EC2.

- S3
    - O S3 é o serviço padrão para armazenar arquivos e metadados como objetos em buckets.

> **Explicação geral**:  
> O Amazon EC2 (Elastic Compute Cloud) é um serviço de computação em nuvem da AWS que oferece instâncias de máquinas virtuais escaláveis, permitindo aos usuários executar diversos tipos de cargas de trabalho. Existem diversos tipos de instâncias EC2, cada um otimizado para diferentes casos de uso. Isso inclui instâncias de propósito geral, otimizadas para computação, memória, armazenamento e GPU. As instâncias EC2 são adequadas para hospedar aplicativos, websites, bancos de dados, análises, processamento de dados e muito mais. Elas podem ser usadas para escalabilidade vertical (aumentando a capacidade de uma instância) ou escalabilidade horizontal (aumentando o número de instâncias), de acordo com as necessidades da carga de trabalho. A variedade de tipos de instâncias EC2 permite aos usuários selecionar a configuração ideal para maximizar o desempenho e minimizar os custos, adaptando-se às diferentes demandas de aplicativos e cenários.

---

## Pergunta 33

Uma empresa almeja hospedar todas as suas aplicações em plataformas sem servidores. Levando em conta a necessidade de persistência de dados, qual serviço deve ser empregado na solução?

- EC2
    - O Amazon EC2 (Elastic Compute Cloud) é um serviço de computação em nuvem da AWS que permite aos usuários criar e gerenciar instâncias de servidores virtuais escaláveis. Ele oferece flexibilidade na escolha de recursos como CPU, memória e armazenamento, facilitando a execução de aplicativos na nuvem. Em conjunto com o EBS, pode ser utilizado para a instalação de qualquer banco de dados no modelo IaaS com servidor.

- MySQL
    - MySQL é um sistema de gerenciamento de banco de dados relacional de código aberto. Ele é amplamente utilizado para armazenar, organizar e recuperar dados em uma variedade de aplicativos, desde sites a grandes sistemas corporativos. Pode ser utilizado pelo RDS ou instalado no EC2.

- RDS - MariaDB
    - MariaDB é um sistema de gerenciamento de banco de dados relacional de código aberto, derivado do MySQL. Ele é utilizado para armazenar e gerenciar grandes volumes de dados em servidores, oferecendo alta performance, escalabilidade e suporte a múltiplos tipos de dados e operações SQL.

- **✅** DynamoDB
    - O Amazon DynamoDB é um banco de dados de chave-valor NoSQL, sem servidor e totalmente gerenciado, projetado para executar aplicações de alta performance em qualquer escala.

> **Explicação geral**:  
> O Amazon DynamoDB é ideal para aplicações sem servidores (serverless) porque é um banco de dados NoSQL gerenciado que escala automaticamente para acomodar a carga de trabalho, sem necessidade de gerenciamento de servidores ou provisionamento de capacidade. O Amazon Aurora também suporta essa capacidade quando configurado como Aurora Serverless, permitindo que o banco de dados escale automaticamente com base na demanda, oferecendo uma solução flexível e econômica para cargas de trabalho variáveis.

---

## Pergunta 34

Uma organização pretende disponibilizar aplicativos SaaS e ambientes de trabalho virtual para seus usuários finais. Como o AWS AppStream 2.0 pode ser uma contribuição significativa nesse contexto?

- **✅** Fornecendo streaming de aplicativos.
    - O AWS AppStream 2.0 é um serviço projetado para fornecer streaming de aplicativos na nuvem. Ele permite a execução de aplicativos de desktop na nuvem, transmitindo a saída para dispositivos dos usuários, garantindo uma experiência consistente em diversos dispositivos e sistemas operacionais.

- Armazenando dados na nuvem.
    - Armazenar dados na nuvem é um objetivo do Amazon S3 ou do Amazon EBS.

- Gerenciando servidores de banco de dados.
    - Gerenciar servidores de banco de dados é uma tarefa realizada com serviços como o Amazon RDS ou o Amazon DynamoDB.

- Hospedando sites da web.
    - Hospedar sites da web é um caso de uso relacionado ao Amazon EC2, S3, LigthSail.

> **Explicação geral**:  
> O AWS AppStream 2.0 é um serviço do AWS End User Computing (EUC) projetado para fornecer streaming de aplicativos na nuvem. Ele permite a execução de aplicativos de desktop na nuvem, transmitindo a saída para dispositivos dos usuários, garantindo uma experiência consistente em diversos dispositivos e sistemas operacionais. Além disso, o AppStream 2.0 pode ser configurado para transmitir aplicativos SaaS ou oferecer áreas de trabalho virtuais com persistência seletiva. Isso significa que as configurações e arquivos das aplicações podem persistir entre as sessões dos usuários, proporcionando uma experiência personalizada e produtiva em cada login.

---

## Pergunta 35

Sua empresa adotou o Step Function para orquestrar funções sem servidor para realizar análise de fraudes. Uma vez que o código das funções estejam construídos e testados, qual serviço deve ser implementado para executar tais funções na plataforma?

- **✅** AWS Lambda
    - Para executar as funções sem servidor na plataforma AWS após a construção e teste do código, você deve implementar o AWS Lambda. O AWS Lambda se integra com o AWS Step Functions para executar suas funções em resposta a eventos, permitindo orquestrar e automatizar o processamento de tarefas de negócio como a análise de fraudes.

- Amazon EC2
    - O Amazon EC2 (Elastic Compute Cloud) é um serviço que fornece capacidade de computação escalável na nuvem. Ele permite criar e gerenciar instâncias virtuais de servidores, chamadas de instâncias, oferecendo controle sobre o sistema operacional, a configuração e o software.

- Amazon Athena
    - O Amazon Athena é um serviço de consultas interativas que permite analisar dados armazenados no Amazon S3 usando SQL padrão. Ele é sem servidor e cobra apenas pelas consultas realizadas, facilitando a análise de grandes volumes de dados sem a necessidade de provisionar infraestrutura.

- Amazon ECS
    - O Amazon ECS (Elastic Container Service) é um serviço gerenciado para orquestrar e executar contêineres Docker. Ele permite gerenciar a implantação, escalabilidade e operação de contêineres em clusters de instâncias EC2 ou utilizando AWS Fargate, que gerencia a infraestrutura subjacente.

> **Explicação geral**:  
> O AWS Lambda é adequado para executar funções sem servidor orquestradas pelo AWS Step Functions porque oferece um ambiente que escala automaticamente, ideal para tarefas rápidas e independentes. Ele permite executar código sem gerenciar servidores e cobra apenas pelo tempo de execução, tornando-o eficiente para funções que são parte de workflows mais complexos gerenciados pelo Step Functions. Isso facilita a criação de workflows escaláveis e de baixo custo, com cada função Lambda focada em uma tarefa específica dentro do processo.

---

## Pergunta 36

Uma empresa deseja implantar uma rede social interna que facilite a conexão entre os colaboradores por meio de grafos. Qual banco de dados, totalmente gerenciado pela AWS, seria adequado para realizar essa implementação?

- Amazon Graph
    - Atualmente, não existe um serviço específico chamado "Amazon Graph" na AWS. O termo "graph" geralmente se refere a um tipo de banco de dados ou modelo de dados que armazena informações em estruturas de grafos, facilitando a modelagem de relações complexas entre dados.

- Amazon JanusGraph
    - Amazon JanusGraph não existe; entretanto, o "JanusGraph" é um banco de dados em grafo amplamente utilizado que pode ser instalado em instâncias EC2 na AWS e gerenciado pelo cliente. Isso significa que o cliente é responsável pela configuração, manutenção e gerenciamento do banco de dados e da infraestrutura subjacente.

- **✅** Amazon Neptune
    - O Amazon Neptune é um serviço de banco de dados de grafos rápido, confiável e totalmente gerenciado que facilita a criação e a execução de aplicativos com muitas conexões entre os diversos elementos existentes.

- Amazon Neo4j
    - O Amazon Neo4j não existe; entretanto, o "Neo4j" é um banco de dados em grafo amplamente utilizado que pode ser instalado em instâncias EC2 na AWS e gerenciado pelo cliente. Isso significa que o cliente é responsável pela configuração, manutenção e gerenciamento do banco de dados e da infraestrutura subjacente.

> **Explicação geral**:  
> O Amazon Neptune é um serviço de banco de dados de grafos rápido, confiável e totalmente gerenciado que facilita a criação e a execução de aplicativos com muitas conexões entre os diversos elementos existentes. Ele é utilizado para modelar e consultar relações complexas entre dados, sendo útil em cenários como redes sociais, análise de fraudes, recomendações personalizadas e detecção de padrões em dados interconectados. Neptune é adequado para casos em que a estrutura de dados é altamente relacional e exige consultas complexas para explorar as interações entre os elementos.

---

## Pergunta 37

Considerando o uso de tags associadas aos serviços e recursos da AWS, qual das seguintes descrições NÃO representa uma função aplicável para tags?

- Organização e categorização de recursos
    - Tags são amplamente utilizadas para organizar e categorizar recursos de acordo com diferentes critérios, como departamento, projeto ou ambiente. Isso facilita o gerenciamento e a busca de recursos específicos na AWS.

- Atribuição de custos e criação de relatórios de faturamento
    - Tags permitem a atribuição de custos a diferentes projetos ou departamentos, ajudando a criar relatórios detalhados de faturamento e a analisar despesas de forma granular.

- **✅** Gerenciamento de permissões e controle de acesso
    - Tags não gerenciam permissões nem controlam o acesso diretamente. A gestão de permissões e acesso é realizada através do AWS Identity and Access Management (IAM) e suas políticas, não por tags.

- Automatização de backups de recursos
    - Tags não são diretamente usadas para automatizar backups de recursos. Embora possam ajudar a identificar recursos para backups, a automação de backups geralmente é gerenciada por outros serviços, como o AWS Backup.

> **Explicação geral**:  
> Uma etiqueta (tag) na AWS é um rótulo composto por uma chave e um valor associados a recursos, como instâncias EC2, buckets S3 e volumes EBS. A estrutura é simples: uma chave identifica o tipo de informação e um valor fornece detalhes adicionais. Por exemplo, uma tag pode ter a chave "Departamento" e o valor "Financeiro". As tags são usadas para organizar, categorizar e gerenciar recursos, permitindo a aplicação de políticas de custo, a criação de relatórios e a automação de processos. Elas também ajudam a filtrar recursos em grandes ambientes e a aplicar práticas de governança.

---

## Pergunta 38

Durante uma migração de banco de dados para a AWS, a equipe encarregada identificou a necessidade de transferir dados de um banco Oracle on-premises para um banco Oracle no RDS. Como esse procedimento pode ser executado?

- **✅** Implementando o AWS DMS
    - O AWS DMS - Database Migration Service é um serviço utilzado para migrar dados de bancos de dados on-premises, para uma instância de banco de dados do Amazon Relational Database Service (Amazon RDS) em qualquer um dos mecanismos de bancos de dados disponíveis no serviço, como o Oracle.

- Implementando o AWS Snow
    - O AWS Snow fornece dispositivos portáteis altamente seguros para coletar e processar dados na borda e migrar dados para dentro e fora da AWS sem utilizar conexões de rede.

- Implementando o AWS Glue
    - O AWS Glue é um serviço de integração de dados sem servidor que facilita descobrir, preparar e combinar dados para análise, machine learning e desenvolvimento da aplicação.

- Implementando o AWS Connect
    - O Amazon Connect é uma central de atendimentos baseada em IA que facilita o atendimento ao cliente através de canais como voz e chat, com baixo custo. Não deve ser confundido com o AWS Direct Connect, que oferece uma conexão de rede dedicada entre instalações locais e a AWS, reduzindo latência e melhorando a largura de banda.

> **Explicação geral**:  
> O AWS Database Migration Service (DMS) é um serviço que facilita a migração de bancos de dados para a AWS, com tempo de inatividade mínimo. Ele pode ser usado para migrar dados de sistemas on-premises para bancos de dados na AWS, incluindo Amazon RDS, Aurora, e Oracle RDS. O DMS suporta migrações homogêneas (por exemplo, Oracle para Oracle) e heterogêneas (por exemplo, Oracle para PostgreSQL), além de permitir a replicação contínua de dados para manter o banco de dados de origem e destino sincronizados durante a migração. No caso de migrações de bancos de dados NoSQL, o DMS também suporta a migração de dados de fontes como MongoDB, Cassandra, e DynamoDB.

---

## Pergunta 39

Para permitir que uma aplicação em execução em uma instância EC2 acesse um banco de dados no RDS, qual recurso do IAM deve ser criado para autorizar essa integração?

- Usuários Genéricos
    - Usuários genéricos no IAM são desaconselhados porque eles possuem credenciais estáticas (como senhas e chaves de acesso) que podem ser facilmente comprometidas e são difíceis de gerenciar e rotacionar. Além disso, usuários genéricos não permitem a aplicação de permissões temporárias ou baseadas em contexto, como fazem as funções (roles).

- Grupos
    - Grupos no IAM gerenciam permissões de usuários humanos, mas não são adequados para acessos entre aplicações ou serviços. Para esses casos, funções (roles) são usadas, pois permitem permissões temporárias e específicas para aplicações e serviços.

- Pares de Chaves (Key Pairs)
    - Key pairs, como pares de chave pública e privada, são usados principalmente para autenticação em conexões SSH e não são ideais para gerenciar acessos a serviços AWS. Eles não fornecem controle granular de permissões e não são facilmente rotacionáveis ou auditáveis.

- **✅** Funções (Roles)
    - Todos os acessos entre aplicações devem ser feitos através de uma função (role) configurada no serviço IAM. Através de uma função você associa politicas e restrições de acesso que podem ser associadas a uma ou mais aplicações para autorizar leituras e gravações aos recursos.

> **Explicação geral**:  
> No AWS Identity and Access Management (IAM), uma função (role) é um conjunto de permissões que define o que uma aplicação ou serviço pode fazer na AWS. As funções são associadas a políticas de permissões que especificam quais ações são permitidas ou negadas em recursos específicos. Quando uma aplicação precisa acessar recursos da AWS, como bancos de dados, buckets S3 ou outros serviços, ela assume uma função apropriada que lhe concede as permissões necessárias. Isso é crucial para a segurança, pois permite um controle granular sobre o que cada aplicação pode acessar, além de facilitar a aplicação de políticas de segurança e auditoria. As funções podem ser assumidas por várias aplicações ou serviços, garantindo que os acessos sejam consistentes e gerenciados centralmente, minimizando riscos de segurança.

---

## Pergunta 40

Uma aplicação web está enfrentando problemas de indisponibilidade devido a bots e automações mal-intencionadas que executam raspagens de tela, consumindo considerável parte dos recursos de infraestrutura provisionados para os usuários. Como se pode evitar efetivamente essa situação?

- Habilitando o AWS Shield
    - O AWS Shield é um serviço gerenciado de proteção contra DDoS (Negação de serviço distribuída) que protege os aplicativos executados na AWS. O AWS Shield oferece de detecção e mitigações em linha automáticas e sempre ativas que minimizam o tempo de inatividade e a latência dos aplicativos, fornecendo proteção contra DDoS sem necessidade de envolver o AWS Support.

- **✅** Habilitando o AWS WAF
    - O AWS WAF é um firewall de aplicações Web que ajuda a proteger suas aplicações Web ou APIs contra bots e exploits comuns na Web que podem afetar a disponibilidade, comprometer a segurança ou consumir recursos em excesso.

- Habilitando o AWS Certificate Manager
    - O AWS Certificate Manager é um serviço que permite provisionar, gerenciar e implantar facilmente certificados Secure Sockets Layer (SSL)/Transport Layer Security (TLS) para uso com os serviços da AWS e os recursos internos conectados.

- Habilitando o AWS CloudFront
    - O Amazon CloudFront é um serviço rápido de rede de entrega de conteúdo (CDN) que entrega dados, vídeos, aplicações e APIs a clientes em todo o mundo com segurança, baixa latência e altas velocidades de transferência em um ambiente de uso facilitado para desenvolvedores.

> **Explicação geral**:  
> O AWS WAF (Web Application Firewall) é um serviço que protege suas aplicações web e APIs contra ameaças e vulnerabilidades comuns na web, como SQL injection e cross-site scripting (XSS). Ele permite criar regras personalizadas para filtrar e bloquear tráfego indesejado, além de fornecer proteção contra bots maliciosos. O WAF ajuda a preservar a disponibilidade da aplicação e a proteger os recursos contra abusos que possam comprometer a segurança ou consumir recursos de forma excessiva. Integrado com o Amazon CloudFront e o Application Load Balancer, ele oferece proteção escalável e eficiente.

---

## Pergunta 41

Como o AWS IoT Core utiliza múltiplos mecanismos de segurança para assegurar a integridade e confidencialidade das comunicações entre dispositivos IoT e a nuvem?

- O AWS IoT Core exige que todos os dispositivos estejam na mesma rede virtual privada (VPC) para garantir a segurança das comunicações.
    - O AWS IoT Core pode operar com dispositivos em diferentes redes e utiliza criptografia e certificados para garantir a segurança, sem exigir que todos os dispositivos estejam na mesma VPC.

- O AWS IoT Core utiliza apenas autenticação baseada em IP e não usa certificados para autenticar dispositivos.
    - O AWS IoT Core utiliza certificados digitais para autenticação mútua, garantindo que tanto os dispositivos quanto a nuvem possam verificar a identidade um do outro, enquanto a autenticação baseada em IP não é utilizada.

- O AWS IoT Core usa apenas criptografia simétrica para proteger dados em trânsito e não realiza autenticação dos dispositivos.
    - O AWS IoT Core usa criptografia TLS (que é uma forma de criptografia assimétrica) para proteger dados em trânsito e realiza autenticação mútua usando certificados digitais.

- **✅** O AWS IoT Core utiliza certificados de dispositivo para autenticação mútua, criptografia TLS para proteger dados em trânsito e políticas de acesso baseadas em identidade para controlar o acesso e garantir a segurança das comunicações entre dispositivos e a nuvem.
    - Estes são os múltiplos mecanismos de segurança utilizados pelo serviço.

> **Explicação geral**:  
> O AWS IoT Core utiliza uma combinação de medidas para garantir a segurança das comunicações entre dispositivos IoT e a nuvem. Certificados de dispositivo são usados para autenticação mútua, garantindo que apenas dispositivos autorizados possam se conectar à nuvem e que a nuvem possa autenticar os dispositivos. Criptografia TLS protege os dados em trânsito, assegurando que as informações transmitidas entre os dispositivos e a nuvem sejam criptografadas e, portanto, protegidas contra interceptação e adulteração. Políticas de acesso baseadas em identidade controlam quais ações e recursos cada dispositivo pode acessar, garantindo que apenas os dispositivos e usuários autorizados possam executar operações específicas. Juntas, essas medidas asseguram a integridade, confidencialidade e segurança das comunicações no ambiente IoT.

---

## Pergunta 42

Uma empresa necessita realizar monitoramento da saúde dos serviços de infraestrutura de uma aplicação crítica para poder emitir alertas diante de eventuais problemas. Qual seria a melhor forma de implementar esse procedimento?

- **✅** Com métricas e alarmes do CloudWatch
    - Uma empresa pode usar o Amazon CloudWatch para monitorar a saúde dos serviços de infraestrutura de aplicações críticas.

- Com métricas e alarmes do AWS Budgets
    - O AWS Budget é utilizado para definir orçamentos para limites de uso de serviços da AWS.

- Com métricas e alarmes do WAF
    - O AWS Web Application Firewall (WAF) é um serviço que protege aplicações web contra ataques comuns na web, como injeção de SQL e scripts entre sites (XSS).

- Com métricas e alarmes do CloudTrail
    - O CloudTrail é utilizado para logar ações de usuários em APIs de serviços da AWS.

> **Explicação geral**:  
> Uma empresa pode usar o Amazon CloudWatch para monitorar a saúde dos serviços de infraestrutura da aplicação crítica. Primeiro, configure métricas relevantes, como CPU, uso de memória e latência. Em seguida, defina alarmes no CloudWatch para detectar condições anormais. Esses alarmes podem ser configurados para acionar notificações (por exemplo, via Amazon SNS) em caso de problemas, permitindo ação rápida. Além disso, você pode criar painéis personalizados no CloudWatch para visualizar o desempenho da aplicação em tempo real e histórico. Isso ajuda a garantir a disponibilidade e o desempenho da aplicação crítica, identificando problemas e permitindo respostas proativas.

---

## Pergunta 43

Para implementar um processo de escalonamento automático de instâncias EC2, um analista de operações precisa definir o sistema operacional, os softwares e as configurações necessárias para cada inclusão de uma nova instância no processo. Qual abordagem pode ser adotada para operacionalizar esse processo?

- Utilização de uma imagem no Amazon Image.
    - Este serviço não existe.

- **✅** Utilização de uma imagem no AMI.
    - Ele pode criar Amazon Machine Images (AMIs) que incluem o sistema operacional, os softwares e as configurações necessárias para as instâncias. Quando o escalonamento automático ocorre, novas instâncias são lançadas a partir dessas AMIs, garantindo que todas as instâncias tenham a configuração desejada. Essa abordagem simplifica a administração e garante consistência nas configurações das instâncias.

- Utilização de uma imagem no ECR.
    - O Amazon Elastic Container Registry (ECR) é um serviço da AWS que permite armazenar, gerenciar e implantar imagens de contêineres Docker de maneira segura e altamente escalável na nuvem da AWS, não de instâncias EC2.

- Utilização de uma imagem no IAM.
    - O AWS Identity and Access Management (IAM) permite que você gerencie com segurança o acesso aos serviços e recursos da AWS. Usando o IAM, você pode criar e gerenciar usuários e grupos da AWS e usar permissões para conceder e negar acesso a recursos da AWS.

> **Explicação geral**:  
> Uma Imagem de Máquina da Amazon (AMI) é um template que inclui o sistema operacional, aplicativos e configurações necessárias para iniciar uma instância EC2. Ao lançar uma instância, você especifica uma AMI para definir seu ambiente e configuração. Usar a mesma AMI permite criar várias instâncias com a mesma configuração, garantindo consistência. Para diferentes configurações, você pode usar AMIs distintas. AMIs podem ser personalizadas ou usadas conforme fornecidas pela AWS. Elas simplificam a criação e o gerenciamento de instâncias, facilitando a escalabilidade e a padronização dos ambientes.

---

## Pergunta 44

Para manter a infraestrutura de uma aplicação elástica e balanceada, quais serviços devem ser utilizados? (Escolha 2 alternativas)

- CloudFront
    - O Amazon CloudFront é um serviço rápido de rede de entrega de conteúdo (CDN) que entrega dados, vídeos, aplicações e APIs a clientes em todo o mundo com segurança, baixa latência e altas velocidades de transferência em um ambiente de uso facilitado para desenvolvedores.

- CloudFormation
    - O AWS CloudFormation oferece uma forma fácil de modelar uma coleção de recursos relacionados da AWS e de terceiros, provisioná-la com rapidez e consistência e gerenciar todo o seu ciclo de vida mediante o tratamento da infraestrutura como código.

- ElastiCache
    - O Amazon ElastiCache é um serviço de memória rápida utilizado para armazenar dados em cachê é atender as mais diversas necessidades de solução.

- **✅** ELB
- **✅** ASG

> **Explicação geral**:  
> O Auto Scaling Group (ASG) e o Elastic Load Balancer (ELB) trabalham juntos para escalar uma aplicação e distribuir a carga de forma eficiente. O ASG ajusta automaticamente o número de instâncias EC2 com base em políticas de escalabilidade, como a carga de CPU ou a quantidade de requisições. Quando novas instâncias são adicionadas ou removidas, o ELB distribui o tráfego de forma equilibrada entre todas as instâncias saudáveis, garantindo alta disponibilidade e desempenho. Assim, o ASG lida com a elasticidade da aplicação, enquanto o ELB gerencia a distribuição de carga, assegurando que o serviço permaneça estável e responsivo.

---

## Pergunta 45

Um time de desenvolvimento deseja supervisionar as atividades de projetos desde a concepção até a entrega do software na plataforma, além de utilizar modelos pré-definidos de projetos na linguagem de programação que utilizam. Que serviço possibilita esse nível de facilitação?

- AWS CodeBuild
    - O AWS CodeBuild é utilizado para compilar e testar o aplicativo na esteira.

- AWS CodeCommit
    - O AWS CodeCommit é utilizado para fazer o gerenciamento de código fonte do aplicativo.

- **✅** AWS CodeStar
    - O AWS CodeStar é um serviço da Amazon Web Services (AWS) projetado para simplificar e acelerar o processo de desenvolvimento de software. Ele facilita a integração de várias ferramentas essenciais para o desenvolvimento, como ambientes de desenvolvimento integrado (IDEs), pipelines de integração contínua/entrega contínua (CI/CD) e ferramentas de gerenciamento de projetos. Com o CodeStar, os desenvolvedores podem configurar rapidamente um ambiente de desenvolvimento completo, permitindo que eles se concentrem na criação de software em vez de lidar com a configuração e integração de várias ferramentas.

- AWS CodeDeploy
    - O AWS CodeDeploy é utilizado para fazer a implantação do aplicativo na AWS ou em ambientes on-premisses.

> **Explicação geral**:  
> O AWS CodeStar é um serviço da Amazon Web Services (AWS) projetado para simplificar e acelerar o processo de desenvolvimento de software. Ele facilita a integração de várias ferramentas essenciais para o desenvolvimento, como ambientes de desenvolvimento integrado (IDEs), pipelines de integração contínua/entrega contínua (CI/CD) e ferramentas de gerenciamento de projetos. Com o CodeStar, os desenvolvedores podem configurar rapidamente um ambiente de desenvolvimento completo, permitindo que eles se concentrem na criação de software em vez de lidar com a configuração e integração de várias ferramentas. Além disso, o AWS CodeStar fornece modelos predefinidos em várias linguagens de programação, como Java, Python, Node.js, entre outras. Esses modelos contêm configurações pré-definidas para estruturas de projeto comuns, bibliotecas e ferramentas, o que ajuda a acelerar o processo de desenvolvimento, permitindo que os desenvolvedores comecem a trabalhar em seus aplicativos rapidamente, sem precisar configurar tudo do zero. Em resumo, o AWS CodeStar é uma plataforma abrangente que simplifica e agiliza todo o ciclo de vida do desenvolvimento de software na nuvem da AWS.

---

## Pergunta 46

O time de desenvolvedores da sua empresa criou uma aplicação em Java e gostaria de disponibilizá-la na AWS. Uma vez que o time não possua muito conhecimento sobre resiliência, balanceadores de carga, monitoramento e outras questões de infraestrutura, qual serviço poderá ajudá-los?

- **✅** AWS ElasticBeanStalk
    - Com o AWS Elastic Beanstalk, é possível implantar e gerenciar rapidamente aplicações na Nuvem AWS sem precisar se preocupar com a infraestrutura que executa essas aplicações. O AWS Elastic Beanstalk reduz a complexidade do gerenciamento sem restringir as opções ou o controle. Basta fazer upload da sua aplicação e o AWS Elastic Beanstalk automaticamente gerencia os detalhes de provisionamento de capacidade, balanceamento de carga, escalabilidade e monitoramento da integridade da aplicação.

- AWS Fargate
    - O AWS Fargate é um mecanismo de computação sem servidor para contêineres.

- AWS ECS
    - O Amazon Elastic Container Service (Amazon ECS) é um serviço totalmente gerenciado de orquestração de contêineres que ajuda a implantar, gerenciar e escalar facilmente aplicações conteinerizadas.

- AWS CodeDeploy
    - O AWS CodeDeploy é um serviço totalmente gerenciado de implantação que automatiza implantações de software em diversos serviços de computação como Amazon EC2, AWS Fargate, AWS Lambda e servidores locais.

> **Explicação geral**:  
> O AWS Elastic Beanstalk é um serviço de PaaS que facilita a implantação e o gerenciamento de aplicações na AWS sem a necessidade de gerenciar a infraestrutura. Após o upload do código da aplicação, o Elastic Beanstalk cuida do provisionamento de capacidade, balanceamento de carga, escalabilidade e monitoramento da integridade. Ele ajusta automaticamente o número de instâncias EC2 conforme a demanda e oferece monitoramento integrado da saúde da aplicação. Embora simplifique o gerenciamento, ainda permite controle sobre a configuração e personalização do ambiente. O Elastic Beanstalk suporta diversas linguagens e frameworks, proporcionando flexibilidade no desenvolvimento de aplicações.

---

## Pergunta 47

Uma equipe necessita armazenar os dados de uma aplicação em bancos de dados. Esses dados não seguem uma estrutura específica e estão associados a uma chave única de identificação. Qual serviço pode ser implementado para atender a essa demanda?

- **✅** Amazon DynamoDB
    - O Amazon DynamoDB é um banco de dados de chave-valor NoSQL, sem servidor e totalmente gerenciado, projetado para executar aplicações de alta performance em qualquer escala.

- Amazon Aurora
    - Amazon Aurora não é um banco de dados de chave-valor porque é um banco de dados relacional, que utiliza tabelas para armazenar dados estruturados com esquemas predefinidos, suportando consultas SQL complexas e transações ACID.

- Amazon RDS - MySql
    - O MySQL é um banco de dados relacional, não de chave-valor, que organiza dados em tabelas estruturadas e permite a execução de consultas SQL, suportando integridade referencial e transações ACID.

- Amazon KeySpaces
    - Amazon Keyspaces é baseado em um modelo de dados NoSQL de colunas largas, semelhante ao Apache Cassandra, que permite armazenar e consultar grandes volumes de dados distribuídos horizontalmente. Em um banco de dados de colunas largas, cada linha pode conter um número diferente de colunas, e as colunas podem ser agrupadas em "famílias de colunas". Isso permite armazenar grandes volumes de dados de forma eficiente e flexível, com a capacidade de adicionar ou remover colunas sem afetar outras linhas, facilitando a adaptação a dados de formatos variáveis.

> **Explicação geral**:  
> O Amazon DynamoDB é um banco de dados NoSQL de chave-valor e sem servidor, ideal para aplicações que requerem alta performance e baixa latência em qualquer escala. Ele é totalmente gerenciado, o que significa que a AWS cuida da administração de servidores, atualizações de software e escalabilidade. Além disso, oferece recursos avançados como segurança integrada, backups contínuos, replicação multirregional automatizada, armazenamento em cache na memória e ferramentas de exportação de dados. Por exemplo, para armazenar informações de clientes, você pode usar o CPF como chave e um objeto JSON como valor, onde os dados podem variar de forma não estruturada entre os registros, permitindo flexibilidade na forma de armazenar e acessar informações específicas de cada cliente. Isso elimina a necessidade de criar novas tabelas ou colunas para adicionar novos atributos, como seria necessário em um banco de dados relacional, tornando o DynamoDB ideal para aplicações com dados dinâmicos e em constante evolução.

## Pergunta 48

A área de Business Intelligence (BI) de uma organização tem a necessidade de fazer o cruzamento de dados estruturados e semi-estruturados para produzir insights para uma campanha de vendas. Que serviço pode ser empregado para essa finalidade?

- Amazon Kinesis
    - É um serviço da AWS projetado para facilitar a ingestão, processamento e análise de grandes volumes de dados em tempo real. O Amazon Kinesis oferece diferentes serviços, como Kinesis Data Streams para streaming de dados em tempo real, Kinesis Data Firehose para carregamento direto de dados em serviços da AWS e Kinesis Data Analytics para análise em tempo real de dados de streaming. Ele é frequentemente utilizado para construir soluções de análise em tempo real, processamento de logs, detecção de anomalias, entre outros casos de uso.

- Amazon EMR
    - É uma plataforma de Big Data da AWS que permite processar grandes volumes de dados de forma distribuída. O EMR utiliza frameworks como Apache Hadoop, Apache Spark e Presto para realizar análises de dados em larga escala. Ele facilita a configuração, o provisionamento e o gerenciamento de clusters de computação para processamento de dados.

- **✅** Amazon RedShift
    - O serviço do Amazon Redshift gerencia todo o trabalho de configuração, operação e escalabilidade de um data warehouse. Essas tarefas incluem capacidade de provisionamento, monitoramento e backup do cluster e aplicação de patches e atualizações ao mecanismo Amazon Redshift.

- Amazon QuickSight
    - O Amazon QuickSight é uma ferramenta de visualização e análise de dados que permite criar painéis interativos e relatórios. Ele se integra a várias fontes de dados, oferece recursos de análise avançada e visualização de dados, e é projetado para ser escalável e acessível para diversos tipos de usuários e organizações.

> **Explicação geral**:  
> O serviço do Amazon Redshift gerencia todo o trabalho de configuração, operação e escalabilidade de um data warehouse. Essas tarefas incluem capacidade de provisionamento, monitoramento e backup do cluster e aplicação de patches e atualizações ao mecanismo Amazon Redshift. Ao usar o Amazon Redshift, as equipes podem obter insights valiosos das campanhas, pois podem analisar grandes volumes de dados rapidamente e tomar decisões informadas com base em análises detalhadas e atualizadas. Isso contribui para a geração de insights para campanhas mais eficazes, permitindo que as empresas ajustem suas estratégias com base em dados precisos e em tempo real.

---

## Pergunta 49

Uma organização gerencia diversos produtos de forma independente em um ecossistema composto por mais de 30 contas. Como é possível agrupar e consolidar o gerenciamento de custos dessas contas?

- Definindo uma AWS CloudFormation
    - O CloudFormation é utilizado para IAC (Infraestrutura como código), onde são definidos arquivos templates com todos os serviços e configurações que se deseja implementar numa infraestrutura.

- Definindo AWS Multi Factor Authenticator
    - O MFA - Fator de Autenticação duplo, adiciona um passo a mais na autenticação dos acessos na AWS.

- Definindo um AWS Cost Explorer
    - O AWS Cost Explorer é o serviço para explorar custos que sua infraestrutura está consumindo.

- **✅** Definindo uma AWS Organizations
    - O AWS Organization é uma ferramenta essencial para a gestão eficiente de recursos na nuvem, especialmente para empresas de grande porte. Ele permite a criação de uma hierarquia organizacional flexível, na qual as contas podem ser agrupadas em diversas camadas de Organizações.

> **Explicação geral**:  
> O AWS Organization é uma ferramenta essencial para a gestão eficiente de recursos na nuvem, especialmente para empresas de grande porte. Ele permite a criação de uma hierarquia organizacional flexível, na qual as contas podem ser agrupadas em diversas camadas de Organizações. Com o AWS Organization, é possível estabelecer uma estrutura hierárquica que reflete a organização da empresa, desde unidades de negócios até departamentos específicos. Cada Organização pode conter suas próprias contas, e essas contas podem ser agrupadas em sub-Organizações conforme a necessidade. Essa abordagem oferece um alto nível de controle e visibilidade sobre os recursos da AWS, permitindo que as empresas centralizem o gerenciamento de recursos e custos. Além disso, o AWS Organization facilita a implementação de políticas de segurança e conformidade em toda a organização, garantindo que todas as contas e recursos estejam em conformidade com os padrões estabelecidos.

---

## Pergunta 50

Sua empresa precisa criar um chat interativo de alta qualidade com uma central de atendimento "omnichannel" para oferecer suporte aos seus clientes de qualquer lugar do mundo. Com qual serviço isso é possível?

- Amazon CloudFront
    - O Amazon CloudFront é um serviço utilizado para realizar o cache de arquivos em redes próximas aos usuários para melhorar a performance das aplicações.

- **✅** Amazon Connect
    - Com o Amazon Connect, você pode configurar uma central de contato em questão de minutos, e ela pode ser dimensionada para oferecer suporte a milhões de clientes.

- Amazon Cognito
    - O Amazon Cognito é um serviço para gerenciar logins, integrar com redes sociais para aplicações web e móveis.

- AWS Direct Connect
    - O AWS Direct Connect é uma conexão dedicada física para melhorar a performance de transmissão de dados na AWS.

> **Explicação geral**:  
> Com o Amazon Connect, você pode rapidamente configurar uma central de contato escalável para atender milhões de clientes e criar experiências de voz e chat interativo de alta qualidade. Ele também integra funcionalidades de inteligência artificial, como chatbots e análise de sentimentos, para melhorar a eficiência do atendimento e personalizar a interação com os clientes. Isso permite oferecer suporte omnicanal, tornando o atendimento mais eficaz e adaptado às necessidades dos clientes em qualquer lugar.

---

## Pergunta 51

O principal microsserviço de sua aplicação precisa publicar uma mensagem ao término de sua execução para que outros microsserviços de sua organização a consumam a partir da assinatura de um tópico. Qual serviço deve ser utilizado para atender essa necessidade?

- Amazon SES
    - O Amazon SES (Simple Email Service) é um serviço gerenciado de envio de e-mails que facilita o envio e recebimento de mensagens em grande escala. Ele é usado para campanhas de marketing, notificações e comunicação transacional, oferecendo escalabilidade, segurança e custo-efetividade.

- Amazon RDS
    - O Amazon Relational Database Service (Amazon RDS) facilita a configuração, a operação e a escalabilidade de bancos de dados relacionais na nuvem. O serviço oferece capacidade econômica e redimensionável e automatiza tarefas demoradas de administração, como provisionamento de hardware, configuração de bancos de dados, aplicação de patches e backups.

- Amazon EC2
    - O Amazon EC2 (Elastic Compute Cloud) fornece instâncias virtuais escaláveis para executar aplicações e serviços na nuvem. Ele permite controlar a configuração e o gerenciamento de servidores virtuais, facilitando a escalabilidade e flexibilidade.

- **✅** Amazon SNS
    - O Amazon SNS tem diversos usos possíveis na arquitetura de sistemas, a principal característica é essa função Pub/Sub que traz diversas possibilidades para o desenvolvimento das aplicações que precisam gerar mensagens ou eventos para outras consumirem e serem integradas de forma rápida através da leitura dos tópicos.

> **Explicação geral**:  
> O Amazon SNS (Simple Notification Service) é um serviço de mensagens baseado no modelo Pub/Sub que permite a publicação e assinatura de mensagens entre sistemas. Ele é amplamente utilizado para enviar notificações em tempo real e gerar eventos que podem ser consumidos por outras aplicações. Com SNS, você pode criar tópicos onde as mensagens são publicadas e assinantes podem receber essas mensagens por e-mail, SMS, ou HTTP/HTTPS. Isso facilita a integração rápida e a comunicação entre diferentes componentes e serviços dentro de uma arquitetura distribuída. Além disso, o SNS é escalável e pode lidar com grandes volumes de mensagens e assinantes simultaneamente.

---

## Pergunta 52

Uma empresa lançou uma aplicação na internet e busca orientações para otimizá-la e garantir sua segurança contínua. Qual serviço é capaz de fornecer essas recomendações, entre outras?

- Identity and Access Management
    - O IAM é utilizado para gerenciar os usuários, grupos e acessos de serviços.

- Security Group
    - O Security Group é uma camada de proteção utilizada para permitir ou negar o tráfego de dados em uma ou mais instâncias dentro de uma sub rede privada virtual da VPC.

- **✅** Trusted Advisor
    - O Trusted Advisor é um serviço oferecido pela Amazon Web Services (AWS) que fornece orientações personalizadas para otimizar o uso dos recursos da AWS e melhorar a eficiência operacional. Dependendo do plano de suporte contratado pelo cliente, o Trusted Advisor pode oferecer uma variedade de recomendações em diferentes áreas, incluindo segurança, desempenho, custo e tolerância a falhas.

- Multi Factor Authenticator
    - O MFA é utilizado para adicionar um passo a mais no processo de autenticação do usuário no acesso a conta pela console.

> **Explicação geral**:  
> O Trusted Advisor é um serviço oferecido pela Amazon Web Services (AWS) que fornece orientações personalizadas para otimizar o uso dos recursos da AWS e melhorar a eficiência operacional. Dependendo do plano de suporte contratado pelo cliente, o Trusted Advisor pode oferecer uma variedade de recomendações em diferentes áreas, incluindo segurança, desempenho, custo e tolerância a falhas. No contexto das recomendações de otimização de segurança, o Trusted Advisor examina as configurações e recursos da infraestrutura da AWS do cliente em busca de possíveis vulnerabilidades ou áreas onde a segurança possa ser melhorada. Isso pode incluir sugestões para melhorar a configuração de grupos de segurança, aplicar práticas recomendadas de gerenciamento de chaves, habilitar a autenticação multifator (MFA) para contas de usuário, entre outras medidas. Essas recomendações são valiosas para garantir que a aplicação hospedada na AWS permaneça segura e protegida contra ameaças cibernéticas, ao mesmo tempo em que ajudam a otimizar o ambiente de nuvem para melhor desempenho e eficiência geral.

---

## Pergunta 53

A infraestrutura global da AWS é composta por Regiões, Zonas de Disponibilidade e Redes de Borda. Qual destes componentes é utilizado para alocar os serviços de cache ofertados pelo CloudFront e pelo API Gateway?

- **✅** Redes de Borda
    - Redes de borda, ou "edge locations", são projetadas para aproximar serviços e dados dos usuários finais, reduzindo a latência e melhorando a performance das aplicações. Elas posicionam recursos e servidores em locais geograficamente distribuídos, próximos aos pontos de acesso dos usuários.

- Zonas de disponibilidade
    - As Zonas de Disponibilidade (AZs) não são usadas para otimização de cache como as Redes de Borda, pois são centros de dados isolados em uma região AWS projetados para alta disponibilidade e resiliência. As AZs oferecem infraestrutura para serviços de computação, armazenamento e banco de dados, mas não são especificamente projetadas para distribuir e cachear conteúdo próximo aos usuários finais.

- Virtual Private Cloud (VPC)
    - A VPC (Virtual Private Cloud) não é adequada para otimização de cache porque é uma rede virtual privada que fornece isolamento e controle sobre recursos na AWS, como instâncias EC2 e bancos de dados, dentro de uma região específica.

- Regiões
    - As Regiões AWS fornecem infraestrutura central e recursos principais, mas não são usadas para esse tipo de cache.

> **Explicação geral**:  
> Redes de borda, ou "edge networks/edge locations", são projetadas para trazer serviços e dados mais próximos dos usuários finais, reduzindo a latência e melhorando a performance das aplicações. Elas funcionam posicionando recursos e servidores em locais geograficamente distribuídos, perto dos pontos de acesso dos usuários. Essas redes são usadas para melhorar a eficiência e a experiência do usuário em serviços que exigem baixa latência, como streaming de vídeo, jogos online e aplicativos móveis. Serviços comuns hospedados em redes de borda incluem:
> - CDNs (Content Delivery Networks): Distribuem conteúdo web, como vídeos e imagens, para reduzir a carga no servidor principal e acelerar a entrega de conteúdo.
> - AWS Lambda@Edge: Permite executar funções Lambda na borda da rede para personalizar a resposta e manipular o tráfego diretamente nos pontos de presença da AWS.
> - Amazon CloudFront: Um serviço de CDN que usa a infraestrutura de borda para entregar conteúdo web com baixa latência e alta transferência de dados.
> - Amazon API Gateway: Facilita a criação, publicação e gerenciamento de APIs, utilizando a infraestrutura de borda para reduzir a latência e melhorar o desempenho das APIs ao processar solicitações mais perto dos usuários finais.
> Esses serviços ajudam a melhorar a performance, reduzir o tempo de resposta e otimizar a entrega de conteúdo e serviços para usuários em diversas localidades.

---

## Pergunta 54

Um cliente que detém uma conta na AWS deseja aprimorar a segurança dos acessos realizados por meio do Console de Gerenciamento. Qual medida pode ser adotada para alcançar esse objetivo?

- **✅** Utilizar a autenticação multifator (MFA)
    - A Autenticação Multifator (MFA) na AWS é uma camada adicional de segurança que exige múltiplos métodos de verificação para acessar contas e serviços. Ao habilitar o MFA, os usuários precisam fornecer algo que conhecem (senha) e algo que possuem (dispositivo MFA) para autenticar.

- Utilizar key pairs (par de chaves) na autenticação dos usuários
    - É uma forma de permitir a conexão SSH entre a máquina do cliente e um servidor na AWS através de um arquivo contendo chaves de segurança geradas e disponibilizadas pelos administradores da conta.

- Utilizar o Secrets Manager
    - O AWS Secrets Manager gerencia credenciais e senhas de acesso, facilitando o armazenamento e a recuperação segura de informações sensíveis, como chaves de API e senhas, para integração entre serviços e aplicativos, não senhas utilizadas para acessar o Console.

- Utilizar o KMS
    - O AWS Key Management Service (KMS) gerencia chaves de criptografia para proteger dados, facilitando a criação, armazenamento e controle de chaves de forma segura na nuvem. Ele integra-se com outros serviços da AWS para simplificar a criptografia e o gerenciamento de chaves.

> **Explicação geral**:  
> A Autenticação Multifator (MFA) na AWS é uma camada adicional de segurança que exige múltiplos métodos de verificação para acessar contas e serviços. Ao habilitar o MFA, os usuários precisam fornecer algo que conhecem (senha) e algo que possuem (dispositivo MFA) para autenticar. Isso protege os acessos ao console da AWS, tornando mais difícil para invasores obterem acesso não autorizado, mesmo que tenham a senha. A Autenticação Multi Fator deve ser habilitada com algum dispositivo de terceiros para a proteção do acesso via console. Um exemplo é o Google Authenticator, que gera um código numérico a cada minuto que deve ser utilizado no login.

---

## Pergunta 55

Uma empresa quer alocar custos de serviços por departamento, aplicar taxas personalizadas e distribuir créditos conforme o consumo compartilhado da AWS. Qual serviço permite exibir custos de forma personalizada e suporta fluxos de trabalho de cobrança e relatórios?

- AWS Organizations
    - O AWS Organizations é um serviço da AWS projetado para ajudar as empresas a gerenciar várias contas da AWS de forma centralizada. Ele permite a criação de hierarquias de contas, a aplicação de políticas de segurança e orçamento, simplificando o gerenciamento de recursos e custos em uma estrutura organizacional unificada.

- AWS Pricing Calculator
    - O AWS Pricing Calculator permite que os usuários estimem os custos de uso dos serviços da AWS com base em suas necessidades específicas de recursos, configurando cenários de implantação personalizados. Isso ajuda as empresas a planejar orçamentos, otimizar gastos e tomar decisões informadas sobre a utilização de serviços na nuvem da AWS.

- **✅** AWS Billing Conductor
    - O AWS Billing Conductor permite personalizar a alocação de custos por departamento, aplicar taxas específicas e distribuir créditos conforme o consumo. Ele facilita a gestão financeira com relatórios detalhados e regras de cobrança personalizadas.

- AWS Cost Explorer
    - O AWS Cost Explorer é uma ferramenta da AWS que oferece insights detalhados sobre os custos e o uso dos serviços na nuvem de uma conta, não de um departamento. Permite que as empresas analisem, planejem e otimizem seus gastos na plataforma AWS. Ele ajuda a tomar decisões informadas sobre alocação de recursos e redução de custos na nuvem.

> **Explicação geral**:  
> O AWS Billing Conductor é o serviço ideal para atender a essas necessidades. Ele permite personalizar a exibição de custos alocados por departamento, aplicar taxas de cobrança específicas e distribuir créditos conforme o consumo de cada unidade. Com o AWS Billing Conductor, você pode mapear contas para grupos de cobrança exclusivos e definir regras de preços e itens personalizados para cada grupo. Isso facilita a gestão financeira interna e a alocação precisa de custos, fornecendo relatórios detalhados e adaptados à lógica comercial da empresa. A personalização das taxas e a distribuição de créditos ajudam a manter a transparência e o controle financeiro dentro da organização. Suponha que uma empresa tenha uma infraestrutura compartilhada na AWS, incluindo servidores, armazenamento e banco de dados, acessados pelos departamentos financeiro, recursos humanos e marketing. O AWS Billing Conductor personalizará a exibição de custos alocados para cada um destes departamentos.

---

## Pergunta 56

O cientista de dados de uma empresa tem a necessidade de preparar, construir, treinar e implantar modelos de machine learning na AWS. Como essas tarefas podem ser realizadas?

- Com as ferramentas e recursos do AWS RedShift
    - O Redshift é a plataforma de data warehouse da AWS, otimizada para análises e consultas de BI (Business Intelligence).

- Com as ferramentas e recursos do AWS QuickSight
    - O QuickSight é um serviço de BI com o foco na visualização de dashboards e interação com linguagem natural para a extração de ideias.

- **✅** Com as ferramentas e recursos do AWS SageMaker
    - O Amazon SageMaker é uma plataforma abrangente de aprendizado de máquina (Machine Learning) na AWS, oferecendo uma variedade de serviços e recursos para apoiar desenvolvedores e cientistas de dados. Com recursos como treinamento escalável, hospedagem de modelos e monitoramento em tempo real, os usuários podem criar e implantar modelos com rapidez e eficiência.

- Com as ferramentas e recursos do AWS EMR
    - O Elastic MapReduce (EMR) é uma plataforma gerenciada para processamento de Big Data na AWS.

> **Explicação geral**:  
> O Amazon SageMaker é uma plataforma de machine learning da AWS que facilita o desenvolvimento de modelos de ML. Oferece uma gama de serviços, incluindo algoritmos pré-integrados e notebooks Jupyter para desenvolvimento interativo. O SageMaker permite treinamento escalável com instâncias poderosas e suporta a hospedagem de modelos em produção com escalabilidade automática. Ele também fornece monitoramento em tempo real para avaliar o desempenho dos modelos e inclui ferramentas para automação de fluxos de trabalho. Essas características simplificam e aceleram o ciclo de vida do desenvolvimento de modelos de machine learning.

---

## Pergunta 57

Uma empresa necessita estabelecer uma nova filial de forma ágil e virtualizar dez desktops com o sistema operacional Windows para novos colaboradores. Com qual serviço isso pode ser realizado?

- Com o Amazon CLI
    - O Amazon CLI - Command Line Interface é uma interface por linha de comando que você pode instalar pra fazer uso no seu desktop.

- Com o EC2
    - O EC2 - Elastic Compute Cloud - fornece instâncias de servidores com diversas configurações e opções de processamento, memória e rede.

- **✅** Com o Amazon WorkSpaces
    - Com o Amazon Workspaces é possível provisionar um grande número de máquinas virtuais para uso como desktops.

- Com o Amazon Desktops
    - Este serviço não existe.

> **Explicação geral**:  
> O Amazon WorkSpaces é um serviço de desktop como serviço (DaaS) que permite provisionar desktops virtuais na nuvem, oferecendo uma experiência de desktop segura e personalizada. Ele é ideal para criar escritórios virtuais e facilita a rápida inclusão de novos colaboradores, independentemente da localização. Os desktops podem ser acessados de qualquer lugar com internet, promovendo a mobilidade e o trabalho remoto. O serviço oferece segurança robusta, com controle de acesso, criptografia de dados e backups automáticos. É uma solução escalável para empresas que buscam expandir ou gerenciar seus ambientes de trabalho de forma ágil.

---

## Pergunta 58

Qual é uma das principais vantagens do AWS Network Firewall em comparação com soluções tradicionais de firewall?

- Controle físico do hardware
    - O AWS Network Firewall é um serviço baseado em nuvem e não oferece controle físico direto do hardware, ao contrário de soluções tradicionais de firewall que podem permitir a personalização do hardware e a configuração física do dispositivo.

- Gerenciamento local de dispositivos
    - Diferente das soluções tradicionais que podem ser gerenciadas localmente, o AWS Network Firewall é totalmente gerenciado na nuvem, o que pode não ser ideal para organizações que preferem ou necessitam de gerenciamento local e físico dos dispositivos de firewall.

- Customização de firmware
    - O AWS Network Firewall não permite a customização do firmware, uma característica comum em soluções tradicionais de firewall que podem ser ajustadas em nível de firmware para atender a requisitos específicos.

- **✅** Facilidade de escalabilidade e integração nativa com serviços da AWS.
    - Uma das principais vantagens do AWS Network Firewall é a facilidade de escalabilidade e a integração nativa com serviços da AWS, permitindo uma gestão mais simplificada em ambientes de nuvem.

> **Explicação geral**:  
> O AWS Network Firewall oferece facilidade de escalabilidade e integração nativa com serviços da AWS, simplificando a gestão em ambientes de nuvem. Sua principal função é fornecer uma solução de firewall gerenciado para proteger redes e recursos da AWS contra ameaças cibernéticas, como ataques DDoS, intrusões e malware. Ele assegura a segurança e a integridade do tráfego de rede por meio de regras personalizadas, oferecendo uma camada adicional de proteção para as cargas de trabalho na nuvem e auxiliando na implementação de políticas de segurança robustas.

---

## Pergunta 59

Uma empresa está transferindo suas aplicações para a AWS para direcionar maior atenção ao seu core business, delegando à AWS a responsabilidade pelo gerenciamento da infraestrutura e dos servidores. Diante desse propósito, qual serviço seria aconselhável evitar na nova plataforma?

- DynamoDB
    - O DynamoDB é um banco de dados NoSQL totalmente gerenciado, projetado para oferecer desempenho rápido e escalabilidade automática. Por ser gerenciado pela AWS é aconselhável para uso na situação apresentada.

- Lambda
    - Lambda é um serviço de computação sem servidor que permite executar código sem a necessidade de provisionar ou gerenciar servidores, sendo ativado em resposta a eventos específicos. Por ser gerenciado pela AWS é aconselhável para uso na situação apresentada.

- **✅** EC2
    - Ao utilizar o Amazon EC2, o cliente é responsável pelo gerenciamento de várias tarefas operacionais. Isso inclui a escolha do sistema operacional, instalação de patches de segurança, configuração de firewalls e políticas de segurança, além do monitoramento e escalonamento automático das instâncias. Deve ser evitado para a necessidade apresentada.

- RDS
    - O RDS (Relational Database Service) é um serviço de banco de dados relacional gerenciado, permitindo o uso de engines como MySQL, PostgreSQL, Oracle e SQL Server. Por ser gerenciado pela AWS é aconselhável para uso na situação apresentada.

> **Explicação geral**:  
> Ao utilizar o Amazon EC2, o cliente é responsável pelo gerenciamento de várias tarefas operacionais. Isso inclui a escolha do sistema operacional, instalação de patches de segurança, configuração de firewalls e políticas de segurança, além do monitoramento e escalonamento automático das instâncias. O cliente também é responsável pelo backup e recuperação de dados, bem como pela administração de aplicativos e bancos de dados hospedados nas instâncias. Embora a AWS forneça a infraestrutura física e virtual, o cliente tem autonomia para controlar e personalizar o ambiente EC2 de acordo com suas necessidades específicas, garantindo maior flexibilidade e controle.

---

## Pergunta 60

Sua empresa precisa enviar regularmente documentos e contratos para auditores e reguladores a fim de demonstrar a segurança e a conformidade da infraestrutura da AWS e dos serviços usados por vocês. Qual serviço da AWS pode gerar gratuitamente tais documentos?

- AWS Secret Manager
    - O Secrets Manager é utilizado para armazenar e rotacionar credenciais de acesso a recursos numa espécie de cofre virtual.

- AWS Parameter Store
    - O Parameter Store também é utilizado para armazenar parâmetros e credenciais de acessos de maneira centralizando semelhante ao Secret Manager, mas não faz a rotação das senhas integradas como serviços utilizados.

- AWS Config
    - O Config é utilizado para gerenciar a configuração dos serviços implementados na sua infraestrutura.

- **✅** AWS Artifact
    - O AWS Artifact fornece downloads sob demanda de documentos de segurança e conformidade, como certificações ISO da AWS, Payment Card Industry (PCI) e relatórios SOC (Service Organization Control).

> **Explicação geral**:  
> O Artifact fornece downloads sob demanda de documentos de segurança e conformidade, como certificações ISO da AWS, Payment Card Industry (PCI) e relatórios SOC (Service Organization Control). Você pode enviar os documentos de segurança e conformidade (também conhecidos como artefatos de auditoria) para seus auditores ou reguladores a fim de demonstrar a segurança e a conformidade da infraestrutura da AWS e dos serviços usados por você. Você também pode usar esses documentos como diretrizes para avaliar sua própria arquitetura de nuvem e avaliar os controles internos de sua empresa.

---

## Pergunta 61

Com o objetivo de reduzir a carga de trabalho para os desenvolvedores de microsserviços, uma startup deseja implementar contêineres sem depender de instâncias EC2 como infraestrutura base. Como isso pode ser realizado?

- Com o uso de computação sem servidor com o ECS
    - Apesar do ECS fornecer serviços para contêiner, é o Fargate que fornece os recursos para rodar numa arquitetura sem servidor.

- Com o uso de computação sem servidor com o EKS
    - Apesar do EKS fornecer serviços para contêiner, é o Fargate que fornece os recursos para rodar numa arquitetura sem servidor.

- **✅** Com o uso de computação sem servidor com o Fargate
    - O AWS Fargate é um mecanismo de computação sem servidor e com pagamento conforme o uso que permite a você se concentrar em construir aplicações sem gerenciar servidores.

- Com o uso de computação sem servidor com o DynamoDb
    - O DynamoDB prove bancos de dados noSQL, sem servidor, do tipo chave/valor.

> **Explicação geral**:  
> O AWS Fargate é um mecanismo de computação sem servidor e com pagamento conforme o uso que permite a você se concentrar em construir aplicações sem gerenciar servidores. O AWS Fargate é compatível com o serviço de container ECS (Elastic Container Service) e com o orquestrador de container EKS (Elastic Kubernetes Services). O Fargate acaba com a necessidade de ser proprietário, executar e gerenciar o ciclo de vida de uma infraestrutura de computação, para que você possa se concentrar nas suas aplicações.

---

## Pergunta 62

Uma aplicação requer o provisionamento de novas instâncias EC2 para lidar com picos de carga, sendo necessário desativá-las quando a demanda diminui. Como é possível implementar e automatizar esse processo para otimizar o uso dos recursos computacionais sob demanda?

- Com o uso do AWS Fargate.
    - O AWS Fargate é um mecanismo de computação sem servidor para contêineres que funciona com o ECS e com o EKS. O Fargate facilita a sua concentração no desenvolvimento de aplicativos. O Fargate elimina a necessidade de provisionar e gerenciar servidores, permite que você especifique e pague pelos recursos por aplicativo, além de aumentar a segurança ao conceber aplicativos isolados.

- Com o uso do AWS Elastic Load Balancer.
    - O Elastic Load Balancing distribui automaticamente o tráfego de entrada de aplicações entre diversos destinos, como instâncias do Amazon EC2, contêineres, endereços IP, funções do Lambda e dispositivos virtuais.

- Com o uso do AWS Elastic Contâiner Service.
    - O Amazon Elastic Container Service (Amazon ECS) é um serviço totalmente gerenciado de orquestração de contêineres que ajuda a implantar, gerenciar e escalar facilmente aplicações conteinerizadas. Ele se integra completamente ao restante da plataforma AWS para fornecer uma solução segura e fácil de usar para a execução de workloads de contêiner na nuvem.

- **✅** Com o uso do AWS Auto Scaling Group.
    - Para gerenciar o provisionamento e a desativação automática de instâncias EC2, use o AWS Auto Scaling. Ele ajusta o número de instâncias com base em métricas de desempenho, como uso de CPU, garantindo que você tenha a quantidade ideal de recursos conforme a demanda. Isso otimiza o uso dos recursos e reduz custos.

> **Explicação geral**:  
> O processo de provisionamento e desprovisionamento pelo Auto Scaling Groups é baseado na demanda de recursos. Quando a carga aumenta, o Auto Scaling adiciona instâncias para atender à demanda, usando AMIs predefinidas e configurações especificadas. À medida que a demanda diminui, o Auto Scaling desprovisiona as instâncias excedentes, garantindo eficiência de custos e otimizando o uso de recursos. Esse ajuste automático é contínuo e ajusta-se às flutuações de tráfego, permitindo que a infraestrutura se adapte dinamicamente às necessidades do aplicativo em tempo real, garantindo alta disponibilidade e desempenho.

---

## Pergunta 63

Para acompanhar os custos da sua infraestrutura você gostaria de estimar um teto a ser gasto mensalmente e receber uma notificação por e-mail caso esse valor esteja próximo de ser atingido. Com qual serviço essa configuração é possível?

- AWS Organization
    - O AWS Organizations permite consolidar os gastos de mais de uma conta fazendo a unificação das duas para isso e para outros fins.

- **✅** AWS Budget
    - O AWS Budget permite que você acompanhe os custos da sua conta e habilite o envio de mensagens para até 10 e-mails caso ocorra algum desvio do orçamento estimado.

- AWS Pricing Calculator
    - O AWS Pricing Calculator permite estimar os custos dos serviços da AWS, criando cenários personalizados e ajustando configurações. Ele fornece uma previsão detalhada das despesas e ajuda a comparar preços para otimizar seu orçamento. É uma ferramenta útil para planejar seus gastos com a nuvem.

- AWS Cost Explorer
    - O AWS Cost Explorer permite que você explore os gastos detalhados, porém não envia a notificação automática.

> **Explicação geral**:  
> O AWS Budgets é uma ferramenta que ajuda a monitorar e controlar os custos da sua conta AWS. Com o AWS Budgets, você pode definir orçamentos personalizados para seus serviços e recursos, e receber alertas quando seus gastos se aproximam ou ultrapassam esses limites. Ele permite configurar notificações por e-mail para até 10 destinatários, garantindo que você e sua equipe sejam informados sobre qualquer desvio do orçamento estimado. Isso ajuda a evitar surpresas com custos e facilita o gerenciamento financeiro dos recursos na AWS.

---

## Pergunta 64

Ao criar uma instância EC2, qual serviço deve ser configurado para armazenar e manter os arquivos do sistema operacional, aplicativos e dados, a fim de formar uma máquina virtual completa?

- Elastic Load Balancer (ELB)
    - O ELB (Elastic Load Balancer) distribui automaticamente o tráfego de entrada entre instâncias EC2, garantindo maior disponibilidade e escalabilidade para aplicações.

- Key Management Service (KMS)
    - O KMS (Key Management Service) fornece chaves de criptografia para vários serviços, incluindo o EBS, permitindo a criptografia de dados de forma segura e integrada.

- Simple Storage Service (S3)
    - O S3 (Simple Storage Service) é o serviço padrão da AWS para armazenamento de objetos e arquivos, oferecendo escalabilidade, durabilidade e segurança para dados.

- **✅** Elastic Block Storage (EBS)
    - O Amazon Elastic Block Store (EBS) é um serviço de armazenamento persistente da AWS, projetado para ser usado com instâncias do Amazon EC2. Ele fornece volumes de bloco que atuam como discos virtuais para as instâncias.

> **Explicação geral**:  
> O Amazon Elastic Block Store (EBS) é um serviço de armazenamento persistente da AWS, projetado para ser usado com instâncias do Amazon EC2. Ele fornece volumes de bloco que atuam como discos virtuais para instâncias EC2. Esses volumes podem ser anexados, formatados e usados como dispositivos de armazenamento primário ou secundário para dados e aplicativos. O EBS desempenha um papel fundamental no armazenamento de dados duráveis e altamente disponíveis para instâncias EC2. Ele permite que os dados persistam mesmo quando as instâncias são interrompidas ou desligadas, fornecendo armazenamento persistente e confiável. Os tipos de volumes EBS, como SSDs e discos magnéticos, oferecem diferentes níveis de desempenho e características, permitindo que os usuários escolham a melhor opção para suas necessidades de aplicativos e armazenamento.

---

## Pergunta 65

Uma empresa pretende implantar um conjunto de recursos de infraestrutura na Região de São Paulo, buscando replicabilidade em outras partes do mundo. Como esse objetivo pode ser alcançado?

- Com templates do AWS InfraAsCode
    - "InfraAsCode" é um conceito geral que se refere à prática de gerenciar infraestrutura através de código, e não a um serviço específico. A AWS oferece ferramentas como AWS CloudFormation para implementar a prática de InfraAsCode, e não um serviço chamado "InfraAsCode" para replicar recursos de infraestrutura.

- **✅** Com templates do AWS CloudFormation
    - O AWS CloudFormation é um serviço que permite provisionar e gerenciar recursos da AWS de forma automatizada, usando templates em formato JSON ou YAML, que podem ser replicados em diversas regiões.

- Com templates do AWS CodePipeline.
    - O AWS CodePipeline é uma ferramenta de integração e entrega contínua que automatiza o fluxo de trabalho de software, mas não é projetada para provisionar e replicar recursos de infraestrutura. Seu foco é na automação de pipelines de entrega de software, não na criação de ambientes de infraestrutura.

- Com templates do AWS CodeBuild
    - O AWS CodeBuild é uma ferramenta de construção e integração contínua, não destinada ao provisionamento e replicação de recursos de infraestrutura. Ele se foca em compilar código e executar testes, e não na criação de infraestrutura replicável.

> **Explicação geral**:  
> O AWS CloudFormation é um serviço que permite provisionar e gerenciar recursos da AWS de forma automatizada, usando templates em formato JSON ou YAML. Esses templates descrevem a infraestrutura como código, permitindo que ela seja versionada e replicada em várias regiões. Ao criar um template, é possível configurá-lo para utilizar parâmetros que se adaptam a diferentes regiões. Dessa forma, é fácil reaproveitar o mesmo template em várias regiões da AWS, tornando a implantação de recursos consistente e eficiente em diferentes ambientes geográficos.

---