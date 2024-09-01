## Pergunta 1
Incorreto
Quais são os recursos disponíveis para monitorar eventos no Amazon EventBridge?

- AWS CloudWatch Metrics:
    - Fornece métricas como o número de eventos enviados, taxa de erros e latência, permitindo monitorar o desempenho e a eficiência do EventBridge.

- Trilha de auditoria do AWS CloudTrail
    - Registra chamadas de API para o EventBridge, fornecendo logs detalhados de atividades para auditoria, conformidade e análise de segurança.

- Logs de eventos e métricas do CloudWatch Logs
    - Captura logs detalhados sobre a execução de regras e destinos de eventos, permitindo análise e depuração de problemas.

- **✅** Todas as opções estão corretas
    - Todas as opções estão corretas

> **Explicação geral**:  
> Para monitorar eventos no Amazon EventBridge, é possível utilizar o AWS CloudWatch Logs e Metrics, que fornecem informações detalhadas sobre a entrega de eventos e o desempenho do sistema. O CloudWatch Logs captura dados sobre a execução de regras e destinos de eventos, ajudando a identificar problemas, enquanto o CloudWatch Metrics monitora estatísticas como o número de eventos enviados e a latência. A console do EventBridge facilita a visualização e gerenciamento de eventos em tempo real. Além disso, o AWS CloudTrail pode registrar chamadas de API feitas ao EventBridge, oferecendo logs detalhados para auditoria, conformidade e segurança, permitindo rastrear todas as interações no serviço.

---

## Pergunta 2
Correto
Uma empresa enfrenta incidentes frequentes decorrentes de alterações nas configurações de recursos de aplicativos críticos. Qual serviço pode ser utilizado para avaliar e auditar de maneira contínua as configurações e os relacionamentos desses recursos, visando evitar problemas operacionais?

- **✅** AWS Config
    - Com o AWS Config é possível avaliar e auditar continuamente as configurações e os relacionamentos de seus recursos, contribuindo para a conformidade e evitando problemas operacionais.

- AWS ElastiCache
    - ElastiCache é o serviço recomendado para armazenar dados da aplicação em cache e diminuir a quantidade de entrada e saída de banco de dados, melhorando a performance e reduzindo os custos.

- AWS CloudSearch
    - CloudSearch é o serviço utilizado para implementar mecanismos de busca nas aplicações.

- AWS CloudTrail
    - CloudTrail é o serviço utilizado para logar as chamadas das apis de serviços da AWS, útil para auditorias, identificação de usuários que ligaram ou desligaram recursos, entre outros.

> **Explicação geral**:  
> O AWS Config é um serviço gerenciado que permite avaliar, auditar e monitorar continuamente as configurações dos recursos da AWS. Ele registra e armazena o histórico das configurações dos recursos, facilitando a análise de mudanças ao longo do tempo. O AWS Config permite definir regras de conformidade personalizadas e verificar se os recursos estão alinhados com as políticas de segurança e melhores práticas. Além disso, integra-se com outros serviços da AWS, como AWS Systems Manager Automation, para realizar correções automatizadas. É uma ferramenta essencial para garantir conformidade contínua e gestão eficiente das configurações na nuvem.

---

## Pergunta 3
Correto
Para garantir a proteção das cargas de trabalho na AWS, uma organização precisa implementar um sistema robusto de monitoramento capaz de identificar e remover possíveis malwares instalados nos serviços de sua conta. Quais são os passos e melhores práticas para efetuar essa implementação para detectar, analisar e mitigar essas ameaças de forma eficaz?

- Implemente o Shield no Console da AWS, configure um detector, e integre-o ao CloudTrail. Ajuste as configurações de detecção, estabeleça ações automáticas e revise regularmente os alertas para identificar e remover malwares dos serviços de sua conta AWS
    - O Shield é um serviço de proteção contra DDoS que protege as aplicações em execução e que podem ser atacadas via web.

- Implemente o Inspector no Console da AWS, configure um detector, e integre-o ao CloudTrail. Ajuste as configurações de detecção, estabeleça ações automáticas e revise regularmente os alertas para identificar e remover malwares dos serviços de sua conta AWS
    - O Inspector é o serviço que gerencia vulnerabilidades através da verificação contínua das suas cargas de trabalho. Ele atribui uma pontuação de risco para indicar os itens mais prioritários.

- **✅** Implemente o GuardDuty no Console da AWS, configure um detector, e integre-o ao CloudTrail. Ajuste as configurações de detecção, estabeleça ações automáticas e revise regularmente os alertas para identificar e remover malwares dos serviços de sua conta AWS.
    - O Amazon GuardDuty é um serviço de detecção de ameaças que monitora continuamente atividades maliciosas e comportamentos anômalos em suas contas e cargas de trabalho da AWS.

- Implemente o Macie no Console da AWS, configure um detector, e integre-o ao CloudTrail. Ajuste as configurações de detecção, estabeleça ações automáticas e revise regularmente os alertas para identificar e remover malwares dos serviços de sua conta AWS
    - O Macie é o serviço que usa ML para proteger seus dados confidenciais e restritos em buckets do S3.

> **Explicação geral**:  
> O Amazon GuardDuty é um serviço de detecção de ameaças que monitora continuamente atividades maliciosas e comportamentos anômalos em suas contas e cargas de trabalho da AWS. Ele utiliza inteligência de ameaças e aprendizado de máquina para identificar atividades suspeitas, como tentativas de acesso não autorizado, exploração de vulnerabilidades, malware e comportamentos incomuns em contas AWS. O GuardDuty é fácil de configurar e se integra perfeitamente com outros serviços da AWS, oferecendo alertas detalhados que facilitam a investigação e resposta a incidentes. Além disso, ele ajuda a manter a segurança e conformidade, fornecendo uma camada adicional de proteção contra ameaças avançadas.

> **Nota sobre malwares**:  
> Malware, ou software malicioso, é um tipo de programa criado para causar danos a computadores, servidores, redes ou dispositivos. Ele pode roubar dados sensíveis, corromper arquivos, espionagem, ou comprometer a segurança dos sistemas. Os tipos mais comuns de malware incluem vírus, trojans, worms, ransomware e spyware. Malware pode ser disseminado por e-mails, downloads, sites maliciosos, ou anexos em mensagens. A prevenção e detecção eficazes envolvem o uso de software antivírus e práticas seguras de navegação e gerenciamento de dados.

---

## Pergunta 4
Correto
Uma agência de turismo deseja criar um blog em um ambiente extremamente seguro, acessível e eficiente. Como isso pode ser alcançado através do uso de um provedor de Servidor Privado Virtual (VPS), garantindo segurança robusta, alta disponibilidade e desempenho otimizado?

- Hospedando o blog com o Amazon ECS
    - Subir um blog com VPS no Amazon ECS não é viável porque ECS é projetado para gerenciar containers, não VMs completas, e adiciona complexidade desnecessária na configuração e persistência de dados.

- Hospedando o blog com o Amazon Lambda
    - Não é viável subir um blog com VPS no AWS Lambda porque Lambda é stateless, tem tempo de execução limitado a 15 minutos, e não oferece armazenamento persistente ou configuração contínua do servidor.

- Hospedando o blog com o Amazon Kinesis
    - Não é viável subir um blog com VPS no Amazon Kinesis porque Kinesis é um serviço projetado para processamento e análise de streams de dados em tempo real, não para hospedar aplicações web ou servidores.

- **✅** Hospedando o blog com o Amazon Lightsail
    - O Amazon Lightsail é um provedor de servidor privado virtual (VPS) e a maneira mais fácil de começar a usar a AWS para desenvolvedores, pequenas empresas, estudantes e outros usuários que precisam de uma solução para construir e hospedar suas aplicações na nuvem.

> **Explicação geral**:  
> O Amazon Lightsail é um serviço de Virtual Private Server (VPS) que oferece uma maneira simples e acessível para desenvolvedores, pequenas empresas, estudantes e outros usuários começarem a usar a AWS. Ele é ideal para quem precisa de uma solução fácil para construir e hospedar suas aplicações na nuvem, como um blog, por exemplo. Lightsail fornece tudo o que é necessário para lançar rapidamente um servidor, incluindo armazenamento, DNS e endereços IP estáticos, facilitando a gestão e o escalonamento das aplicações. Essa abordagem simplificada permite que os usuários concentrem-se no desenvolvimento sem se preocupar com a complexidade da infraestrutura.

---

## Pergunta 5
Correto
Para atender aos requisitos de conformidade corporativa, contratual e regulatória, uma empresa necessita criptografar seus dados e aplicativos usando chaves de criptografia armazenadas em um dispositivo de hardware inviolável. De que maneira é viável realizar esse processo?

- Com o uso do Managed Services
    - O Managed Services é o serviço que fornece recursos proativos, preventivos e de detecção que elevam o nível operacional e ajudam a reduzir riscos sem restringir a agilidade, permitindo que você se concentre na inovação e reduza o custo operacional da sua empresa.

- **✅** Com o uso do CloudHSM
    - O CloudHSM ajuda a cumprir requisitos de conformidade contratuais e normativos para a segurança de dados usando instâncias de Hardware Security Module (HSM – Módulo de segurança de hardware).

- Com o uso do Secrets Manager
    - O Secrets Manager tem a função de gerenciar, recuperar e alternar credenciais de acesso a banco de dados, chaves de API e outros segredos ao longo de seus ciclos de vida. Com esse serviço é possível programar a alteração das credenciais sem interromper o uso dos serviços.

- Com o uso do Config
    - Config é o serviço utilizado para gerenciar as configurações de serviços e aplicações permitindo conformidade e auditoria.

> **Explicação geral**:  
> O AWS CloudHSM ajuda a cumprir requisitos de conformidade contratuais e normativos para a segurança de dados, utilizando instâncias de Hardware Security Module (HSM). Um HSM oferece armazenamento seguro de chaves e realiza operações criptográficas em um dispositivo de hardware inviolável. Isso garante que as chaves criptográficas sejam protegidas contra acessos não autorizados e manipulação. Com o CloudHSM, as empresas podem gerenciar suas próprias chaves de criptografia em um ambiente seguro, atendendo a altos padrões de segurança e conformidade regulatória, enquanto beneficiam-se da escalabilidade e flexibilidade da nuvem AWS.

---

## Pergunta 6
Incorreto
Considerando que o pilar de Excelência Operacional do Well-Architected Framework foca na execução e monitoramento de sistemas, além da melhoria contínua de processos e procedimentos, quais são seus principais tópicos?

- projeto de sistemas distribuídos, planejamento de recuperação e requisitos adaptação a mudanças.
    - Refere-se ao pilar de Confiabilidade.

- confidencialidade e integridade de dados, gerenciamento de permissões de usuário e estabelecimento de controles para detectar eventos de segurança.
    - Refere-se ao pilar de Segurança.

- seleção dos tipos e tamanhos certos dos recursos otimizados para os requisitos de workload, monitoramento de performance e manutenção da eficiência à medida que as necessidades comerciais evoluem.
    - Refere-se ao pilar Eficiência de Performance.

- **✅** automação de alterações, reação a eventos e definição de padrões para gerenciar as operações diárias.
    - Refere-se aos principais tópicos do pilar Excelência Operacional.

> **Explicação geral**:  
> O pilar de Excelência Operacional do AWS Well-Architected Framework ajuda arquitetos de nuvem a criar infraestruturas eficientes e de alta performance para aplicações e workloads. Ele se concentra na execução e monitoramento de sistemas, além da melhoria contínua de processos e procedimentos. Os principais tópicos deste pilar incluem automação de operações para reduzir erros manuais, monitoramento contínuo para identificar e resolver problemas rapidamente, e implementação de práticas de gerenciamento de mudanças para garantir atualizações sem interrupções. Ao seguir esses princípios, as organizações podem melhorar a eficiência operacional, aumentar a confiabilidade dos sistemas e promover uma cultura de melhoria contínua.

---

## Pergunta 7
Incorreto
Uma empresa planeja migrar seu CRM para a AWS e deseja ajustar os SLAs para a resolução de incidentes dos seus clientes. Quais são os prazos de resposta estabelecidos pela AWS, de acordo com a gravidade dos incidentes, nos planos de suporte Business, Enterprise on-Ramp e Enterprise?

- Orientações gerais: menos de 24 horas
- Sistema afetado: menos de 12 horas
- Sistema de produção afetado: menos de 4 horas
- Sistema de produção inativo: menos de 1 hora
- Sistema essencial aos negócios inativo: menos de 30 minutos
    - Sistema essencial aos negócios inativo: menos de 30 minutos é válido apenas para o Enterprise On-Ramp e Enterprise

- **✅** Orientações gerais: menos de 24 horas
- Sistema afetado: menos de 12 horas
- Sistema de produção afetado: menos de 4 horas
- Sistema de produção inativo: menos de 1 hora
    - Esses SLAS são garantidos para os 3 planos.

- Orientações gerais: menos de 24 horas
- Sistema afetado: menos de 12 horas
- Sistema de produção afetado: menos de 4 horas
- Sistema de produção inativo: menos de 1 hora
- Sistema essencial aos negócios ou a missão inativo: menos de 15 minutos
    - Sistema essencial aos negócios inativo: menos de 15 minutos para o Enterprise

- Orientações gerais: menos de 12 horas
- Sistema afetado: menos de 6 horas
- Sistema de produção afetado: menos de 2 horas
- Sistema de produção inativo: menos de 30 minutos
- Sistema essencial aos negócios ou a missão inativo: menos de 5 minutos
    - Esses SLAs não são atendidos em nenhum plano.

> **Explicação geral**:  
> Cada plano é projetado para diferentes níveis de complexidade e criticidade, permitindo que os clientes escolham o suporte que melhor se adapta às suas necessidades específicas de negócios e operação.

---

## Pergunta 8
Correto
Uma desenvolvedora precisa migrar uma aplicação que faz uso de um sistema de arquivos para a AWS. Quais são os serviços necessários para alocar essa aplicação neste novo ambiente?

- **✅** EC2 e EFS
    - A integração do Amazon EC2 (Elastic Compute Cloud) com o Amazon EFS (Elastic File System) permite compartilhar armazenamento de arquivos escalável entre instâncias EC2. Isso é útil para aplicativos que precisam de um sistema de arquivos compartilhado, como ambientes de desenvolvimento ou aplicativos de análise.

- EC2 e Storage Gateway
    - O AWS Storage Gateway não é exatamente um sistema de arquivos, mas sim um serviço híbrido de armazenamento que permite que seus aplicativos locais utilizem o armazenamento em nuvem da AWS de maneira transparente.

- ECS e S3
    - O Amazon S3 (Simple Storage Service) não é um sistema de arquivos tradicional, mas sim um serviço de armazenamento de objetos na nuvem. Ao contrário de sistemas de arquivos, que organizam dados em uma hierarquia de diretórios e arquivos, o S3 armazena dados como objetos dentro de "buckets". Cada objeto é composto de dados, metadados e uma chave única que o identifica dentro do bucket.

- EC2 e EBS
    - O Amazon EBS (Elastic Block Store) não é um sistema de arquivos, mas sim um serviço de armazenamento de blocos fornecido pela AWS. Ele fornece volumes de armazenamento em bloco que podem ser anexados a instâncias do Amazon EC2, permitindo que essas instâncias utilizem o EBS como se fosse um disco rígido físico.

> **Explicação geral**:  
> A integração do Amazon EC2 com o Amazon EFS permite compartilhar armazenamento de arquivos escalável entre instâncias EC2. Isso é ideal para aplicativos que necessitam de um sistema de arquivos compartilhado, como ambientes de desenvolvimento ou análise. Montando o EFS em várias instâncias EC2, é possível compartilhar dados de forma consistente e colaborar entre essas instâncias. Essa configuração facilita a escalabilidade horizontal, melhorando a flexibilidade e o desempenho das cargas de trabalho ao permitir uma comunicação eficiente entre as instâncias.

---

## Pergunta 9
Incorreto
Uma empresa de telemarketing deseja utilizar inteligência artificial para gerar insights e melhorar os processos de sua central de atendimento em operação. Qual serviço da AWS pode ser utilizado para essa finalidade?

  - **✅** Contact Center Intelligence (CCI)
    - O CCI (Contact Center Intelligence) permite melhorar a experiência do cliente, impulsionar a produtividade dos atendentes e obter insights de conversas adicionando recursos de IA à central de atendimento de sua preferência, sem qualquer conhecimento de ML.

- Marketplace
    - O Marketplace é utilizado para empresas e desenvolvedores venderem e comprarem soluções prontas desenvolvidas na AWS.

- Quicksight
    - O Quicksight é o serviço que utiliza dashboards e linguagem natural para os usuários tirarem insights a partir dos dados.

- Sua resposta está incorreta
    - Connect
    - O Amazon Connect é o serviço recomendado para criar uma central de atendimento que utilize IA, especialmente se o cliente ainda não possui uma infraestrutura existente. A resposta não é essa justamente porque a questão menciona que já existe uma central em operações.

> **Explicação geral**:  
> O CCI (Contact Center Intelligence) melhora a experiência do cliente, aumenta a produtividade dos atendentes e fornece insights das conversas, adicionando recursos de IA à central de atendimento de sua escolha. Tudo isso é feito sem a necessidade de conhecimentos em Machine Learning (ML), permitindo uma integração fácil e eficiente de inteligência artificial para otimizar o atendimento ao cliente.

---

## Pergunta 10
Correto
Uma Organização pretende empregar o AWS Cloud Adoption Framework (AWS CAF) para incorporar a expertise e as melhores práticas em seu processo de transformação digital, acelerando os resultados de negócios por meio de inovações com a AWS. Em quais seis perspectivas esse serviço agrupa recursos para atender a esse propósito?

- Produto, Pessoas, Governança, Plataforma, Segurança e Operações
    - Não existe uma perspectiva de Produto, ela está incorporada nas demais.

- Negócios, Pessoas, Gestão, Tecnologia, Segurança e Operações
    - Não existe uma perspectiva de Tecnologia, ela está incorporada nas demais.

- **✅** Negócios, Pessoas, Governança, Plataforma, Segurança e Operações
    - O AWS CAF fornece um conjunto de perspectivas ou "lentes", cada uma delas abordando áreas específicas de preocupação, como negócios, pessoas, governança, plataforma, segurança e operações.

- Produto, Pessoas, Gestão, Tecnologia, Segurança e Operações
    - Não existe uma perspectiva de Gestão, ela está incorporada nas demais.

> **Explicação geral**:  
> O AWS CAF (AWS Cloud Adoption Framework) é um conjunto de práticas recomendadas desenvolvido pela Amazon Web Services (AWS) para ajudar organizações a criar uma abordagem eficaz e abrangente para a adoção da nuvem. Ele oferece orientações estratégicas, práticas e conceitos fundamentais para ajudar as empresas a planejar, implementar e gerenciar suas operações na nuvem de maneira eficiente.

> O AWS Cloud Adoption Framework (CAF) é composto por seis perspectivas que ajudam as organizações a estruturar sua jornada de adoção da nuvem de maneira abrangente:
> 1. Negócios (Business): Foca em estratégias de negócios e valores, identificando oportunidades para alavancar a nuvem para alcançar objetivos empresariais.
> 2. Pessoas (People): Trata do gerenciamento de mudanças organizacionais, funções e responsabilidades, além de treinamento e desenvolvimento de habilidades.
> 3. Governança (Governance): Envolve a criação de políticas de governança, gerenciamento de riscos e conformidade para assegurar que a adoção da nuvem esteja alinhada com as normas e regulamentações.
> 4. Plataforma (Platform): Aborda a infraestrutura da nuvem, incluindo arquitetura de sistemas, redes e serviços essenciais para suportar cargas de trabalho.
> 5. Segurança (Security): Foca em aspectos de segurança, como proteção de dados, identidade e acesso, bem como monitoramento e resposta a incidentes.
> 6. Operações (Operations): Envolve a administração e otimização das operações na nuvem, garantindo eficiência e confiabilidade contínuas.

> Essas perspectivas trabalham juntas para garantir uma adoção da nuvem segura, eficiente e alinhada com os objetivos de negócio da organização.

---

## Pergunta 11
Correto
Qual serviço da AWS é ideal para armazenar arquivos de maneira altamente disponível e escalável, permitindo o compartilhamento simultâneo entre várias instâncias EC2?

- Amazon Aurora
    - O Aurora é um banco de dados relacional totalmente gerenciado pela AWS e 5 vezes mais rápido que o MySQL. Recomendado para persistir dados relacionais gerenciados pela AWS através de APIs em aplicações e não para compartilhamento entre instâncias do EC2.

- **✅** Amazon Elastic File System (EFS)
    - O serviço adequado para armazenar arquivos e compartilhá-los entre várias instâncias EC2 é o Amazon Elastic File System (EFS). O Amazon EFS oferece um sistema de arquivos escalável e elástico que pode ser montado simultaneamente em várias instâncias EC2, permitindo o compartilhamento de dados de maneira eficiente e segura.

- AWS Key Management Service (AWS KMS)
    - O KMS é utilizado para gerenciar chaves de criptografia para aplicações e outros serviços da AWS.

- Amazon DocumentDB
    - O Amazon DocumentDB é um banco de dados de documentos gerenciado, compatível com o MongoDB, que permite armazenar, consultar e indexar dados JSON com alta performance e escalabilidade. Ele é projetado para ser altamente disponível e seguro, facilitando a migração e operação de aplicações baseadas em MongoDB. Recomendado para persistir arquivos através de APIs em aplicações e não para compartilhamento entre instâncias do EC2.

> **Explicação geral**:  
> O serviço Amazon Elastic File System (EFS) da AWS é projetado para fornecer armazenamento de arquivos que pode ser compartilhado entre várias instâncias EC2. Ele oferece uma solução de armazenamento escalável e elástica, ajustando automaticamente sua capacidade conforme o volume de dados cresce ou diminui. O EFS é altamente disponível e durável, distribuindo dados automaticamente entre várias zonas de disponibilidade para garantir a resiliência. As instâncias EC2 podem acessar o EFS simultaneamente, facilitando o compartilhamento de arquivos e a colaboração em tempo real. Com suporte para o protocolo NFS, o EFS é fácil de integrar e gerenciar, proporcionando uma experiência de armazenamento de arquivos eficiente e segura.

---

## Pergunta 12
Correto
Uma empresa precisa processar grandes volumes de dados em paralelo, utilizando clusters de servidores de alto desempenho que suportem frameworks como Apache Hadoop, Spark, HBase e Presto. Qual serviço da AWS permite criar, configurar e gerenciar esses clusters de forma eficiente, garantindo escalabilidade, flexibilidade e integração com outros serviços de armazenamento e análise de dados?

- AWS Batch
    - Planeja, agenda e executa cargas de trabalho de computação batch em contêineres, gerenciando automaticamente os recursos necessários para executar trabalhos de forma eficiente.

- Amazon Elastic Container Service (ECS)
    - Gerencia a execução de contêineres Docker em um cluster de máquinas virtuais, facilitando o deployment, scaling e gestão de aplicativos containerizados.

- Amazon Elastic Kubernetes Service (EKS)
    - Gerencia clusters Kubernetes para executar aplicativos em contêineres, automatizando a operação de clusters Kubernetes na infraestrutura da AWS.

- **✅** Amazon Elastic MapReduce (EMR)
    - Processa grandes volumes de dados utilizando frameworks como Apache Hadoop e Spark em clusters escaláveis e gerenciados, ideal para análise de dados e machine learning.

> **Explicação geral**:  
> O Amazon EMR (Elastic MapReduce) é uma escolha eficaz para criar e gerenciar clusters de servidores de alto desempenho para processamento paralelo. Ele utiliza frameworks como Hadoop e Spark para distribuir e processar tarefas em paralelo, permitindo análises de big data em larga escala. Ao provisionar clusters sob demanda, o EMR dimensiona automaticamente recursos de acordo com a carga de trabalho, garantindo eficiência. Isso é especialmente útil para processar e analisar grandes volumes de dados, como modelagem preditiva, análise de logs e extração de informações valiosas, aproveitando a potência do processamento distribuído.

---

## Pergunta 13
Correto
No modelo de Responsabilidade Compartilhada, quais atividades são compartilhadas entre a AWS e o cliente?

(selecione 3 alternativas)

- Proteção ou zona de segurança de serviços e comunicação, roteamento de dados para ambientes de segurança específicos.
    - A proteção ou zona de segurança de serviços e comunicação, bem como o roteamento de dados para ambientes de segurança específicos, é responsabilidade da AWS porque envolve a infraestrutura de rede subjacente e as medidas de segurança implementadas nos data centers da AWS. A AWS assegura que o tráfego de dados seja gerenciado de forma segura, protegendo contra interceptações e garantindo a integridade e confidencialidade das comunicações dentro de sua rede global.

- **✅** Gerenciamento de patches.
    - O gerenciamento de patches é compartilhado no modelo de responsabilidade da AWS porque a AWS é responsável por atualizar e manter a infraestrutura subjacente, enquanto o cliente deve gerenciar patches e atualizações dos sistemas operacionais, aplicativos e dados que ele próprio instala e controla.

- **✅** Gerenciamento de configuração.
    - O gerenciamento de configuração é compartilhado no modelo de responsabilidade da AWS porque a AWS gerencia a configuração da infraestrutura subjacente e dos serviços fornecidos, enquanto o cliente é responsável pela configuração e gerenciamento das suas aplicações, dados e sistemas operacionais implementados na plataforma da AWS.

- **✅** Conhecimentos e treinamentos.
    - O conhecimento e o treinamento são compartilhados no modelo de responsabilidade da AWS porque a AWS fornece documentação, recursos educativos e suporte, enquanto o cliente deve se responsabilizar por entender esses materiais e treinar sua equipe para usar os serviços da AWS de forma eficaz e segura.

- Controles físicos e ambientais.
    - Os controles físicos e ambientais são responsabilidade da AWS porque ela possui e gerencia os data centers onde a infraestrutura de nuvem está localizada, garantindo segurança física, controle de acesso, climatização, prevenção de incêndios e outros aspectos ambientais essenciais para proteger o hardware e manter a continuidade dos serviços.

> **Explicação geral**:  
> O modelo de responsabilidade compartilhada é um princípio fundamental na segurança da nuvem, delineando as responsabilidades entre o provedor de serviços em nuvem (como a AWS) e o cliente. Neste modelo, o provedor é responsável pela segurança da nuvem, ou seja, pela proteção da infraestrutura que executa todos os serviços oferecidos na nuvem. Isso inclui hardware, software, rede e instalações físicas. Por outro lado, o cliente é responsável pela segurança na nuvem, que abrange a gestão e a proteção dos dados, identidade, configurações de segurança, sistemas operacionais, aplicações e firewall de rede.

> Outros itens compartilhados entre a AWS e o cliente incluem:
> - Gerenciamento de identidade e acesso: enquanto a infraestrutura subjacente é gerida pelo provedor, as permissões e acessos específicos são controlados pelo cliente.
> - Segurança dos dados: o provedor garante a disponibilidade e durabilidade dos dados, enquanto o cliente deve encriptar e gerenciar o acesso a esses dados.
> - Configurações de rede: o provedor assegura a infraestrutura de rede segura, enquanto o cliente configura suas próprias políticas de firewall e grupos de segurança.
> - Cumprimento regulatório: o provedor oferece conformidade com várias certificações e padrões, mas cabe ao cliente garantir que suas aplicações e dados cumpram esses requisitos.

---

## Pergunta 14
Correto
Uma empresa situada em uma região com conectividade limitada à internet deseja processar e transferir dados periodicamente de suas cargas de trabalho na AWS. Qual serviço da AWS pode ser empregado para essa finalidade, facilitando a transferência segura e eficiente de grandes volumes de dados, mesmo em condições de conectividade restrita?

- Direct Connect
    - O AWS Direct Connect faz uso da própria infraestrutura global da AWS para melhorar esse tipo de conexão, entretanto, dado a limitação de conectividade e a alta volumetria de dados, serviços da família Snow são mais apropriados.

- Snowmobile
    - O Snowmobile é um dispositivo físico da família Snow utilizado para migrar dados na escala de petabytes para a AWS. Apresenta dimensões de Contêiner de transporte de 45 pés, transportado por caminhão.

- Snowcone
    - O Snowcone é o dispositivo mais compacto e portátil utilizado para migrar dados na escala de petabytes para a AWS. Apresenta dimensões de 227 mm x 148.6 mm x 82.65 mm.

- **✅** Snowball Edge
    - O Snowball Edge é um dispositivo físico da família Snow, projetado para processar e migrar dados.

> **Explicação geral**:  
> O Snowball Edge é um dispositivo físico da família Snow, projetado para processar e migrar dados em escala de terabytes para a AWS, ideal para locais com baixa ou nenhuma conectividade com a Internet. Ele é oferecido em dois modelos: um otimizado para armazenamento e outro para computação, permitindo flexibilidade conforme a necessidade. Com dimensões de 548 mm x 320 mm x 501 mm, o Snowball Edge é portátil e pode ser facilmente transportado por veículos, facilitando a movimentação de grandes volumes de dados de maneira segura e eficiente. É uma solução robusta para desafios de transferência de dados em ambientes remotos ou desconectados.

> **Nota sobre a família Snowball**:  
> O Snowball Edge está incluído no guia oficial do exame, enquanto o Snowmobile e o Snowcone não estão. O Snowball Edge fornece dispositivos para armazenamento e computação, ao passo que o Snowmobile e o Snowcone são apenas para armazenamento. Para a prova, é essencial compreender a finalidade dos serviços da família Snow, que é a migração de dados através de dispositivos físicos, e não pela internet, atendendo a diversos casos de uso.

---

## Pergunta 15
Correto
Com o objetivo de assegurar a segurança e disponibilidade de suas cargas de trabalho, uma empresa requer que a equipe de suporte do Concierge forneça assistência e suporte para as contas da AWS. Quais planos de suporte oferecem esse serviço? (selecione 2 alternativas)

- Business
    - Esse plano não oferece esse tipo de serviço.

- Basic
    - Esse plano não oferece esse tipo de serviço.

- **✅** Enterprise On-Ramp
    - Esse plano inclui acesso a um Concierge Support Team dedicado para ajudar com questões de gerenciamento de contas e faturamento.

- **✅** Enterprise
    - Esse plano inclui acesso a um Concierge Support Team dedicado para ajudar com questões de gerenciamento de contas e faturamento.

- Developer
    - Esse plano não oferece esse tipo de serviço.

> **Explicação geral**:  
> Os planos de suporte da AWS que oferecem serviços de concierge são o Enterprise On-Ramp e o Enterprise Support. Esses planos incluem acesso a um Concierge Support Team dedicado para ajudar com questões de gerenciamento de contas e faturamento. O serviço de concierge fornece uma camada adicional de suporte, ajudando as empresas a navegar pelo ecossistema AWS, otimizar custos e resolver rapidamente problemas administrativos. Este suporte é especialmente valioso para empresas que gerenciam grandes volumes de recursos na nuvem e precisam de assistência personalizada para maximizar o valor de seus investimentos na AWS.

---

## Pergunta 16
Correto
Como um auditor pode monitorar, registrar e analisar atividades detalhadas em múltiplas contas da AWS, garantindo conformidade com políticas de segurança e regulatórias?

- Através do Amazon Macie
    - Detecta e protege dados confidenciais usando machine learning, mas não é projetado para monitorar e registrar todas as atividades e eventos das contas da AWS como o CloudTrail.

- **✅** Através do AWS CloudTrail
    - O AWS CloudTrail registra todas as atividades de API e eventos em suas contas AWS, fornecendo logs detalhados que permitem monitorar e auditar ações realizadas por usuários e serviços. CloudTrail facilita a análise de segurança, conformidade regulatória e a solução de problemas operacionais ao oferecer visibilidade completa das atividades na AWS.

- Através do AWS WAF
    - Protege aplicações web contra ameaças comuns na internet ao filtrar e monitorar requisições HTTP e HTTPS, mas não fornece logs detalhados de atividades de API e eventos em contas da AWS como o CloudTrail.

- Através do AWS Config
    - Monitora e registra as configurações de recursos da AWS e suas mudanças ao longo do tempo, mas não fornece logs detalhados de atividades de API e eventos como o CloudTrail.

> **Explicação geral**:  
> O AWS CloudTrail é um serviço de auditoria que registra e monitora todas as atividades realizadas em sua conta da AWS, proporcionando visibilidade abrangente sobre as operações e ações realizadas. Ele gera logs detalhados de eventos, incluindo ações de usuários, chamadas de API, alterações de configuração e interações com outros serviços da AWS. Esses registros permitem que administradores rastreiem e auditem atividades para garantir conformidade com políticas de segurança e regulatórias. CloudTrail pode ser configurado para capturar eventos em todas as regiões da AWS, garantindo que nenhuma atividade passe despercebida. Além disso, os logs podem ser armazenados no Amazon S3 para análise posterior e integração com serviços como Amazon CloudWatch Logs para monitoramento contínuo. Com CloudTrail, é possível identificar padrões de uso, detectar comportamentos anômalos e realizar investigações detalhadas em caso de incidentes de segurança, tornando-se uma ferramenta essencial para a governança, conformidade e segurança na nuvem da AWS.

---

## Pergunta 17
Correto
Os componentes das soluções do AWS Virtual Private Network (VPN) permitem conexões seguras entre redes locais, escritórios remotos, dispositivos de clientes e a rede global da AWS. Quais são os serviços que compõem essas soluções?

(selecione 2 alternativas)

- **✅** AWS Site-to-Site VPN
    - O Site-to-Site VPN estabelece túneis criptografados entre sua rede e as Amazon Virtual Private Clouds ou os AWS Transit Gateways, proporcionando uma conexão segura entre redes locais e os recursos da AWS.

- **✅** AWS Client VPN
    - O AWS Client VPN conecta usuários à AWS ou a recursos locais por meio de um cliente de software VPN, oferecendo uma solução para acesso remoto seguro à infraestrutura da AWS.

- AWS Direct Connect
    - O Direct Connect cria uma conexão dedicada que não trafega dados fora da infraestrutura da AWS, não faz parte do AWS VPN.

- AWS Storage Gateway
    - O Storage Gateway é um serviço de armazenamento em nuvem híbrida que permite que soluções no ambiente on premises façam uso do armazenamento em cloud praticamente sem limites. Pode armazenar backups, data lakes, etc.

- AWS Connect
    - O Connect permite a implementação de uma central de atendimento multi-canal e que faz uso de IA.

> **Explicação geral**:  
> O AWS VPN é composto por dois serviços principais: o AWS Site-to-Site VPN e o AWS Client VPN. O Site-to-Site VPN permite a criação de túneis criptografados entre sua rede local e as Amazon Virtual Private Clouds (VPCs) ou AWS Transit Gateways, assegurando uma conexão segura e privada entre suas instalações on-premises e os recursos da AWS. Esse serviço é ideal para empresas que precisam integrar suas redes locais com a infraestrutura da AWS de maneira segura e confiável. Por outro lado, o AWS Client VPN conecta usuários individuais à AWS ou a recursos locais através de um cliente de software VPN, proporcionando uma solução eficiente e segura para acesso remoto. Com o Client VPN, os usuários podem se conectar de qualquer lugar, garantindo a segurança e a integridade dos dados transmitidos. Ambos os serviços utilizam criptografia robusta para proteger os dados em trânsito e são altamente escaláveis, permitindo que as empresas adaptem suas necessidades de conectividade à medida que crescem. Além disso, a configuração e o gerenciamento dessas VPNs são simplificados através do console de gerenciamento da AWS, tornando a implementação de soluções de rede seguras acessível para organizações de todos os tamanhos.

---

## Pergunta 18
Correto
Qual serviço da AWS foi projetado para capacitar analistas de Business Intelligence a realizar análises avançadas e executar consultas complexas em grandes volumes de dados, oferecendo alto desempenho e escalabilidade para processar datasets massivos de maneira eficiente?

- Amazon RDS (Relational Database Service)
    - Amazon RDS (Relational Database Service) é uma plataforma gerenciada para bancos de dados relacionais, ideal para cargas de trabalho OLTP e aplicações que requerem alta disponibilidade e recuperação de desastres. Embora suporte consultas SQL e análises básicas, RDS não é otimizado para consultas analíticas complexas e grandes volumes de dados como o Amazon Redshift, que utiliza técnicas avançadas de armazenamento em coluna e paralelismo para análises de Business Intelligence em larga escala.

- **✅** Amazon Redshift
    - O Amazon Redshift é um data warehouse totalmente gerenciado, projetado para análises de Business Intelligence (BI) em larga escala. Ele permite que analistas realizem consultas SQL complexas e análises avançadas em grandes conjuntos de dados de forma rápida e eficiente. Redshift é altamente escalável e oferece alto desempenho ao processar datasets massivos.

- Amazon DynamoDB
    - O Amazon DynamoDB é um banco de dados NoSQL otimizado para acesso rápido e escalabilidade, ideal para cargas de trabalho de chave-valor e documentos. No entanto, não é adequado para consultas analíticas complexas em grandes volumes de dados, como o Amazon Redshift, que é projetado especificamente para análises de Business Intelligence e consultas SQL avançadas.

- Amazon Aurora
    - O Amazon Aurora é um banco de dados relacional otimizado para cargas de trabalho transacionais (OLTP) com alta disponibilidade. Ele não é ideal para análises de Business Intelligence em grande escala, pois não possui as otimizações específicas de processamento de consultas e armazenamento em coluna que o Amazon Redshift oferece para grandes volumes de dados e análises complexas.

> **Explicação geral**:  
> O Amazon Redshift é um serviço de data warehouse na nuvem, rápido e totalmente gerenciado, oferecido pela AWS. Ele é otimizado para executar análises avançadas e consultas SQL complexas em grandes conjuntos de dados, utilizando armazenamento em coluna para maximizar a eficiência e a velocidade das consultas. Redshift oferece alta escalabilidade, permitindo o processamento de petabytes de dados com facilidade, e usa paralelismo massivo para acelerar o tempo de resposta das consultas.

---

## Pergunta 19
Correto
Com o objetivo de reforçar a segurança na esteira de desenvolvimento de uma aplicação, o setor de segurança de uma corretora de investimentos requisitou que as configurações de conexões e senhas para acessar o banco de dados sejam removidas do código-fonte da aplicação. Como é possível atender a essa solicitação sem comprometer tais conexões e o funcionamento da aplicação?

- Alterando o código fonte para acessar as configurações a partir do KMS
    - O KMS é utilizado para gerenciar chaves de criptografia para serviços e aplicações.

- Alterando o código fonte para acessar as configurações a partir do License Manager
    - O License Manager deve ser utilizado para gerenciar as licenças ao rastrear o seu uso, permitindo maior controle, economia de custos e conformidade com o limite de uso estabelecido em contrato com os fornecedores.

- Alterando o código fonte para acessar as configurações a partir do Managed Services
    - O Managed Services é o serviço que fornece recursos proativos, preventivos e de detecção que elevam o nível operacional e ajudam a reduzir riscos sem restringir a agilidade, permitindo que você se concentre na inovação e reduza o custo operacional da sua empresa. Contempla segurança, gerenciamento de incidentes, automação, redução de custos e acesso a especialistas da AWS.

- **✅** Alterando o código fonte para acessar as configurações a partir do Parameter Store.
    - Com o Parameter Store, é possível atualizar as configurações e senhas de forma dinâmica sem a necessidade de alterar o código-fonte ou reiniciar a aplicação, mantendo a continuidade do serviço.

> **Explicação geral**:  
> O AWS Systems Manager Parameter Store é um serviço que permite armazenar e gerenciar parâmetros de configuração e segredos de forma segura e centralizada. Ele é particularmente útil para aplicações, pois permite que informações sensíveis como credenciais de banco de dados, endpoints de APIs e variáveis de ambiente sejam mantidas fora do código-fonte. Ao utilizar o Parameter Store, os desenvolvedores podem acessar esses parâmetros de forma dinâmica durante o tempo de execução, garantindo que as configurações sejam atualizáveis sem a necessidade de modificar o código da aplicação. Além disso, a integração com o AWS IAM permite controlar rigorosamente quem pode acessar e modificar esses parâmetros, aumentando a segurança. Esse serviço também oferece criptografia automática para proteger dados sensíveis, contribuindo para práticas de segurança robustas e conformidade com políticas de segurança.

---

## Pergunta 20
Correto
Uma startup está prestes a lançar um aplicativo em produção e precisa de suporte adequado. Qual é o plano de suporte mínimo recomendado pela AWS para garantir acesso a recursos técnicos essenciais e suporte 24/7 para assegurar uma operação contínua e bem-sucedida?

- Enterprise
    - O Enterprise é recomendado para quem tem negócios e/ou workloads essenciais na AWS.

- **✅** Business
    - O Business é o Nível mínimo recomendado para quem tem workloads de produção na AWS.

- Developer
    - O Developer é recomendado se você estiver experimentando ou testando a AWS.

- Enterprise On-ramp
    - O Enterprise on-Ramp é recomendado para quem tem workloads essenciais à produção ou aos negócios na AWS.

> **Explicação geral**:  
> Cada plano é projetado para diferentes níveis de complexidade e criticidade, permitindo que os clientes escolham o suporte que melhor se adapta às suas necessidades específicas de negócios e operação:
> - Basic Support: Ideal para clientes que estão apenas começando com a AWS. Este plano é gratuito e inclui acesso 24/7 ao atendimento ao cliente para questões de cobrança e suporte aos serviços, além de acesso à comunidade AWS e ao AWS Personal Health Dashboard.
> - Developer Support: Adequado para desenvolvedores que estão testando ou explorando a AWS. Por um custo mensal, este plano oferece suporte durante horário comercial, acesso a engenheiros de suporte via e-mail e consultoria geral sobre melhores práticas.
> - Business Support: Recomendado para empresas que têm cargas de trabalho críticas e precisam de suporte 24/7. Inclui acesso a engenheiros de suporte via e-mail, chat e telefone, resposta rápida a incidentes críticos, suporte para gerenciamento de contas e orientação arquitetônica.
> - Enterprise On-Ramp Support: Ideal para empresas em crescimento com cargas de trabalho importantes. Oferece suporte 24/7, tempos de resposta rápidos, análises proativas de contas e planejamento de eventos. Serve como uma ponte entre os planos Business e Enterprise, fornecendo suporte robusto sem a necessidade de um Gerente Técnico de Contas (TAM) dedicado.
> - Enterprise Support: Destinado a grandes empresas que necessitam de suporte contínuo e personalizado para ambientes de missão crítica. Este plano oferece um Gerente Técnico de Contas (TAM), suporte 24/7 com resposta prioritária, revisões de arquitetura e uma variedade de workshops e treinamentos.

---

## Pergunta 21
Correto
Uma startup deseja migrar integralmente a carga de trabalho de seus aplicativos para a AWS, mas enfrenta a limitação de uma equipe de TI insuficiente para garantir o desenvolvimento de novas funcionalidades e suporte. Diante desse cenário, qual serviço da AWS é essencial para atender às necessidades de suporte dessa startup, proporcionando auxílio contínuo e especializado para manter a operação e o desenvolvimento dos aplicativos?

- Marketplace
    - O Marketplace é o portal onde você pode encontrar software prontos para diversas necessidades de negócio, além disso, se você é um desenvolvedor ou uma empresa que possui um aplicativo, você pode comercializá-lo nesta plataforma também.

- License Manager
    - O License Manager deve ser utilizado para gerenciar as licenças ao rastrear o seu uso, permitindo maior controle, economia de custos e conformidade com o limite de uso estabelecida em contrato com os fornecedores.

- Parameter Store
    - O Parameter Store é um recurso do AWS Systems Manager que oferece armazenamento hierárquico seguro para gerenciamento de dados de configuração e gerenciamento de segredos.

- **✅** Managed Services
    - O AWS Managed Services (AMS) fornece recursos proativos, preventivos e de detecção que melhoram o nível operacional e ajudam a reduzir riscos sem comprometer a agilidade, permitindo que você se concentre na inovação e reduza os custos operacionais da sua empresa.

> **Explicação geral**:  
> O AWS Managed Services (AMS) fornece recursos proativos, preventivos e de detecção que melhoram o nível operacional e ajudam a reduzir riscos sem comprometer a agilidade, permitindo que você se concentre na inovação e reduza os custos operacionais da sua empresa. Ele abrange segurança, gerenciamento de incidentes, automação, redução de custos e oferece acesso a especialistas da AWS. AMS garante que suas operações sejam eficientes e seguras, com suporte contínuo e otimização de recursos, facilitando a gestão de infraestrutura e liberando sua equipe para focar em iniciativas estratégicas e de inovação.

---

## Pergunta 22
Correto
Para otimizar a performance de uma integração entre serviços localizados em duas regiões diferentes da AWS, uma empresa busca conectá-los evitando o uso do tráfego instável da internet. Como isso pode ser realizado?

- Com o uso do Amazon API Gateway
    - O API Gateway é um serviço para criar e gerenciar APIs.

- Com o uso do AWS VPN
    - A VPN é um serviço que cria conexões virtuais, permitindo que usuários e redes se conectem de forma segura através da internet.

- **✅** Com o uso do AWS Direct Connect
    - O AWS Direct Connect é um serviço de rede que fornece uma alternativa ao uso da internet para se conectar à AWS. Com ele, os dados que antes trafegariam pela internet são transmitidos por meio de uma conexão de rede privada diretamente entre suas instalações e a AWS, garantindo maior segurança e desempenho.

- Com o uso do Amazon Connect
    - O Connect é o serviço para implementar uma central de atendimento multi-canal com IA.

> **Explicação geral**:  
> O AWS Direct Connect é um serviço de rede que fornece uma conexão dedicada e privada entre suas instalações e a infraestrutura da AWS, oferecendo uma alternativa ao uso da internet para acessar serviços na nuvem. Utilizando o Direct Connect, você pode transferir dados de forma mais segura, consistente e com menor latência, o que é ideal para aplicações sensíveis ao desempenho. Essa conexão dedicada melhora a estabilidade e a confiabilidade das transferências de dados, tornando-a uma solução eficiente para migrações de dados em larga escala, backups e recuperação de desastres. Além disso, o Direct Connect permite escalabilidade de largura de banda, atendendo às necessidades crescentes de sua organização.

---

## Pergunta 23
Correto
Uma organização precisa executar cargas de trabalho de Computação de Alto Desempenho (HPC), que requerem grande capacidade de processamento e baixa latência. Qual serviço da AWS oferece uma solução para implementar e operar essas cargas de trabalho complexas de maneira eficiente?

- AWS Lambda
    - Serviço serverless que executa código em resposta a eventos sem necessidade de gerenciar servidores. Não é adequado para HPC devido às limitações de tempo de execução e capacidade de processamento.

- **✅** Amazon EC2
    - O Amazon EC2 oferece instâncias especializadas para HPC, como as instâncias C5, C6g e P4, que são otimizadas para processamento intensivo e baixa latência.

- Amazon ECS (Elastic Container Service)
    - Serviço de gerenciamento de contêineres Docker em clusters. Embora eficiente para gerenciamento de contêineres, não proporciona o desempenho e a baixa latência requeridos para cargas de trabalho HPC intensivas.

- AWS Elastic Beanstalk
    - Plataforma que facilita a implantação e gerenciamento de aplicativos web. Não é ideal para HPC porque não oferece o controle necessário sobre os recursos de hardware e a otimização da rede.

> **Explicação geral**:  
> O Amazon EC2 (Elastic Compute Cloud) é um serviço que fornece capacidade de computação escalável na nuvem, permitindo a execução de diversas cargas de trabalho, incluindo Computação de Alto Desempenho (HPC). Para HPC, o EC2 oferece instâncias especializadas, como as instâncias C5, C6g e P4, que são otimizadas para processamento intensivo, cálculos científicos, modelagem financeira, simulações e renderização de gráficos.

> Essas instâncias de alto desempenho são equipadas com CPUs e GPUs poderosas, redes de alta largura de banda com baixa latência e suporte a sistemas de arquivos paralelos, como Amazon FSx for Lustre. Além disso, EC2 pode ser combinado com o AWS ParallelCluster para simplificar a criação e gerenciamento de clusters HPC, permitindo que os usuários configurem rapidamente ambientes de HPC escaláveis e integrados com outros serviços da AWS, como S3 e DynamoDB, para armazenamento de dados.

---

## Pergunta 24
Correto
Uma engenheira Devops está construindo uma esteira com diversos serviços para habilitar um processo de integração e entrega contínua (CI/CD) para o time de desenvolvimento da sua empresa. Qual serviço da AWS é utilizado para esse tipo de implementação?

- AWS CodeCommit
    - O AWS CodeCommit é um serviço de controle de origem gerenciado seguro e altamente dimensionável que hospeda repositórios privados do Git. Ele torna mais fácil para as equipes colaborarem com segurança no código com contribuições criptografadas em trânsito e em repouso.

- AWS Step Functions
    - O AWS Step Functions é um serviço de fluxo de trabalho visual que utiliza pouco código, usado para orquestrar serviços da AWS, automatizar processos de negócios e criar aplicações sem servidor. Os fluxos de trabalho gerenciam falhas, novas tentativas, paralelização, integrações de serviços e observabilidade, de modo que os desenvolvedores possam se concentrar na lógica de negócios com maior valor.

- **✅** AWS CodePipeline
    - O AWS CodePipeline é um serviço gerenciado de entrega continua que ajuda a automatizar pipelines de liberação para oferecer atualizações rápidas e confiáveis de aplicativos e infraestruturas.

- AWS Workflow
    - O AWS Workflow não existe na AWS.

> **Explicação geral**:  
> O AWS CodePipeline é um serviço gerenciado de entrega contínua que automatiza o processo de liberação de software, facilitando atualizações rápidas e confiáveis de aplicativos e infraestruturas. Ele permite a definição de pipelines de liberação que automatizam as etapas de compilação, teste e implantação, ativadas sempre que ocorrem mudanças no código. Com o CodePipeline, os desenvolvedores podem implementar integrações contínuas e fluxos de trabalho de entrega contínua, garantindo que o software seja testado e liberado de forma consistente e segura. O serviço é altamente personalizável, permitindo a integração com diversas ferramentas e serviços de desenvolvimento, como GitHub, Jenkins e AWS CodeBuild. Isso garante uma cadeia de entrega eficiente, melhorando a qualidade e a velocidade de entrega de novas funcionalidades.

---

## Pergunta 25
Correto
Uma equipe de desenvolvimento pretende gerenciar o código-fonte de uma aplicação por meio de um repositório centralizado que permita a criação de ramos (branches) distintos para o código em fase de desenvolvimento e produção. Por meio de qual serviço essa implementação pode ser realizada?

- AWS CodeBuild
    - O CodeBuild é um serviço da AWS CI/CD (Continuous Integration/Continuous Delivery) que automatiza a compilação e teste de código, facilitando a integração e entrega contínua de software.

- **✅** AWS CodeCommit
    - O AWS CodeCommit é um serviço de controle de versão totalmente gerenciado da AWS, que utiliza a tecnologia Git para gerenciar o código-fonte das aplicações. Ele é fundamental no início da esteira de CI/CD (Integração Contínua/Entrega Contínua), permitindo que equipes de desenvolvimento colaborem de maneira eficiente. Com o CodeCommit, os desenvolvedores podem criar ramos (branches) para trabalhar de forma independente em diferentes funcionalidades ou correções, facilitando o fluxo de trabalho colaborativo. Além disso, ele suporta merges para integrar mudanças de diferentes ramos de forma segura e eficaz. O CodeCommit oferece todas as funcionalidades padrão do Git, como commits, pull requests e revisões de código, enquanto se integra perfeitamente com outros serviços da AWS. Isso proporciona uma solução robusta e segura para o gerenciamento de código, escalável para projetos de qualquer tamanho.

- AWS CodeStar
    - O AWS CodeStar facilita o desenvolvimento, construção e implantação rápida de aplicações na AWS, oferecendo um ambiente integrado para gerenciamento de projetos CI/CD. Ele inclui ferramentas de gerenciamento de projetos e integração com serviços da AWS. CodeStar também fornece projetos de exemplo pré-configurados, ajudando desenvolvedores a iniciar rapidamente com práticas recomendadas.

- AWS CodeDeploy
    - O AWS CodeDeploy é um serviço de implantação que automatiza a distribuição de código a qualquer instância, seja em nuvem ou on-premises, facilitando atualizações rápidas e seguras de aplicações.

> **Explicação geral**:  
> O CodeCommit é um serviço de controle de versão totalmente gerenciado da AWS, que utiliza a tecnologia Git para gerenciar o código-fonte das aplicações. Ele é fundamental no início da esteira de CI/CD (Integração Contínua/Entrega Contínua), permitindo que equipes de desenvolvimento colaborem de maneira eficiente. Com o CodeCommit, os desenvolvedores podem criar ramos (branches) para trabalhar de forma independente em diferentes funcionalidades ou correções, facilitando o fluxo de trabalho colaborativo. Além disso, ele suporta merges para integrar mudanças de diferentes ramos de forma segura e eficaz. O CodeCommit oferece todas as funcionalidades padrão do Git, como commits, pull requests e revisões de código, enquanto se integra perfeitamente com outros serviços da AWS. Isso proporciona uma solução robusta e segura para o gerenciamento de código, escalável para projetos de qualquer tamanho.

---

## Pergunta 26
Correto
No modelo de Responsabilidade Compartilhada da AWS, quais são os controles que o cliente herda completamente da AWS, ficando sob a responsabilidade exclusiva da AWS garantir sua implementação e gestão?

- Gerenciamento de configuração.
    - O gerenciamento de configuração é compartilhado no modelo de responsabilidade da AWS porque a AWS gerencia a configuração da infraestrutura subjacente e dos serviços fornecidos, enquanto o cliente é responsável pela configuração e gerenciamento das suas aplicações, dados e sistemas operacionais implementados na plataforma da AWS.

- Conhecimentos e treinamento.
    - O conhecimento e o treinamento são compartilhados no modelo de responsabilidade da AWS porque a AWS fornece documentação, recursos educativos e suporte, enquanto o cliente deve se responsabilizar por entender esses materiais e treinar sua equipe para usar os serviços da AWS de forma eficaz e segura.

- **✅** Controles físicos e ambientais
    - A AWS é responsável pela segurança físicas e ambientais dos data centers, rede e hardware subjacente, bem como pela segurança das áreas compartilhadas.

- Gerenciamento de patches.
    - O gerenciamento de patches é compartilhado no modelo de responsabilidade da AWS porque a AWS é responsável por atualizar e manter os softwares de infraestrutura subjacente, enquanto o cliente deve gerenciar patches e atualizações dos sistemas operacionais, aplicativos e dados que ele próprio instala e controla.

> **Explicação geral**:  
> No modelo de responsabilidade compartilhada da AWS, os clientes herdam controles de segurança da infraestrutura de nuvem da AWS. A AWS é responsável pela segurança físicas e ambientais dos data centers, rede e hardware subjacente, bem como pela segurança das áreas compartilhadas. Os clientes são responsáveis por configurar corretamente os serviços, implementar medidas de segurança, gerenciar a identidade e o acesso dos usuários, além de proteger os dados e aplicativos. Isso inclui a definição de políticas de acesso, criptografia e monitoramento de atividades, garantindo a conformidade e segurança dos recursos implantados na nuvem AWS.

---

## Pergunta 27
Correto
Uma startup precisa implantar e gerenciar aplicativos serverless que sejam escaláveis automaticamente, integrem-se facilmente a outros serviços da AWS e ofereçam suporte a uma ampla gama de linguagens de programação. Qual serviço da AWS é mais adequado para atender a essas necessidades, garantindo eficiência operacional e custos otimizados?

- Amazon API Gateway
    - O Amazon API Gateway permite criar, publicar e gerenciar APIs, funcionando como interface para backend. Ele não gerencia diretamente aplicativos serverless, mas integra-se com serviços como AWS Lambda, que executam o código sem servidor.

- Amazon Relational Database Service (Amazon RDS)
    - O Amazon RDS é um serviço de banco de dados relacional gerenciado.

- Amazon Elastic Container Service (Amazon ECS)
    - O Amazon Elastic Container Service (ECS) é usado para implantar e gerenciar aplicativos em contêineres, com servidores. O Fargate realiza a mesma função sem servidores.

- **✅** Amazon Lambda
    - O AWS Lambda é um serviço de computação sem servidor (serverless) que executa código em resposta a eventos. Ele permite que os desenvolvedores executem funções de forma escalável e automatizada, sem se preocupar com a infraestrutura subjacente. Com o Lambda, você pode criar microserviços, automatizar tarefas, processar eventos em tempo real e executar código sob demanda. Ele é altamente flexível, suporta várias linguagens de programação e pode ser integrado a outros serviços AWS.

> **Explicação geral**:  
> O AWS Lambda é um serviço de computação sem servidor (serverless) que executa código em resposta a eventos, permitindo que os desenvolvedores executem funções de maneira escalável e automatizada, sem a necessidade de gerenciar a infraestrutura subjacente. Com o Lambda, é possível criar microserviços, automatizar tarefas, processar eventos em tempo real e executar código sob demanda, o que torna o desenvolvimento mais ágil e eficiente. Ele oferece suporte a várias linguagens de programação, como Python, Java, Go, Node.js, entre outras, proporcionando flexibilidade na escolha das ferramentas de desenvolvimento. Além disso, o Lambda pode ser facilmente integrado a outros serviços da AWS, como S3, DynamoDB, SNS, SQS, entre outros, facilitando a implementação de lógica de negócios e processos automatizados. A escalabilidade automática do Lambda garante que sua aplicação possa lidar com variações de carga de maneira eficiente, otimizando custos ao cobrar apenas pelo tempo de execução do código. Isso permite que as empresas se concentrem mais na inovação e no desenvolvimento de novos recursos, sem se preocupar com a manutenção e o dimensionamento da infraestrutura.

---

## Pergunta 28
Incorreto
Qual serviço deve ser utilizado para que uma equipe de suporte receba um e-mail quando algum alerta de monitoramento for gerado pelo CloudWatch?

- Amazon Simple Queue Service (SQS)
    - O SQS é o sistema de mensageria que possibilita a comunicação e desacoplamento de microsserviços.

- AWS Budgets
    - O AWS Budgets é um serviço que permite aos clientes definir e gerenciar orçamentos para seus gastos na AWS. Um dos recursos do AWS Budgets é enviar notificações por e-mail quando os custos projetados ou reais excedem os limites definidos pelo cliente, mas é apenas neste contexto de custo, não para alerta e monitoramento de outros serviços.

- Resposta correta
    - AWS Simple Email Service (SES)
    - Além de permitir o alcance dos clientes por e-mail sem um sistema de SMTP (Simple Mail Transfer Protocol), o Simple Email Service (SES) pode ser integrado em diversos serviços da AWS para enviar mensagens por email sobre a evolução de processos, implantações e alertas de monitoramento.

- Sua resposta está incorreta
    - AWS Amazon Simple Notification Service (SNS)
    - O SNS é o serviço de Pub/Sub que utiliza tópicos para que a partir de uma mensagem publicada, todos os assinantes possam acessá-la.

> **Explicação geral**:  
> O Simple Email Service (SES) da AWS permite enviar e-mails aos clientes sem a necessidade de configurar um sistema SMTP próprio. Além disso, o SES pode ser integrado a vários serviços da AWS para enviar notificações por e-mail sobre o progresso de processos, implantações e alertas de monitoramento. Essa integração facilita a comunicação em tempo real com usuários e equipes, proporcionando uma solução eficaz e escalável para o envio de mensagens automatizadas. O SES é ideal para casos de uso que requerem alta capacidade de entrega de e-mails com controle sobre conteúdo e formato das mensagens.

---

## Pergunta 29
Correto
Uma companhia aérea requer que seus passageiros apresentem comprovantes de vacinação para certos trechos e destinos de viagem no check-in. Para agilizar o processo, uma estratégia de automatização consiste em permitir que os passageiros enviem os comprovantes em formato .pdf ou .jpg por meio do aplicativo da companhia aérea, antecipadamente. Qual seria o procedimento mais eficaz para capturar corretamente os dados dos comprovantes no aplicativo?

- Extrair os dados através da API do Amazon Transcribe
    - O Transcribe utiliza aprendizado de máquina (machine learning) para extrair textos de áudios e vídeos.

- **✅** Extrair os dados através da API do Amazon Textract
    - O Amazon Textract utiliza aprendizado de máquina (machine learning) para analisar os documentos, detectar e extrair texto impresso e manuscrito, dados estruturados (como campos e valores de interesse) e tabelas de imagens e digitalizações de documentos permitindo uma validação antecipada e automatizada.

- Extrair os dados através da API do Amazon Transform
    - O Transform não é um serviço presente na plataforma de ML da AWS.

- Extrair os dados através da API do Amazon Polly
    - O Polly utiliza aprendizado de máquina (machine learning) para converter textos em fala realista.

> **Explicação geral**:  
> O Amazon Textract é um serviço de machine learning da AWS que analisa documentos para detectar e extrair texto impresso e manuscrito, além de dados estruturados, como campos e valores, e tabelas de imagens e digitalizações. Ele processa esses elementos e retorna uma pontuação de confiança para cada item identificado, permitindo aos usuários avaliar a precisão dos resultados. Essa pontuação é útil para tomar decisões informadas sobre o uso dos dados extraídos, como validar informações ou direcionar documentos para diferentes processos. Por exemplo, em aplicativos de validação de documentos, as regras podem ser configuradas para agir com base nas pontuações de confiança, garantindo que apenas dados de alta precisão sejam utilizados ou, se necessário, retornando para uma revisão adicional.

---

## Pergunta 30
Correto
Para estabelecer uma infraestrutura resiliente, uma empresa busca criar duas redes isoladas em zonas de disponibilidade diferentes. Qual serviço possibilita essa implementação?

- AWS Direct Connect
    - O AWS Direct Connect permite criar uma conexão dedicada entre sua rede local e a infraestrutura da AWS, proporcionando maior largura de banda e menor latência em comparação com conexões de internet padrão. Essa conexão dedicada oferece desempenho mais consistente e seguro para acessar serviços da AWS.

- AWS VPN
    - O VPN é utilizado para estabelecer conexões virtuais entre redes e redes e redes e usuários, não para criar as redes.

- **✅** Amazon VPC
    - A Amazon VPC possibilita a criação de uma porção isolada e logicamente definida na nuvem da Amazon Web Services (AWS). Nessa área, é possível executar recursos da AWS dentro de uma rede virtual personalizada, oferecendo isolamento e controle sobre a infraestrutura na nuvem.

- Amazon Connect
    - O Connect é utilizado para implementar uma central de atendimento com IA.

> **Explicação geral**:  
> O Amazon Virtual Private Cloud (Amazon VPC) é um serviço que permite criar uma rede virtual isolada dentro da nuvem da AWS, oferecendo controle total sobre o ambiente de rede, incluindo a seleção do intervalo de endereços IP, sub-redes, tabelas de roteamento e gateways de rede. Com o Amazon VPC, você pode definir e gerenciar suas próprias configurações de rede, estabelecendo políticas de segurança granulares por meio de listas de controle de acesso (ACLs) e grupos de segurança.

> Para criar redes resilientes, o Amazon VPC permite a implementação de sub-redes em várias zonas de disponibilidade (AZs), garantindo alta disponibilidade e tolerância a falhas. Além disso, você pode configurar gateways de internet e NAT para gerenciar o tráfego de entrada e saída, bem como empregar peering de VPC para conectar redes em diferentes regiões. Essas capacidades ajudam a construir infraestruturas de rede robustas, seguras e escaláveis, essenciais para aplicações críticas e ambientes de produção.

---

## Pergunta 31
Correto
Diante de preocupações com o desempenho de uma aplicação, uma equipe decidiu substituir o banco de dados por outro de maior performance. Como pode ser realizado o processo de migração dos dados para esse novo banco de dados?

- **✅** Configurando uma instância do AWS DMS no banco de destino, criando uma tarefa de replicação indicando origem e destino, e iniciando a tarefa para uma migração contínua e em tempo real dos dados.
    - O AWS Database Migration Service (DMS) é uma ferramenta que ajuda os clientes na migração de bancos de dados, oferecendo suporte a diversas situações, como aprimoramento de discos ou mudança de gerenciador de bancos de dados. Ele simplifica o processo, permitindo a transferência eficiente e segura de dados entre diferentes ambientes, garantindo a integridade e consistência durante as migrações.

- Configurando uma instância do AWS DataSync no banco de destino, criando uma tarefa de replicação indicando origem e destino, e iniciando a tarefa para uma migração contínua e em tempo real dos dados.
    - O AWS DataSync é mais adequado para transferir grandes volumes de dados entre sistemas de armazenamento, como migrar dados entre sistemas de arquivos locais e Amazon S3, Amazon EFS ou Amazon FSx.

- Configurando uma instância do Amazon DynamoDB no banco de destino, criando uma tarefa de replicação indicando origem e destino, e iniciando a tarefa para uma migração contínua e em tempo real dos dados.
    - O DynamoDB é o serviço utilizado para implementar bancos de dados noSQL gerenciados, não para migrar os dados.

- Configurando uma instância do AWS RDS no banco de destino, criando uma tarefa de replicação indicando origem e destino, e iniciando a tarefa para uma migração contínua e em tempo real dos dados.
    - O RDS é o serviço utilizado para implementar bancos de dados relacionais gerenciados, não para migrar os dados.

> **Explicação geral**:  
> O AWS Database Migration Service (DMS) é uma ferramenta essencial para clientes que desejam realizar upgrades de performance em seus bancos de dados. Ele oferece suporte a diversas situações, como a melhoria de discos e a mudança de gerenciadores de bancos de dados, facilitando a transição para sistemas mais eficientes e poderosos. Com o DMS, o processo de migração é simplificado, permitindo a transferência segura e eficiente de dados entre diferentes ambientes, sem comprometer a integridade e a consistência dos dados. Além disso, o DMS minimiza o tempo de inatividade durante a migração, garantindo uma continuidade operacional suave e melhorando significativamente o desempenho do banco de dados.

---

## Pergunta 32
Correto
Considerando as responsabilidades do cliente e da AWS no modelo de responsabilidade compartilhada, todas as seguintes afirmações são precisas, exceto?

- A AWS mantém a configuração dos dispositivos de infraestrutura, mas o cliente é responsável pela configuração dos seus próprios bancos de dados, aplicativos e sistemas operacionais convidados.
    - Esta responsabilidade é compartilhada entre a AWS e o Cliente, cada um no seu escopo de atuação.

- **✅** a AWS mantém o datacenter global, mas o cliente é responsável por manter os hardwares dos hosts utilizados pelas suas cargas de trabalho.
    - Esta responsabilidade é apenas da AWS. O Cliente não tem acesso a hardwares de hosts.

- A AWS é responsável pela aplicação de patches e pela correção de falhas na infraestrutura, mas os clientes são responsáveis pela aplicação de patches em seu SO convidado e nos seus aplicativos.
    - Esta responsabilidade é compartilhada entre a AWS e o Cliente, cada um no seu escopo de atuação.

- A AWS treina funcionários da AWS, mas o cliente deve treinar seus próprios funcionários.
    - Esta responsabilidade é compartilhada entre a AWS e o Cliente, cada um no seu escopo de atuação.

> **Explicação geral**:  
> A AWS é responsável pelos controles físicos e pela manutenção de toda a infraestrutura global, o que inclui a gestão e segurança dos data centers e hosts utilizados pelos clientes. Essas responsabilidades são herdadas pelos clientes, o que significa que eles se beneficiam das medidas de segurança e manutenção implementadas pela AWS, mas não participam ativamente dessas atividades. A AWS garante que a infraestrutura física esteja protegida contra acessos não autorizados, desastres naturais e falhas de hardware, proporcionando um ambiente seguro e resiliente. No entanto, essa responsabilidade não é compartilhada com os clientes, que devem focar na segurança e manutenção de suas próprias aplicações e dados na camada lógica.

---

## Pergunta 33
Correto
Para que tipo de cenário o AWS IoT Greengrass é mais adequado?

- Hospedagem de sites da web.
    - Não é usado para hospedagem de sites da web, isso pode ser feito pelo S3, EC2, Elastic Beanstalk.

- Armazenamento de arquivos de mídia.
    - Não é voltado para o armazenamento de arquivos de mídia, isso pode ser feito com o S3.

- Análise de big data em lote.
    - Não é apropriado para análise de big data em lote, isso pode ser feito com o EMR

- **✅** Aplicações de IoT que exigem baixa latência e capacidade de processamento local.
    - O AWS IoT Greengrass é mais adequado para aplicações de IoT que exigem baixa latência e capacidade de processamento local.

> **Explicação geral**:  
> O AWS IoT Greengrass é mais adequado para aplicações de IoT que exigem baixa latência e capacidade de processamento local. Ele permite que dispositivos IoT executem código na borda da rede, o que é especialmente valioso em cenários onde a latência é crítica e as decisões devem ser tomadas rapidamente.

> O AWS IoT Core e o AWS IoT Greengrass são serviços relacionados, mas com finalidades e funcionalidades distintas na plataforma AWS. O AWS IoT Core é o serviço fundamental de IoT da AWS, projetado para conectar dispositivos IoT à nuvem, gerenciar sua segurança, autenticar e transmitir dados entre dispositivos e aplicativos na nuvem. Ele atua como um hub centralizado para dispositivos IoT, proporcionando conectividade segura e gerenciamento de identidade na nuvem.

> Por outro lado, o AWS IoT Greengrass é uma extensão da nuvem que permite a execução de código localmente em dispositivos IoT, na "borda" da rede. Ele fornece latência reduzida, capacidade de processamento local e lógica de negócios distribuída, o que é útil em cenários onde a latência é crítica ou a conectividade com a nuvem pode ser interrompida.

> Em resumo, enquanto o AWS IoT Core se concentra na conectividade segura entre dispositivos IoT e a nuvem, o AWS IoT Greengrass estende essa funcionalidade para permitir o processamento de dados e lógica localmente nos dispositivos, agregando valor a aplicações IoT em tempo real e com requisitos de latência baixa.

---

## Pergunta 34
Incorreto
Após uma fusão, uma empresa precisa integrar rapidamente 1000 novos colaboradores em suas instalações. Quais são as possíveis abordagens para alcançar essa integração de maneira eficiente?

- Utilizar o AWS Direct Connect configurado e implantado, fornecendo acesso seguro por meio do cliente VPN com credenciais adequadas e garantindo infraestrutura preparada para a carga de usuários.
    - O Direct Connect cria uma conexão dedicada que não trafega dados fora da infraestrutura da AWS, não está disponível para usuários finais se conectarem à AWS.

- **✅** Utilizar o AWS Client VPN configurado e implantado, fornecendo acesso seguro por meio do cliente VPN com credenciais adequadas e garantindo infraestrutura preparada para a carga de usuários.
    - O AWS Client VPN conecta seus usuários à AWS ou a recursos locais por meio de um cliente de software VPN, super adequado para o cenário apresentado.

- Utilizar o AWS Site-to-Site VPN configurado e implantado, fornecendo acesso seguro por meio do cliente VPN com credenciais adequadas e garantindo infraestrutura preparada para a carga de usuários.
    - O Site-to-Site VPN cria túneis criptografados entre a sua rede e as Amazon Virtual Private Clouds ou os AWS Transit Gateways, adequado para integrar as redes.

- Utilizar o AWS Connect configurado e implantado, fornecendo acesso seguro por meio do cliente VPN com credenciais adequadas e garantindo infraestrutura preparada para a carga de usuários.
    - O Connect permite a implementação de uma central de atendimento multi-canal e que faz uso de IA.

> **Explicação geral**:  
> O AWS VPN é composto por dois serviços principais: o AWS Site-to-Site VPN e o AWS Client VPN. O Site-to-Site VPN permite a criação de túneis criptografados entre sua rede local e as Amazon Virtual Private Clouds (VPCs) ou AWS Transit Gateways, assegurando uma conexão segura e privada entre suas instalações on-premises e os recursos da AWS. Esse serviço é ideal para empresas que precisam integrar suas redes locais com a infraestrutura da AWS de maneira segura e confiável. Por outro lado, o AWS Client VPN conecta usuários individuais à AWS ou a recursos locais através de um cliente de software VPN, proporcionando uma solução eficiente e segura para acesso remoto. Com o Client VPN, os usuários podem se conectar de qualquer lugar, garantindo a segurança e a integridade dos dados transmitidos. Ambos os serviços utilizam criptografia robusta para proteger os dados em trânsito e são altamente escaláveis, permitindo que as empresas adaptem suas necessidades de conectividade à medida que crescem. Além disso, a configuração e o gerenciamento dessas VPNs são simplificados através do console de gerenciamento da AWS, tornando a implementação de soluções de rede seguras acessível para organizações de todos os tamanhos.

---

## Pergunta 35
Correto
Um banco de investimentos opera diversos aplicativos web críticos na AWS e necessita de visibilidade e proteção contra ataques DDoS, tanto sofisticados quanto comuns. Qual serviço pode ser utilizado para atender a essa necessidade?

- **✅** Amazon Shield
    - O Amazon Shield é um serviço de segurança gerenciado da AWS projetado para proteger aplicativos contra ataques de negação de serviço distribuído (DDoS). Ele oferece proteção automatizada contra ameaças de DDoS, detectando e mitigando atividades maliciosas em tempo real.

- Amazon Macie
    - O Macie é um serviço que utiliza aprendizado de máquina (ML) para proteger seus dados confidenciais.

- Amazon Detective
    - O Detective é o serviço que gera insights a partir do tráfego de dados que ajuda a identificar a causa raiz de atividades suspeitas.

- Amazon Inspector
    - O Inspector é o serviço que gerencia vulnerabilidades através da verificação contínua das suas cargas de trabalho. Ele atribui uma pontuação de risco para indicar os itens mais prioritários.

> **Explicação geral**:  
> O Amazon Shield é um serviço de segurança gerenciado da AWS projetado para proteger aplicativos contra ataques de negação de serviço distribuído (DDoS). Ele oferece proteção automatizada contra ameaças de DDoS, detectando e mitigando atividades maliciosas em tempo real. O Shield protege não apenas os recursos da AWS, como instâncias EC2 e bancos de dados RDS, mas também serviços como o Amazon CloudFront, garantindo que os ataques DDoS não prejudiquem o desempenho ou a disponibilidade de seus aplicativos distribuídos globalmente. A abordagem do AWS Shield combina tecnologias avançadas e análise de tráfego para manter seus aplicativos seguros contra ataques de DDoS, permitindo operações confiáveis e ininterruptas.

---

## Pergunta 36
Correto
Qual serviço da AWS é um banco de dados NoSQL, totalmente gerenciado e compatível com o MongoDB?

- Route53
    - O Route53 é um serviço global de DNS utilizado para a criação e direcionamento de domínios.

- RDS
    - O RDS é o serviço de banco de dados relacionais que pode implementar diversos mecanismos de bancos de dados de mercado.

- Aurora
    - O Aurora é um banco de dados relacional, 5 x mais rápido que o MySQL.

- **✅** DocumentDB
    - O serviço DocumentDB da AWS é um banco de dados NoSQL totalmente gerenciado, compatível com MongoDB. Ele oferece escalabilidade, disponibilidade e segurança, permitindo que você execute cargas de trabalho do MongoDB sem se preocupar com a operação do banco de dados.

> **Explicação geral**:  
> O serviço Amazon DocumentDB da AWS é um banco de dados NoSQL totalmente gerenciado, compatível com MongoDB, que facilita a execução de cargas de trabalho do MongoDB na nuvem. Ele oferece escalabilidade automática, permitindo o ajuste do armazenamento e da capacidade de processamento conforme necessário, garantindo desempenho consistente. Com alta disponibilidade, o DocumentDB replica dados em várias zonas de disponibilidade, assegurando resiliência e recuperação rápida de desastres. A segurança é aprimorada com criptografia de dados em repouso e em trânsito, além de integração com o AWS Identity and Access Management (IAM) para controle de acesso detalhado. Este serviço elimina a necessidade de gerenciamento operacional, permitindo que você se concentre no desenvolvimento e na otimização de suas aplicações.

---

## Pergunta 37
Correto
Para gerenciar crédito e riscos de forma eficaz, um grande banco precisa realizar processamentos em lotes com alta performance computacional. Qual serviço pode ser utilizado para reduzir erros humanos, aumentar a velocidade e precisão, e diminuir os custos por meio da automação desses processos?

- **✅** AWS Batch
    - O AWS Batch permite que organizações automatizem a provisão de recursos e a programação de tarefas, resultando em economia de custos e acelerando a tomada de decisões.

- AWS Sagemaker
    - O AWS SageMaker é utilizado para criar, testar e implementar modelos de Machine Learning.

- AWS Step Functions
    - O AWS Step Functions é um serviço de fluxo de trabalho visual que utiliza pouco código, usado para orquestrar serviços da AWS, automatizar processos de negócios e criar aplicações sem servidor.

- AWS Kinesis
    - O AWS Kinesis é utilizado para capturar e transmitir dados em tempo real.

> **Explicação geral**:  
> A indústria de serviços financeiros adotou a computação de alto desempenho para atividades como definição de preços, posições de mercado e gerenciamento de riscos. Migrando essas cargas de trabalho intensivas em computação para a AWS, as empresas conseguiram aumentar a velocidade, escalabilidade e reduzir custos. O AWS Batch permite que essas organizações automatizem a provisão de recursos e a programação dessas tarefas, resultando em economia de custos e acelerando a tomada de decisões. Esse aumento de eficiência e rapidez também melhora o tempo de lançamento no mercado, beneficiando o desempenho geral das operações financeiras.

---

## Pergunta 38
Correto
Uma empresa deseja desenvolver uma aplicação orientada a eventos que possa ser integrada de maneira simples a outras aplicações e serviços da AWS. Qual abordagem é mais adequada para atender à arquitetura e facilitar a ágil integração dessa aplicação?

- **✅** Criar um barramento de eventos com o EventBridge.
    - O EventBridge é um barramento de eventos sem servidor que torna mais fácil a criação de aplicações orientadas por eventos em escala usando eventos gerados com base em suas aplicações, aplicações integradas de software como serviço (SaaS) e serviços da AWS.

- Criar um barramento de eventos com o CodeStar.
    - CodeStar é o serviço utilizado para gerenciar o projeto, membros e artefatos e que permite integração com o Jira.

- Criar um barramento de eventos com o Kinesis.
    - Kinesis é o serviço utilizado para capturar e transmitir dados através de streaming em tempo real.

- Criar um barramento de eventos com o CodePipeline.
    - CodePipeline é o serviço que fornece a esteira de CI/CD Continuous Integration/Continuous Delivery (Integração e Entrega Contínua) e permite a integração dos demais serviços: CodeCommit, CodeBuild e CodeDeploy.

> **Explicação geral**:  
> O AWS EventBridge é um barramento de eventos sem servidor que facilita a criação de aplicações orientadas por eventos em escala. Ele utiliza eventos gerados a partir de suas aplicações, aplicações SaaS integradas e serviços da AWS. Com o EventBridge, você pode configurar regras de roteamento para direcionar seus dados, permitindo a criação de arquiteturas de aplicações que reagem em tempo real às suas fontes de dados. O serviço permite que o consumidor e o editor de eventos sejam completamente dissociados, proporcionando flexibilidade e escalabilidade na construção de sistemas responsivos e eficientes.

---

## Pergunta 39
Correto
Uma organização pública utiliza softwares da Microsoft, Oracle e JetBrains, os quais são utilizados por mais de 1000 funcionários. A organização necessita gerenciar as licenças adquiridas desses softwares para evitar desperdícios, otimizar o uso e manter a conformidade em relação aos limites estabelecidos nos contratos com os fornecedores. Por meio de qual serviço é possível alcançar esse objetivo?

- Através do Parameter Store
    - O Parameter Store é um recurso do AWS Systems Manager que oferece armazenamento hierárquico seguro para gerenciamento de dados de configuração e gerenciamento de segredos.

- Através do Marketplace
    - O Marketplace é o portal onde você pode encontrar software prontos para diversas necessidades de negócio, além disso, se você é um desenvolvedor ou uma empresa que possui um aplicativo, você pode comercializá-lo nesta plataforma também.

- Através do Config
    - O Config é o serviço utilizado para gerenciar as configurações de serviços e aplicações permitindo conformidade e auditoria.

- **✅** Através do License Manager
    - O License Manager deve ser utilizado para gerenciar as licenças ao rastrear o seu uso, permitindo maior controle, economia de custos e conformidade com o limite de uso estabelecida em contrato com os fornecedores.

> **Explicação geral**:  
> O AWS License Manager é utilizado para gerenciar licenças ao rastrear seu uso, oferecendo maior controle, economia de custos e conformidade com os limites de uso estabelecidos em contrato com fornecedores. Ele permite que você centralize a administração das licenças de software em um único local, facilitando o monitoramento e a auditoria. Com o License Manager, você pode definir regras de licenciamento, verificar a conformidade em tempo real e evitar a compra excessiva de licenças. Além disso, ele ajuda a minimizar o risco de não conformidade e otimiza o uso dos recursos licenciados, garantindo que você utilize suas licenças de maneira eficiente e econômica.

---

## Pergunta 40
Correto
Você precisa preparar dados de várias fontes de forma rápida, simples e econômica para serem processados por um modelo de machine learning no SageMaker. Qual é o serviço de integração de dados sem servidor recomendado para essa tarefa?

- AWS DataSync
    - O AWS DataSync é utilizado para realizar a sincronização automática entre dados da infraestrutura on premise e da AWS.

- **✅** AWS Glue
    - O AWS Glue é um serviço de integração de dados com tecnologia sem servidor que torna a preparação de dados mais simples, rápida e barata. É um serviço indicado para ETL - Extrair, transformar e carregar dados.

- AWS Redshift
    - O AWS Redshift é um data warehouse escalável e totalmente gerenciado que facilita análises de Business Intelligence, permitindo consultas rápidas e complexas sobre grandes volumes de dados.

- AWS DMS
    - O AWS Database Migration Service (DMS) é utilizado para facilitar a migração de bancos de dados para a AWS de maneira segura e eficiente, minimizando o tempo de inatividade durante o processo. Além de migrar os dados, o DMS também pode realizar conversões de dados, adaptando-os ao novo formato necessário na plataforma de destino, garantindo uma transição suave e funcional.

> **Explicação geral**:  
> O AWS Glue é um serviço de integração de dados com tecnologia sem servidor que simplifica, acelera e reduz o custo da preparação de dados. Ele é ideal para processos de ETL (Extração, Transformação e Carga), permitindo que você extraia dados de várias fontes, os transforme conforme necessário e os carregue em seu destino. Com o AWS Glue, você pode automatizar a descoberta e catalogação de dados, facilitando a organização e a gestão de grandes volumes de informações. Além disso, o serviço oferece uma interface amigável e suporte para tarefas complexas de transformação de dados, tudo isso sem a necessidade de gerenciar infraestrutura, proporcionando uma solução escalável e eficiente para integrar e preparar dados para análises e machine learning no SageMaker.

---

## Pergunta 41
Correto
Uma startup deseja desenvolver um software nativo na nuvem de maneira ágil utilizando as linguagens de programação JavaScript e Kotlin. Qual ferramenta da AWS oferece diversos recursos para facilitar o desenvolvimento dessas aplicações?

- AWS CodeCommit
    - O CodeCommit é o serviço utilizado para gerenciamento do código fonte.

- AWS Elastic Beanstalk
    - O Elastic Beanstalk é o serviço utilizado para provisionar o ambiente de execução para uma aplicação ser processada.

- AWS CodeBuild
    - O CodeBuild é o serviço utilizado para compilar e testar o código fonte.

- **✅** AWS SDK
    - As AWS SDKs para JavaScript e Kotlin fornecem diversos recursos para que o time de desenvolvimento desenvolva e compile os aplicativos que serão executados na AWS com agilidade.

> **Explicação geral**:  
> O AWS SDK (Software Development Kit) é um conjunto de ferramentas que facilita a integração de aplicativos com os serviços da AWS. Ele oferece bibliotecas, exemplos de código e documentação para ajudar os desenvolvedores a criar aplicações robustas e escaláveis na nuvem da AWS. Com o AWS SDK, é possível interagir com serviços como S3, EC2, DynamoDB, entre outros, de maneira simples e eficiente.

> Além de JavaScript e Kotlin, existem AWS SDKs para diversas outras linguagens de programação, incluindo C++, Go, Java, .NET, Node.js, PHP, Python, Ruby, Rust e Swift. Esses SDKs permitem que os desenvolvedores escolham a linguagem com a qual se sentem mais confortáveis, aproveitando os recursos da AWS para criar e gerenciar suas aplicações na nuvem.

---

## Pergunta 42
Correto
Uma empresa planeja implementar o Single Sign-On (SSO) em todos os seus aplicativos. Qual benefício ela busca alcançar com essa iniciativa?

- Exigir múltiplos logins para acessar com segurança os recursos da AWS.
    - Não requer múltiplos logins, ao contrário, elimina a necessidade de vários logins.

- Autenticar usuários por meio de dispositivos móveis como duplo fator de segurança.
    - Não é uma medida de segurança específica para dispositivos móveis, nem de duplo fator.

- Criar várias contas de usuário de modo simultâneo na AWS.
    - SSO não se refere a criar várias contas de usuário.

- **✅** Permitir que os usuários efetuem login uma única vez e acessem múltiplas contas e aplicativos sem a necessidade de fazer login repetidamente.
    - Single Sign-On (SSO) na AWS significa um método que permite que os usuários façam login uma vez e acessem várias contas e aplicativos sem a necessidade de fazer login novamente, proporcionando maior conveniência e eficiência no acesso.

> **Explicação geral**:  
> O Single Sign-On (SSO) na AWS é um método de autenticação que permite aos usuários acessar várias contas e aplicativos com um único login, eliminando a necessidade de múltiplas credenciais. Com o AWS SSO, os administradores podem gerenciar o acesso a diferentes recursos e permissões centralmente, proporcionando uma experiência de login simplificada e segura. O SSO integra-se com serviços de diretório existentes, como o Microsoft Active Directory, e suporta diversos padrões de autenticação, como SAML 2.0. Isso aumenta a eficiência e a conveniência para os usuários, enquanto fortalece a segurança, pois reduz a complexidade de gerenciamento de senhas e o risco de uso de credenciais fracas ou repetidas.

---

## Pergunta 43
Correto
A fim de atender aos requisitos de performance em um ambiente híbrido, um site mantém parte de sua carga de trabalho em servidores locais e parte em instâncias EC2 na AWS. Como é possível distribuir novas versões desse site em ambos os ambientes com um serviço da AWS?

- **✅** Realizando o deploy com o CodeDeploy
    - Com o AWS CodeDeploy é possível automatizar as implantações em instâncias EC2, ECS, Lambda e também em servidores on-premises, se necessário.

- Não existe essa possibilidade
    - Isso é possível com o AWS CodeDeploy.

- Realizando o deploy com o CodePipeline
    - O AWS CodePipeline é um serviço de entrega contínua que automatiza as etapas de construção, teste e implantação de código. Ele permite a criação de pipelines personalizáveis para gerenciar e monitorar o fluxo de trabalho de desenvolvimento, integrando-se com serviços da AWS e ferramentas de terceiros. Isso garante entregas de software rápidas e confiáveis, facilitando a implementação de atualizações e novas funcionalidades.

- Realizando o deploy com o CodeStar
    - O AWS CodeStar facilita o desenvolvimento, construção e implantação rápida de aplicações na AWS, oferecendo um ambiente integrado para gerenciamento de projetos CI/CD e integração com ferramentas de projetos, como o Jira.

> **Explicação geral**:  
> O AWS CodeDeploy é um serviço que permite automatizar implantações em uma variedade de ambientes, incluindo instâncias EC2, ECS, Lambda e até mesmo servidores on-premises, se necessário. Para realizar implantações em instâncias EC2 e servidores on-premises, é obrigatório instalar um agente específico que gerencia o processo de implantação. Esse agente facilita a distribuição automatizada de código, atualizações de software e configurações de maneira eficiente e consistente. O CodeDeploy minimiza o tempo de inatividade durante as implantações e garante que as atualizações sejam feitas de forma segura e controlada. Além disso, ele oferece recursos como rollback automático em caso de falhas, integração com outros serviços da AWS e suporte a diferentes estratégias de implantação, como blue/green e canary, melhorando a flexibilidade e a robustez do ciclo de desenvolvimento e operação.

---

## Pergunta 44
Correto
Uma empresa está interessada em implementar o Amazon Translate em certos processos de traduções de textos. Quais são as opções para iniciar o uso deste serviço? (selecione 3 alternativas)

- Através do MFA
    - O MFA (Multi Factor Authentication) é um serviço utilizado para adicionar uma etapa a mais no processo de autenticação no acesso a conta e aplicativos com o Cognito, também é utilizado para incluir proteção adicional na deleção de Buckets do S3.

- **✅** Através da CLI
    - A maneira mais fácil de utilizar o serviço é através do console, da chamada do serviço diretamente da Interface da Linha de Comando da AWS ou através de uma das SDKs para integrar o serviço aos aplicativos.

- Através do IAM
    - O IAM é o serviço gerenciador de acessos de usuários e recursos das contas da AWS.

- **✅** Através das SDKs
    - A maneira mais fácil de utilizar o serviço é através do console, da chamada do serviço diretamente da Interface da Linha de Comando da AWS ou através de uma das SDKs para integrar o serviço aos aplicativos.

- **✅** Através do Console
    - A maneira mais fácil de utilizar o serviço é através do console, da chamada do serviço diretamente da Interface da Linha de Comando da AWS ou através de uma das SDKs para integrar o serviço aos aplicativos.

> **Explicação geral**:  
> O Amazon Translate é um serviço de machine learning que oferece tradução de textos entre vários idiomas suportados. Ele permite a tradução de texto de um idioma de origem para outro de destino, tanto em tempo real quanto em lotes. O serviço pode ser acessado de forma simples através do console da AWS, de chamadas diretas à API usando a Interface de Linha de Comando da AWS, ou integrando-se a aplicativos via SDKs. Essas opções facilitam a incorporação de traduções automáticas em diversas aplicações, proporcionando uma solução rápida e eficaz para necessidades de tradução de texto.

---

## Pergunta 45
Correto
O site de vendas de uma companhia aérea tem enfrentado indisponibilidades frequentes causadas pelo grande número de requisições não autorizadas feitas por bots. Quais estratégias e ferramentas de segurança podem ser implementadas para proteger o site contra essas atividades maliciosas e garantir sua disponibilidade contínua para os usuários legítimos?

- **✅** Criar regras contra explorações indevidas da Web através do WAF.
    - O AWS Web Application Firewall (WAF) é um serviço de segurança que protege aplicativos da web contra ameaças e vulnerabilidades. Ele oferece proteção avançada contra bots maliciosos por meio de regras personalizadas, listas de bloqueio e recursos de aprendizado de máquina.

- Criar regras contra explorações indevidas da Web através do Macie.
    - O Amazon Macie utiliza aprendizado de máquina (ML) para identificar e proteger dados confidenciais armazenados no S3, ajudando a automatizar a detecção de informações sensíveis e monitorar possíveis riscos de segurança.

- Criar regras contra explorações indevidas da Web através do Shield.
    - O AWS Shield é um serviço de proteção contra ataques DDoS que protege aplicações em execução, garantindo alta disponibilidade e resiliência contra ameaças de negação de serviço.

- Criar regras contra explorações indevidas da Web através do Inspector.
    - O AWS Inspector é um serviço que gerencia vulnerabilidades através da verificação contínua das suas cargas de trabalho. Ele atribui uma pontuação de risco para indicar os itens mais prioritários, facilitando a identificação e correção de vulnerabilidades críticas.

> **Explicação geral**:  
> O Web Application Firewall (WAF) é um serviço de segurança essencial que detecta e bloqueia atividades suspeitas, como scraping de dados e ataques de força bruta. Ele garante a integridade e a disponibilidade dos aplicativos para os usuários legítimos. Essa camada de proteção é eficaz contra ataques automatizados por bots, salvaguardando os aplicativos web contra vulnerabilidades exploradas por hackers. Além de minimizar riscos de segurança, o WAF filtra tráfego malicioso e permite um controle granular sobre as políticas de segurança, assegurando uma experiência de navegação segura para os usuários finais.

---

## Pergunta 46
Correto
Uma aplicação monolítica foi refatorada em microsserviços e agora precisa ser migrada para a AWS. Qual serviço da AWS deve ser utilizado para implantar e executar esses microsserviços, garantindo alta escalabilidade, resiliência e gerenciamento eficiente de contêineres?

- Amazon EC2
    - Proporciona controle total sobre a infraestrutura virtual, mas não é tão adequado para microsserviços devido à necessidade de gerenciar manualmente a escalabilidade, o balanceamento de carga e a orquestração de contêineres, tarefas que ECS automatiza de forma eficiente.

- **✅** Amazon ECS
    - O Amazon ECS oferece uma plataforma robusta para gerenciar contêineres Docker, proporcionando escalabilidade automática e integração com outros serviços AWS. ECS facilita o deployment, gerenciamento e escalonamento de microsserviços, garantindo alta disponibilidade e resiliência da aplicação.

- AWS Elastic Beanstalk
    - Simplifica a implantação de aplicativos web, mas oferece menos controle e flexibilidade para arquiteturas de microsserviços complexas em comparação com ECS.

- AWS Lambda
    - Executa código serverless em resposta a eventos, mas não é ideal para microsserviços complexos devido às limitações de tempo de execução e ao gerenciamento de estado.

> **Explicação geral**:  
> O Amazon ECS (Elastic Container Service) é um serviço da AWS projetado para implantar e gerenciar microsserviços altamente escaláveis em contêineres. Ele simplifica a execução de aplicativos em contêineres, eliminando a necessidade de gerenciar a infraestrutura subjacente. O ECS oferece suporte tanto para clusters gerenciados pela AWS quanto para clusters autogerenciados, proporcionando flexibilidade e controle conforme necessário. Com integração nativa com outros serviços da AWS, como IAM, CloudWatch, e VPC, o ECS facilita a implementação de arquiteturas seguras e monitoráveis. Além disso, o ECS suporta o escalonamento automático de contêineres, garantindo que suas aplicações possam lidar com variações de carga de forma eficiente. Isso torna o ECS uma escolha robusta para empresas que buscam executar microsserviços em um ambiente de contêineres de maneira escalável e confiável.

---

## Pergunta 47
Correto
Uma empresa busca aprimorar o desempenho e diminuir os custos de uma aplicação que faz uso intenso de dados. Como é viável minimizar as operações de entrada e saída nos bancos de dados para atingir esse objetivo?

- **✅** Implementando o ElastiCache entre a aplicação e o banco de dados
    - Com o ElastiCache é possível armazenar os dados da aplicação em cache e descarregar a E/S do banco de dados para reduzir a carga operacional, reduzir os custos e melhorar o desempenho do banco de dados e da aplicação.

- Implementando o CloudSearch entre a aplicação e o banco de dados
    - Não é viável usar Amazon CloudSearch para minimizar operações de E/S em bancos de dados porque CloudSearch é projetado para facilitar a pesquisa e indexação de dados em aplicativos, não para gerenciar transações ou armazenar dados de forma persistente.

- Implementando o Lambda entre a aplicação e o banco de dados
    - Não é viável usar AWS Lambda para minimizar operações de E/S em bancos de dados porque Lambda é projetado para executar código em resposta a eventos, com tempo de execução limitado e sem estado persistente. Embora possa ser usado para processar eventos e dados em tempo real, não é adequado para gerenciar transações ou operações contínuas de banco de dados que requerem persistência e longos tempos de execução.

- Implementando o Kinesis entre a aplicação e o banco de dados
    - Não é viável usar Amazon Kinesis para minimizar operações de E/S em bancos de dados porque Kinesis é projetado para ingestão e processamento de streams de dados em tempo real, não para gerenciamento de transações e armazenamento persistente.

> **Explicação geral**:  
> O Amazon ElastiCache é um serviço gerenciado de cache na memória que permite armazenar dados da aplicação em cache, aliviando a carga do banco de dados principal. Utilizando motores de cache populares como Redis e Memcached, o ElastiCache oferece alta performance e baixa latência, tornando-o ideal para cenários que exigem respostas rápidas, como sessões de usuário, páginas da web dinâmicas e cálculos em tempo real. Ao descarregar a E/S do banco de dados, ele reduz significativamente a carga operacional, permitindo que o banco de dados principal foque em operações críticas. Isso não só melhora o desempenho geral da aplicação, mas também reduz custos operacionais ao minimizar a necessidade de aumentar a capacidade do banco de dados. Com a escalabilidade automática do ElastiCache, as aplicações podem facilmente se adaptar a aumentos repentinos de demanda, mantendo a eficiência e a rapidez. Além disso, como é um serviço gerenciado, o ElastiCache simplifica a administração com monitoramento contínuo, backups automáticos e recuperação de falhas, garantindo alta disponibilidade e confiabilidade para suas aplicações.

---

## Pergunta 48
Correto
Uma organização precisa estabelecer um processo para troca de arquivos de dados entre o seu ambiente on-premises e a AWS. De que maneira esse processo pode ser implementado?

- **✅** Configurando um agente AWS DataSync tanto no ambiente local quanto na AWS e criando as tarefas de transferência.
    - O AWS DataSync é um serviço online seguro que automatiza e acelera a movimentação de dados entre serviços de armazenamento on-premises e da AWS.

- Configurando um agente AWS DMS tanto no ambiente local quanto na AWS e criando as tarefas de transferência.
    - O AWS DMS - Data Migration Service é utilizado para migrar bancos de dados mantendo a disponibilidade e consistências dos mesmos.

- Configurando um agente AWS Glue tanto no ambiente local quanto na AWS e criando as tarefas de transferência.
    - O AWS Glue é o serviço utilizado para realizar ETL (Extrair, Transformar e Carregar arquivos) na AWS.

- Configurando um agente AWS Glacier tanto no ambiente local quanto na AWS e criando as tarefas de transferência.
    - O AWS Glacier é uma categoria de armazenamento do S3 utilizado para dados armazenar dados que são poucas vezes acessados e que permitem um tempo de resposta menos otimizado na sua recuperação.

> **Explicação geral**:  
> O AWS DataSync é um serviço online seguro que automatiza e acelera a movimentação de dados entre serviços de armazenamento on-premises e da AWS. O DataSync pode copiar dados entre compartilhamentos do Network File System (NFS), Server Message Block (SMB), Sistema de Arquivos Distribuídos do Hadoop (HDFS), armazenamento de objetos autogerenciado, AWS Snowcone, buckets do Amazon Simple Storage Service (Amazon S3), sistemas de arquivos do Amazon Elastic File System (Amazon EFS), sistemas de arquivos do Amazon FSx for Windows File Server, sistemas de arquivos do Amazon FSx for Lustre e sistema de arquivos do Amazon FSx for OpenZFS.

---

## Pergunta 49

Correto
O CTO de uma empresa requisitou a adesão a um plano de suporte que garanta respostas da AWS em menos de 15 minutos para incidentes que causem inatividade nos sistemas essenciais ao negócio. Qual seria o plano de suporte recomendado para atender a esse SLA?

- Business
    - O plano Enterprise On-Ramp oferece uma resposta garantida em menos de 1 hora.

- Developer
    - O plano Developer oferece respostas para sistema afetado em menos de 12 horas.

- Enterprise On-ramp
    - O plano Enterprise On-Ramp oferece uma resposta garantida em menos de 30 minutos.

- **✅** Enterprise
    - O plano Enterprise é a única opção de suporte que oferece uma resposta garantida em menos de 15 minutos.

> **Explicação geral**:  
> O plano Enterprise é a única opção de suporte que oferece uma resposta garantida em menos de 15 minutos da AWS. Optar por este plano significa que, em situações críticas ou emergenciais, você pode contar com uma assistência extremamente rápida, com uma equipe especializada da AWS pronta para fornecer suporte em questões importantes. Esse nível de resposta ágil é particularmente crucial para organizações que precisam de uma solução de suporte de alto desempenho para manter a disponibilidade e confiabilidade de suas operações na nuvem.

---

## Pergunta 50
Correto
Um desenvolvedor de um aplicativo backend deseja permitir que outros sistemas acessem dados online de forma segura por meio de APIs. Quais são as melhores práticas que podem ser utilizadas para realizar essas integrações de maneira segura?

- **✅** A utilização do API Gateway
    - O API Gateway é um serviço que permite a criação, publicação, manutenção, monitoração e proteção de APIs. As APIs funcionam como a “porta de entrada” para aplicativos acessarem dados, lógica de negócios ou funcionalidade de seus serviços de back-end.

- A utilização do Managed Services
    - O AWS Managed Services (AMS) oferece recursos proativos, preventivos e de detecção para elevar o nível operacional e reduzir riscos, sem comprometer a agilidade. Ele permite que as empresas se concentrem na inovação e reduzam os custos operacionais.

- A utilização de funções Lambdas
    - O AWS Lambda é um serviço que permite implementar funções sem servidor usando várias linguagens de programação para diversos usos de backend. Para expor essas funções a outros consumidores, é necessário utilizar o API Gateway.

- A utilização de certificados digitais do Certificate Manager
    - O AWS Certificate Manager é usado para gerenciar e provisionar certificados SSL/TLS, garantindo a criptografia dos dados transmitidos entre servidores e clientes.

> **Explicação geral**:  
> O API Gateway é ideal para desenvolvedores que desejam compartilhar dados do backend de forma segura e eficiente. Ele permite a criação, publicação, manutenção e monitoração de APIs, atuando como uma "porta de entrada" para acessar dados e lógica de negócios. Com recursos avançados de segurança, como autenticação e proteção contra ataques DDoS, o API Gateway garante que apenas usuários autorizados possam acessar as APIs. Além disso, ele oferece escalabilidade automática para lidar com picos de tráfego, assegurando alta disponibilidade e desempenho consistente, simplificando a integração entre sistemas e serviços.

---

## Pergunta 51
Correto
Periodicamente, uma equipe de desenvolvimento replica arquivos e dados de produção do S3 para realizar testes em aplicações em outros ambientes. Qual serviço é ideal para monitorar esses dados sensíveis, prevenindo sua exposição tanto nesses contextos de teste quanto em outros ambientes?

- WAF
    - O WAF é o serviço recomendado para atuar contra explorações comuns da Web e bots que podem afetar a disponibilidade pelo consumo excessivo de chamadas.

- Inspector
    - O Inspector é o serviço que gerencia vulnerabilidades através da verificação contínua das suas cargas de trabalho. Ele atribui uma pontuação de risco para indicar os itens mais prioritários.

- **✅** Macie
    - O AWS Macie é um serviço de segurança que utiliza aprendizado de máquina para identificar e proteger dados confidenciais e sensíveis em sua infraestrutura. Ele escaneia automaticamente os dados armazenados no Amazon S3 em busca de informações parametrizadas como restritas.

- Shield
    - O Shield é um serviço de proteção contra DDoS que protege as aplicações em execução.

> **Explicação geral**:  
> O AWS Macie é um serviço de segurança que utiliza aprendizado de máquina para identificar e proteger dados confidenciais e sensíveis em sua infraestrutura. Ele escaneia automaticamente os dados armazenados no Amazon S3 em busca de informações como números de cartões de crédito, números de identificação pessoal e outros dados sensíveis. O Macie ajuda a proteger dados de clientes e produtos ao alertar sobre potenciais vazamentos ou exposições não autorizadas, permitindo que as empresas tomem medidas rápidas para mitigar riscos. Isso é crucial para garantir a conformidade com regulamentações de privacidade e manter a confiança dos clientes.

---

## Pergunta 52
Correto
Com o intuito de reforçar a segurança de suas cargas de trabalho, uma empresa planeja fazer uso das verificações abrangentes do AWS Trusted Advisor. Todos os planos de suporte incluem essas verificações, com exceção de qual?

- Business
    - O Business oferece verificações completas e abrangentes de segurança.

- Enterprise
    - O Enterprise oferece verificações completas e abrangentes de segurança.

- Enterprise On-ramp
    - O Enterprise On-ramp oferece verificações completas e abrangentes de segurança.

- **✅** Developer
    - O Developer oferece verificações básicas de segurança.

> **Explicação geral**:  
> As verificações de segurança do AWS Trusted Advisor variam conforme o plano de suporte da AWS contratado. No Plano Básico, há acesso limitado a verificações básicas, sem suporte técnico abrangente. O Plano Developer inclui todas as verificações básicas e suporte técnico durante o horário comercial. O Plano Business oferece todas as verificações básicas e abrangentes, com suporte técnico 24/7, acesso a especialistas e resposta rápida para incidentes críticos. O Plano Enterprise e Enterprise On-Ramp proporcionam o nível mais alto de suporte, incluindo todas as verificações do Trusted Advisor, revisões de arquitetura e gestão de conta dedicada. Esses planos garantem que as organizações possam utilizar as recomendações do Trusted Advisor para manter a segurança, eficiência e conformidade de suas infraestruturas na AWS, recebendo o nível de assistência necessário para suas necessidades específicas.

---

## Pergunta 53
Correto
A AWS tem ajudado os clientes que precisam implantar aplicações com requisitos de baixa latência ou com processamento de dados em data centers locais. Qual serviço fornece racks de computação e armazenamento para que os clientes possam executar tarefas de computação e armazenamento on-premises?

- Zonas locais da AWS
    - O AWS Local Zones é uma espécie de implantação de infraestrutura que posiciona a computação, armazenamento, banco de dados e outros produtos seletos da AWS perto do público em geral e dos centros industriais.

- AWS Spot
    - Spot é um modelo de uso de instâncias EC2 que permite aproveitar a capacidade não utilizada do EC2 na Nuvem AWS, oferecendo descontos de até 90% comparadas a outros modelos.

- **✅** AWS Outposts
    - O AWS Outposts são racks de computação e armazenamento totalmente gerenciados e configuráveis, criados com hardware desenvolvido pela AWS para que os clientes possam executar tarefas de computação e armazenamento on-premises.

- AWS Direct Connect
    - O AWS Direct Connect é o caminho mais curto para seus recursos na AWS. Seu tráfego de rede permanece todo o tempo na rede global da AWS e nunca entra na Internet pública. Isso reduz as probabilidades de gargalos ou aumentos inesperados de latência.

> **Explicação geral**:  
> O AWS Outposts é uma solução que oferece racks de computação e armazenamento totalmente gerenciados, utilizando hardware da AWS, para permitir que os clientes executem tarefas de computação e armazenamento localmente em suas instalações. Essa solução é ideal para cargas de trabalho que exigem baixa latência ou que devem permanecer on-premises por motivos de conformidade ou segurança. Além de suportar operações locais, o AWS Outposts facilita a integração com a vasta gama de serviços da AWS na nuvem, proporcionando uma experiência híbrida coesa. Isso permite que os clientes mantenham consistência entre suas cargas de trabalho on-premises e na nuvem, aproveitando os mesmos serviços e APIs da AWS, simplificando a gestão e a operação de seus ambientes híbridos.

---

## Pergunta 54
Correto
Sua empresa precisa criar APIs RESTful altamente escaláveis para facilitar integrações entre diversos aplicativos, garantindo segurança, gerenciamento de tráfego, monitoramento e controle de acesso. Qual serviço da AWS oferece a melhor solução para implementar essas APIs, permitindo também integração com outros serviços da AWS e suporte para milhares de solicitações simultâneas?

- Amazon CloudFront
    - É um serviço de distribuição de conteúdo (CDN) que acelera a entrega de sites, APIs e outros conteúdos, mas não é projetado para criar e gerenciar APIs RESTful.

- AWS AppSync
    - Facilita a criação de APIs GraphQL para sincronização de dados em tempo real, mas não é otimizado para APIs RESTful e integração direta com serviços como API Gateway.

- Elastic Load Balancing (ELB)
    - Distribui automaticamente o tráfego de entrada entre várias instâncias EC2, mas não oferece funcionalidades específicas para criação, gerenciamento e monitoramento de APIs RESTful.

- **✅** Amazon API Gateway
    - O Amazon API Gateway permite a criação, implantação e gerenciamento de APIs RESTful escaláveis, oferecendo controle de tráfego, segurança e monitoramento integrado. Ele se integra perfeitamente com outros serviços AWS, como Lambda e DynamoDB, e suporta milhares de solicitações simultâneas, garantindo alta disponibilidade e desempenho.

> **Explicação geral**:  
> O Amazon API Gateway é um serviço totalmente gerenciado que simplifica a criação, implantação e gerenciamento de APIs RESTful. Ele oferece escalabilidade automática para lidar com altas cargas de tráfego, garantindo desempenho consistente. Além disso, o API Gateway fornece funcionalidades robustas de autenticação e autorização para proteger suas APIs, bem como caching integrado para melhorar a eficiência e reduzir a latência. O serviço também permite a transformação de dados, facilitando a integração entre diferentes sistemas e formatos de dados. Com suporte para monitoramento e logging detalhados, o API Gateway assegura visibilidade e controle sobre o tráfego de suas APIs, integrando-se perfeitamente com outros serviços da AWS.

---

## Pergunta 55
Correto
Uma organização utiliza o Parameter Store para armazenar valores de parâmetros, como senhas, strings de banco de dados, IDs de Amazon Machine Images (AMIs) e códigos de licença. As senhas necessitam passar por um ciclo de atualização automática a cada 6 meses. A que serviço o Parameter Store deve ser vinculado para realizar essa integração?

- Ao Config
    - O Config é o serviço utilizado para gerenciar as configurações de serviços e aplicações permitindo conformidade e auditoria.

- Ao Managed Services
    - O Managed Services é o serviço que fornece recursos proativos, preventivos e de detecção que elevam o nível operacional e ajudam a reduzir riscos sem restringir a agilidade, permitindo que você se concentre na inovação e reduza o custo operacional da sua empresa.

- Ao License Manager
    - O License Manager deve ser utilizado para gerenciar as licenças ao rastrear o seu uso, permitindo maior controle, economia de custos e conformidade com o limite de uso estabelecido em contrato com os fornecedores.

- **✅** Ao Secrets Manager
    - O Secrets Manager tem a função de gerenciar, recuperar e alternar credenciais de acesso a banco de dados, chaves de API e outros segredos ao longo de seus ciclos de vida. Com esse serviço é possível programar a alteração das credenciais sem interromper o uso dos serviços.

> **Explicação geral**:  
> O Secrets Manager é responsável por gerenciar, recuperar e alternar credenciais de acesso a bancos de dados, chaves de API e outros segredos ao longo de seus ciclos de vida. Esse serviço permite que você programe a atualização das credenciais de forma automática, garantindo que as mudanças ocorram sem interromper o funcionamento dos serviços. Isso facilita a manutenção da segurança e a gestão das credenciais de acesso, mantendo os dados protegidos e acessíveis conforme necessário.

---

## Pergunta 56
Correto
Qual dos seguintes não é um tipo de diretório oferecido pelo AWS Directory Service?

- Simple AD.
    - O AWS Directory Service simplifica o gerenciamento de identidades e oferece opções como Microsoft AD gerenciado, AD Connector e Simple AD para atender às necessidades de diferentes casos de uso de diretório.

- Microsoft Active Directory (AD) gerenciado.
    - O AWS Directory Service simplifica o gerenciamento de identidades e oferece opções como Microsoft AD gerenciado, AD Connector e Simple AD para atender às necessidades de diferentes casos de uso de diretório.

- **✅** Simple Storage Service (S3).
    - O Simple Storage Service (S3) não é um tipo de diretório oferecido pelo AWS Directory Service, esse é um serviço para armazenamento de objetos (arquivos + metadados) para diversas finalidades na nuvem.

- AD Connector.
    - O AWS Directory Service simplifica o gerenciamento de identidades e oferece opções como Microsoft AD gerenciado, AD Connector e Simple AD para atender às necessidades de diferentes casos de uso de diretório.

> **Explicação geral**:  
> O AWS Directory Service é um serviço da Amazon Web Services que fornece soluções de diretório gerenciado na nuvem para autenticação e autorização de usuários em ambientes de nuvem e locais. Ele facilita a integração com diretórios existentes, como o Microsoft Active Directory (novo EntraID), permitindo que as empresas mantenham um gerenciamento unificado de identidades e acesso. O serviço oferece opções como o Microsoft AD gerenciado, que fornece uma versão gerenciada do Active Directory, o AD Connector, que integra-se a um Active Directory on-premises, e o Simple AD, uma solução de diretório simples e leve. Essas opções permitem às organizações gerenciar usuários, grupos e políticas de segurança de forma escalável e segura, simplificando a administração e a implantação de diretórios na nuvem.

---

## Pergunta 57

Correto
Quais serviços da AWS podem ser utilizados para implementar soluções avançadas de inteligência artificial em centrais de atendimento, visando melhorar a interação com os clientes, aumentar a eficiência dos atendentes e obter insights detalhados a partir das conversas? (selecione 2 alternativas)

- AWS Direct Connect
    - O Direct Connect é o serviço para criar conexões dedicadas utilizando a infraestrutura da AWS.

- AWS Marketplace
    - O Marketplace é o serviço para as empresas e desenvolvedores autônomos venderem e comprarem soluções desenvolvidas na AWS.

- **✅** AWS Contact Center Intelligence (CCI)
    - Caso a empresa já possua uma central de atendimento e só precise melhorá-la com o uso da inteligência artificial, recomenda-se o uso do AWS Contact Center Intelligence (CCI).

- **✅** Amazon Connect
    - Caso a empresa não possua uma central de atendimento, o Amazon Connect é o serviço ideal para a implementação de uma central multi-canal.

- AWS Organizations
    - O Organizations é o serviço utilizado para integrar contas e custos.

> **Explicação geral**:  
> Se a empresa ainda não possui uma central de atendimento, o Amazon Connect é o serviço ideal para implementar uma central multi-canal eficiente. Ele permite a criação de um contact center com funcionalidades de voz, chat, e outros canais, tudo integrado na nuvem da AWS.
> Amazon Connect
> Se a empresa já tem uma central de atendimento e deseja aprimorá-la com inteligência artificial, o AWS Contact Center Intelligence (CCI) é a solução recomendada. O CCI oferece ferramentas de IA que podem ser integradas à central existente para melhorar a experiência do cliente, aumentar a produtividade dos atendentes e fornecer insights valiosos a partir das interações.

---

## Pergunta 58
Incorreto
Considerando-se que o pilar de Otimização de Custos do Well-Architected Framework se concentra em evitar custos desnecessários, quais são seus tópicos principais?

- automação de alterações, reação a eventos e definição de padrões para gerenciar as operações diárias
    - Refere-se a Excelência Operacional.

- seleção dos tipos e tamanhos certos dos recursos otimizados para os requisitos de workload, monitoramento de performance e manutenção da eficiência à medida que as necessidades comerciais evoluem
    - Refere-se ao pilar Eficiência de Performance.

- **✅** compreensão dos gastos ao longo do tempo e controle da alocação de fundos, seleção do tipo e quantidade certa de recursos e dimensionamento para atender às necessidades de negócios sem gastos excessivos
    - Refere-se ao pilar Otimização de Custos.

- modelo de responsabilidade compartilhada para sustentabilidade, compreensão do impacto e maximização da utilização para minimizar os recursos necessários e reduzir os impactos posteriores
    - Refere-se ao pilar de Sustentabilidade.

> **Explicação geral**:  
> Os principais tópicos do pilar de Otimização de Custos do AWS Well-Architected Framework incluem a compreensão detalhada dos gastos ao longo do tempo e o controle rigoroso da alocação de fundos. É essencial selecionar o tipo e a quantidade adequados de recursos para evitar despesas desnecessárias. Além disso, o dimensionamento correto é crucial para atender às necessidades de negócios sem incorrer em custos excessivos. A implementação de monitoramento e relatórios financeiros contínuos ajuda a identificar e corrigir ineficiências. Ao aplicar esses princípios, as organizações podem maximizar o retorno sobre investimento e garantir uma gestão financeira eficaz na nuvem.

---

## Pergunta 59
Correto
Uma empresa deseja manter seus escritórios conectados a aplicativos na AWS com a melhor performance possível. Qual serviço poderá atendê-la?

- Amazon Connect
    - O Connect deve ser utilizado para a criação de uma central de atendimento multi-canais com inteligência artificial.

- AWS WAF
    - O WAF é o serviço recomendado para atuar contra explorações comuns da Web e bots que podem afetar a disponibilidade pelo consumo excessivo de chamadas.

- Amazon Macie
    - O Macie é um serviço que utiliza machine learning para proteger dados confidenciais.

- **✅** Amazon Direct Connect
    - O Amazon Direct Connect é mais rápido do que conexões de Internet padrão devido à sua natureza de conexão direta e dedicada. Ele estabelece uma ligação física privada entre a infraestrutura da AWS e o ambiente local, reduzindo a latência e a variação no tráfego.

> **Explicação geral**:  
> O Amazon Direct Connect supera as conexões de Internet padrão por ser uma conexão direta e dedicada. Ele cria uma ligação física privada entre a infraestrutura da AWS e o ambiente local, diminuindo a latência e a variação no tráfego. Com isso, proporciona maior previsibilidade e desempenho consistente, evitando a congestão da Internet pública. O Direct Connect disponibiliza uma largura de banda dedicada e escalável, sem compartilhamento de recursos com outros usuários, assegurando uma experiência de rede mais rápida, confiável e com baixa latência para acessar os serviços da AWS.

---

## Pergunta 60
Incorreto
Uma diretora de operações precisa de um relatório detalhado sobre todos os serviços que possuem backups, incluindo seus períodos de retenção correspondentes. Como isso pode ser obtido de forma eficiente?

- **✅** Resposta correta: Através do console da AWS, navegue até o AWS Backup e visualize os backups existentes e verifique os períodos de retenção.

- Através do AWS Backup, navegue até o AWS Config e visualize os backups existentes e verifique os períodos de retenção.

- Sua resposta está incorreta: Através do AWS Config, navegue até o AWS Backup e visualize os backups existentes e verifique os períodos de retenção.

- Através do AWS Backup, navegue até o AWS Parameter Store e visualize os backups existentes e verifique os períodos de retenção.

> **Explicação geral**:  
> O AWS Backup é o serviço que permite a criação de planos de backup com regras e políticas para diversos serviços da AWS. Com ele também é possível extrair relatórios sobre todos os backups controlados pelo plano. Se os backups foram feitos sem um plano, é provável que a geração de um relatório se torne muito mais complexa.

---

## Pergunta 61
Correto
Uma empresa planeja lançar um aplicativo móvel com autenticação federada pelas principais redes sociais do mercado. Qual é a abordagem recomendada para implementar essa funcionalidade?

- **✅** Utilizar o SDK Cognito para facilitar a autenticação em seu aplicativo.
    - O SDK Amazon Cognito é uma biblioteca que simplifica a integração de aplicativos com os serviços do Cognito, oferecendo funcionalidades como autenticação de usuários, gerenciamento de credenciais e sincronização de dados de forma eficiente.

- Utilizar o SDK Guard Duty para facilitar a autenticação em seu aplicativo.
    - O Guard Duty é um serviço de detecção de ameaças que monitora continuamente suas contas e workloads da AWS para detectar atividade maliciosa, malwares, etc.

- Utilizar o SDK Connect para facilitar a autenticação em seu aplicativo.
    - O Connect é o serviço utilizado para a implementação de uma central de atendimento multi-canal.

- Utilizar o SDK Managed Services para facilitar a autenticação em seu aplicativo.
    - O Managed Services é o serviço que fornece recursos proativos, preventivos e de detecção que elevam o nível operacional e ajudam a reduzir riscos sem restringir a agilidade, permitindo que você se concentre na inovação e reduza o custo operacional da sua empresa. Contempla segurança, gerenciamento de incidentes, automação, redução de custos e acesso a especialistas da AWS.

> **Explicação geral**:  
> O Amazon Cognito fornece autenticação, autorização e gerenciamento de usuários para suas aplicações Web e móveis. Seus usuários podem fazer login diretamente com um nome de usuário e uma senha ou por meio de terceiros, como o Facebook, a Amazon, o Google ou a Apple. Permite login social com Facebook, Google, Login with Amazon e Iniciar sessão com a Apple, bem como por meio de provedores de identidade SAML e OIDC a partir do seu grupo de usuários. O SDK Amazon Cognito é uma biblioteca que simplifica a integração de aplicativos com os serviços do Cognito, oferecendo funcionalidades como autenticação de usuários, gerenciamento de credenciais e sincronização de dados de forma eficiente. Ele facilita o desenvolvimento de aplicativos seguros e escaláveis com recursos de autenticação federada. Além de fornecer um serviço de autenticação robusto para aplicativos móveis, o Amazon Cognito permite o salvamento de dados num banco local de chave-valor para depois realizar o sincronismo entres os aplicativos.

---

## Pergunta 62

Correto
Qual serviço da AWS permite que um time de desenvolvimento implante e escale aplicativos web de forma simplificada, abstraindo a complexidade da gestão de infraestrutura e permitindo foco total no código e nas funcionalidades do aplicativo?

- Amazon EC2
    - O Amazon EC2 oferece instâncias de servidores virtuais que exigem a configuração manual de todos os componentes de infraestrutura, como balanceamento de carga e autoescalamento, exigindo mais esforço e conhecimento técnico para gerenciar e operar a infraestrutura.

- AWS Lambda
    - O AWS Lambda é adequado para executar funções específicas em resposta a eventos e possui limitações de tempo de execução e recursos, tornando-o menos adequado para aplicativos web complexos ou de longa duração.

- Amazon EKS (Elastic Kubernetes Service)
    - O Amazon EKS (Elastic Kubernetes Service) é uma solução para gerenciar clusters Kubernetes, que oferece grande flexibilidade e controle para implantar aplicativos em contêineres. No entanto, EKS exige um conhecimento mais profundo de Kubernetes e gerenciamento de contêineres, tornando-o mais adequado para equipes com experiência em DevOps e que necessitam de personalização e controle detalhado sobre o ambiente de execução.

- **✅** AWS Elastic Beanstalk
    - O AWS Elastic Beanstalk é um serviço gerenciado que automatiza o provisionamento, o monitoramento e o dimensionamento da infraestrutura necessária para hospedar aplicativos web. Ele abstrai a complexidade da configuração de servidores, balanceamento de carga, autoescalamento e monitoramento, permitindo que os desenvolvedores se concentrem no desenvolvimento de código e na lógica de negócios.

> **Explicação geral**:  
> O AWS Elastic Beanstalk é um serviço que facilita a implantação, gestão e escalabilidade de aplicativos web na nuvem. Ele oferece uma plataforma intuitiva e gerenciada, permitindo que os desenvolvedores foquem no código e nas funcionalidades do aplicativo, sem a necessidade de gerenciar a infraestrutura subjacente. O serviço cuida automaticamente de servidores, balanceamento de carga, autoescalamento e monitoramento, tornando o processo de hospedagem mais eficiente e acessível. Elastic Beanstalk suporta várias linguagens de programação e frameworks, proporcionando flexibilidade e rapidez na entrega de aplicações web. Com ele, as equipes podem rapidamente implementar novas versões e ajustar os recursos conforme a demanda.

---

## Pergunta 63
Correto
Uma organização busca implantar dashboards interativos que possibilitem que todos os colaboradores compreendam seus dados por meio de perguntas formuladas em linguagem natural. Qual serviço pode ser empregado para atender a essa finalidade?

- Athena
    - O Amazon Athena é um serviço de consulta interativo que permite analisar dados diretamente no Amazon S3 usando SQL, sem a necessidade de infraestrutura de servidor, facilitando consultas rápidas e escaláveis a grandes volumes de dados.

- **✅** Amazon QuickSight
    - O Amazon QuickSight permite que todos em sua organização entendam seus dados por meio de perguntas em linguagem natural, do uso de painéis interativos (dashboards) ou procurando automaticamente padrões e discrepâncias com tecnologia de machine learning.

- Amazon EMR (Elastic MapReduce)
    - O Amazon EMR (Elastic MapReduce) é um serviço gerenciado que facilita o processamento e análise de grandes volumes de dados utilizando frameworks como Apache Hadoop, Spark, HBase e Presto. Ele permite a criação de clusters escaláveis para executar tarefas de big data de maneira eficiente e econômica.

- Amazon Kinesis
    - O Amazon Kinesis é um serviço de processamento de dados em tempo real que permite a coleta, processamento e análise contínua de grandes fluxos de dados em tempo real, facilitando a obtenção de insights imediatos e ações rápidas.

> **Explicação geral**:  
> O Amazon QuickSight capacita toda a sua organização a compreender dados de maneira intuitiva. Ele permite que os usuários façam perguntas em linguagem natural para obter insights rápidos e precisos. Além disso, oferece painéis interativos que facilitam a visualização e análise de informações. Com a tecnologia de machine learning, o QuickSight pode identificar automaticamente padrões e discrepâncias nos dados, proporcionando uma análise avançada e detalhada sem a necessidade de conhecimentos técnicos profundos. Dessa forma, todos, desde analistas até executivos, podem tomar decisões informadas com base em dados concretos.

---

## Pergunta 64
Correto
A equipe de operações de uma empresa gerencia cargas de trabalho em um ambiente híbrido que abrange AWS, Azure e infraestrutura on-premises. Como a AWS pode contribuir para a centralização e automação das atividades de gerenciamento de operações, aplicações, alterações e nós nesse ambiente diversificado?

- **✅** Através do Hub de Operações do Systems Manager
    - O Hub de Operações do Systems Manager fornece uma interface unificada para gerenciar recursos na AWS, Azure e on-premises. Ele permite a automação de tarefas operacionais, como patches de segurança, inventário de software e compliance de configuração.

- Através do Hub de Operações do Managed Services
    - O Managed Services é o serviço que fornece recursos proativos, preventivos e de detecção que elevam o nível operacional e ajudam a reduzir riscos sem restringir a agilidade, permitindo que você se concentre na inovação e reduza o custo operacional da sua empresa. Contempla segurança, gerenciamento de incidentes, automação, redução de custos e acesso a especialistas da AWS.

- Através do Hub de Operações do Parameter Store
    - O Parameter Store faz parte do Systems Manager mas só tem função de gerenciar parâmetros, não o Hub.

- Através do Hub de Operações do Config
    - Config é o serviço utilizado para gerenciar as configurações de serviços e aplicações permitindo conformidade e auditoria.

> **Explicação geral**:  
> O Hub de Operações do AWS Systems Manager é uma interface centralizada que facilita o gerenciamento e monitoramento das operações de TI em ambientes híbridos. Ele integra várias ferramentas de operações em um único painel, permitindo que as equipes de operações visualizem e gerenciem recursos tanto na AWS quanto em ambientes on-premises e outros provedores de nuvem, como Azure. Com essa integração, o Hub de Operações detecta problemas, automatiza tarefas de manutenção e coordena respostas a incidentes, melhorando a eficiência operacional. Além disso, garante a conformidade com políticas e normas, oferecendo visibilidade unificada sobre a saúde e o desempenho dos recursos em ambientes complexos e distribuídos, simplificando a administração e operação de infraestruturas híbridas.

---

## Pergunta 65
Correto
Uma empresa deseja utilizar o Amazon S3 na AWS para armazenar arquivos gerados por suas aplicações em um ambiente on-premises. Quais são as maneiras de realizar essa integração?

- Com o uso do Parameter Store
    - O Parameter Store é um recurso do AWS Systems Manager que oferece armazenamento hierárquico seguro para gerenciamento de dados de configuração e gerenciamento de segredos.

- **✅** Com o uso do Storage Gateway
    - O Storage Gateway é um serviço de armazenamento em nuvem híbrida que permite que soluções no ambiente on-premises façam uso do armazenamento em cloud praticamente sem limites. Pode armazenar backups, data lakes, etc.

- Com o uso do Backup
    - O Backup é o serviço que permite a criação de planos de backup com regras e políticas para diversos serviços da AWS.

- Com o uso do EFS
    - O EFS é o serviço utilizado para implementar um sistema de arquivos. Pode ser utilizado em aplicações ou sistemas que foram construídos utilizados esse mecanismo de armazenamento.

> **Explicação geral**:  
> O Storage Gateway é um serviço de armazenamento em nuvem híbrida que facilita a integração entre soluções on-premises e o armazenamento em cloud da AWS, oferecendo armazenamento quase ilimitado. Ele é ideal para armazenar backups, data lakes e outros tipos de dados, permitindo que as empresas aproveitem a escalabilidade e a flexibilidade da nuvem sem abandonar suas infraestruturas locais.

---