# Resiliência Operacional

## Introdução

Nesta lição, você aprenderá sobre as **quatro áreas da resiliência operacional**, os fatores contribuintes, os benefícios da resiliência operacional melhorada, as causas e as possíveis consequências do tempo inativo, além de como a AWS reduz as falhas operacionais. Também exploraremos exemplos de clientes que aumentaram sua resiliência operacional utilizando a AWS.

## O Que é Resiliência Operacional?

O terceiro pilar do **Cloud Value Framework** é a **resiliência operacional**, que se refere à melhoria na disponibilidade e na segurança dos sistemas. Isso significa mais **tempo ativo**, menos **tempo de inatividade** e risco reduzido.

### Importância da Resiliência Operacional

A resiliência operacional abrange a manutenção de uma infraestrutura que seja altamente disponível e segura. Isso envolve vários componentes como camada de rede, servidores, armazenamento e banco de dados, garantindo que cada um esteja sempre disponível.

#### Exemplos de Impactos Negativos do Tempo de Inatividade

- **Empresa Aérea**: Uma interrupção no datacenter cancelou 2 mil voos, resultando em um custo de mais de $150 milhões.
- **Banco**: Um ataque DDoS prolongado afetou a confiança dos clientes.
- **Varejista**: Uma violação de dados resultou em perdas de $250 milhões.

Esses exemplos demonstram que a **falta de resiliência operacional** pode ter consequências financeiras e de reputação devastadoras.

## Causas Comuns de Tempo de Inatividade

O tempo de inatividade não é causado apenas por ataques externos; ele pode ocorrer quando a demanda de serviços excede a capacidade da infraestrutura. Isso é comum durante horários de pico, como quando um banco de dados é sobrecarregado com consultas.

### Custos Associados ao Tempo de Inatividade

Os custos de tempo de inatividade incluem:

- Taxas de terceiros
- Substituição de equipamentos
- Custos de recuperação e detecção
- Perda de receita
- Danos à reputação

O custo de **interrupção dos negócios** é geralmente maior que o custo de perda de receita, devido à rotatividade de clientes e perda de oportunidades.

## Áreas da Resiliência Operacional

### Operações

As falhas operacionais podem ser causadas por:

- **Erros humanos**: Falta de procedimentos bem definidos, erros de configuração, acidentes no datacenter.
- **Exemplo**: Um funcionário derruba café no servidor, causando falhas.

**Como a AWS Ajuda**: A AWS se especializa em gerenciar datacenters, com regras rigorosas e redundância que permitem a recuperação rápida sem que os clientes percebam.

### Segurança

As violações de segurança podem ser causadas por:

- **Malware**: Worms e vírus.
- **Problemas de segurança**: Credenciais mal gerenciadas, falta de patches.

**Como a AWS Ajuda**: A AWS utiliza um modelo de segurança compartilhada, com responsabilidade desde o hypervisor até o sistema operacional. Oferece ferramentas como AWS Identity Access Management (IAM) e mais de 30 certificações de conformidade.

### Software

As falhas de software podem ser causadas por:

- **Esgotamento de recursos**: Processos travados, vazamentos de memória.
- **Erros de lógica**: Referências incorretas, erros de sincronização.

**Como a AWS Ajuda**: A AWS oferece serviços que permitem escalar recursos automaticamente, implantações blue/green para reversões rápidas, e aplicação automática de patches para manter o software seguro e resiliente.

### Infraestrutura

As falhas de infraestrutura podem ser causadas por:

- **Falha de hardware**: Servidores, armazenamento ou redes.
- **Desastres naturais**: Furacões, inundações.
- **Ataques volumétricos**: DDoS.

**Como a AWS Ajuda**: A AWS expande continuamente sua infraestrutura, oferece alta disponibilidade através de múltiplas zonas de disponibilidade, e cria sistemas duráveis e resilientes para garantir que os aplicativos dos clientes estejam sempre disponíveis.

## Exemplos de Sucesso

### Lingopass

- **Redução de Indisponibilidade**: Reduziu sua indisponibilidade de 2 horas semanais para 2 horas ao ano.

### Itaú Unibanco

- **Alta Disponibilidade**: Alcançou 99,97% de disponibilidade devido aos serviços da AWS.

### Portal de Documentos

- **Ganho Operacional**: Aumentou a disponibilidade de 85% para 94% (98% em dias úteis).

---

Com esses exemplos e informações, você agora tem uma visão clara de como a resiliência operacional pode impactar significativamente o sucesso de uma empresa e como a AWS pode ajudar a mitigar os riscos associados.

---

### Qual opção descreve o foco da resiliência operacional?

- **Disponibilidade e segurança**
- ~~Modelos de preços~~
- ~~Velocidade e valor~~
- ~~Impacto ambiental~~

> **Explicação:**
> A resiliência operacional é o benefício conquistado com a melhoria na disponibilidade e na segurança. Isso representa mais tempo ativo, menos tempo de inatividade e risco reduzido.
