# AWS Well-Architected Framework

O **AWS Well-Architected Framework** ajuda você a entender como projetar e operar sistemas confiáveis, seguros, eficientes e econômicos na AWS Cloud. Ele fornece uma maneira de medir consistentemente sua arquitetura em relação às melhores práticas e princípios de design e identificar áreas para melhoria.

O **Well-Architected Framework** é baseado em seis pilares:

- **Excelência Operacional**
- **Segurança**
- **Confiabilidade**
- **Eficiência de Desempenho**
- **Otimização de Custos**
- **Sustentabilidade**

Para saber mais, veja os detalhes de cada um dos seis pilares abaixo.

## 1. Excelência Operacional

**Excelência operacional** é a capacidade de operar e monitorar sistemas para entregar valor de negócios e melhorar continuamente processos e procedimentos de suporte.

- **Princípios de design para excelência operacional na nuvem incluem:**
  - Realizar operações como código.
  - Anotar a documentação.
  - Antecipar falhas.
  - Fazer mudanças pequenas e reversíveis com frequência.

## 2. Segurança

O pilar de **Segurança** é a capacidade de proteger informações, sistemas e ativos enquanto entrega valor de negócios por meio de avaliações de risco e estratégias de mitigação.

- **Ao considerar a segurança da sua arquitetura, aplique estas melhores práticas:**
  - Automatize as melhores práticas de segurança sempre que possível.
  - Aplique segurança em todas as camadas.
  - Proteja os dados em trânsito e em repouso.

## 3. Confiabilidade

**Confiabilidade** é a capacidade de um sistema de:

- Recuperar-se de interrupções de infraestrutura ou serviços.
- Adquirir dinamicamente recursos computacionais para atender à demanda.
- Mitigar interrupções como erros de configuração ou problemas transitórios de rede.

- **A confiabilidade inclui:**
  - Testar procedimentos de recuperação.
  - Escalar horizontalmente para aumentar a disponibilidade agregada do sistema.
  - Recuperar-se automaticamente de falhas.

## 4. Eficiência de Desempenho

**Eficiência de desempenho** é a capacidade de usar recursos computacionais de maneira eficiente para atender aos requisitos do sistema e manter essa eficiência à medida que a demanda muda e as tecnologias evoluem.

- **Avaliar a eficiência de desempenho da sua arquitetura inclui:**
  - Experimentar com mais frequência.
  - Usar arquiteturas serverless.
  - Projetar sistemas para se tornarem globais em minutos.

## 5. Otimização de Custos

**Otimização de custos** é a capacidade de operar sistemas para entregar valor de negócios ao menor custo possível.

- **A otimização de custos inclui:**
  - Adotar um modelo de consumo.
  - Analisar e atribuir despesas.
  - Usar serviços gerenciados para reduzir o custo total de propriedade.

## 6. Sustentabilidade

Em dezembro de 2021, a AWS introduziu um pilar de **sustentabilidade** como parte do AWS Well-Architected Framework.

- **Sustentabilidade** é a capacidade de melhorar continuamente os impactos de sustentabilidade, reduzindo o consumo de energia e aumentando a eficiência em todos os componentes de uma carga de trabalho, maximizando os benefícios dos recursos provisionados e minimizando o total de recursos necessários.

- **Para facilitar o bom design para a sustentabilidade:**
  - Entenda seu impacto.
  - Estabeleça metas de sustentabilidade.
  - Maximize a utilização.
  - Antecipe e adote novas ofertas de hardware e software mais eficientes.
  - Use serviços gerenciados.
  - Reduza o impacto a jusante das suas cargas de trabalho na nuvem.

---

### Which pillar of the AWS Well-Architected Framework focuses on the ability of a workload to consistently and correctly perform its intended functions?

- ~~Operational Excellence~~
- ~~Performance Efficiency~~
- ~~Security~~
- **Reliability**

> **Explanation:**
> The correct response option is **Reliability**.
>
> The other response options are incorrect because:
>
> - The Operational Excellence pillar includes the ability to run workloads effectively, gain insights into their operations, and continuously improve supporting processes to deliver business value.
> - The Performance Efficiency pillar focuses on using computing resources efficiently to meet system requirements, and to maintain that efficiency as demand changes and technologies evolve.
> - The Security pillar includes protecting data, systems, and assets, and using cloud technologies to improve the security of your workloads.

---

### Which pillar of the AWS Well-Architected Framework includes the ability to run workloads effectively and gain insights into their operations?

- ~~Cost Optimization~~
- **Operational Excellence**
- ~~Performance Efficiency~~
- ~~Reliability~~

> **Explanation:**
> The correct response option is **Operational Excellence**.
>
> The other response options are incorrect because:
>
> - The Cost Optimization pillar focuses on the ability to run systems to deliver business value at the lowest price point.
> - The Performance Efficiency pillar focuses on using computing resources efficiently to meet system requirements and to maintain that efficiency as demand changes and technologies evolve.
> - The Reliability pillar focuses on the ability of a workload to consistently and correctly perform its intended functions.
