# AWS Snow Family

A **AWS Snow Family** é uma coleção de dispositivos físicos projetados para ajudar a transferir grandes quantidades de dados para dentro e fora da AWS de forma segura e eficiente. Esses dispositivos são ideais para cenários em que a transferência de dados pela internet seria muito lenta ou impraticável devido ao volume de dados. A Snow Family também é usada em ambientes com conectividade limitada ou em situações onde a segurança dos dados durante o transporte é uma preocupação.

A **AWS Snow Family** é composta por três dispositivos principais: **AWS Snowcone**, **AWS Snowball** e **AWS Snowmobile**. Cada um desses dispositivos atende a diferentes necessidades de capacidade e computação.

## 1. AWS Snowcone

O **AWS Snowcone** é o menor e mais leve dispositivo da família Snow. Ele é projetado para cenários de computação de borda (edge computing) e transferência de dados em pequenas quantidades.

- **Uso Principal:** Transferência segura de dados em locais remotos ou com baixa conectividade, além de executar computação de borda para processar dados localmente antes de enviá-los para a AWS.
- **Especificações:**
  - 2 CPUs
  - 4 GB de memória
  - Até 14 TB de armazenamento utilizável

## 2. AWS Snowball

O **AWS Snowball** é um dispositivo robusto e seguro, projetado para transferir grandes quantidades de dados para a AWS, bem como para realizar computação local durante o processo de transferência.

### Tipos de Dispositivos Snowball:

- **Snowball Edge Storage Optimized:**

  - **Uso Principal:** Ideal para migrações de dados em larga escala e fluxos de trabalho de transferência recorrentes que também exigem computação local.
  - **Armazenamento:**
    - 80 TB de capacidade de HDD para volumes de blocos e armazenamento de objetos compatível com Amazon S3.
    - 1 TB de SSD SATA para volumes de blocos.
  - **Computação:**
    - 40 vCPUs
    - 80 GiB de memória (suporta instâncias Amazon EC2 sbe1, equivalente a C5).

- **Snowball Edge Compute Optimized:**
  - **Uso Principal:** Projetado para casos de uso intensivos em computação, como aprendizado de máquina, análise de vídeo, e outras tarefas que exigem alto poder de processamento.
  - **Armazenamento:**
    - 80 TB de HDD para armazenamento de objetos compatível com Amazon S3 ou volumes de blocos compatíveis com Amazon EBS.
    - 28 TB de NVMe SSD para volumes de blocos compatíveis com Amazon EBS.
  - **Computação:**
    - 104 vCPUs
    - 416 GiB de memória
    - GPU opcional NVIDIA Tesla V100 (para tarefas de processamento gráfico ou aprendizado de máquina).
    - Suporta instâncias Amazon EC2 sbe-c e sbe-g, equivalentes às instâncias C5, M5a, G3 e P3.

## 3. AWS Snowmobile

O **AWS Snowmobile** é o maior dispositivo da Snow Family, projetado para transferir quantidades extremamente grandes de dados, em escala de exabytes, para a AWS.

- **Uso Principal:** Movimentar até 100 petabytes de dados por dispositivo, ideal para grandes organizações que precisam transferir imensos volumes de dados para a AWS em um curto espaço de tempo.
- **Descrição:** Um contêiner reforçado de 45 pés de comprimento, transportado por um caminhão semi-reboque, que oferece segurança física robusta e proteção contra condições adversas durante o transporte de dados.

## Resumo do AWS Snow Family:

Esses dispositivos são utilizados principalmente em cenários onde:

- A transferência de dados pela internet seria muito lenta ou impraticável.
- A segurança física dos dados durante o transporte é uma preocupação.
- Há necessidade de realizar processamento local de dados antes de transferi-los para a nuvem.

A AWS gerencia e integra esses dispositivos com seus serviços de segurança, monitoramento, gerenciamento de armazenamento e capacidades de computação, facilitando a movimentação segura e eficiente de grandes volumes de dados para a nuvem.

---

### What is the storage capacity of Snowball Edge Storage Optimized?

- ~~40 TB~~
- ~~60 TB~~
- **80 TB**
- ~~100 TB~~

> **Explanation:**
> The correct response option is **80 TB**.
>
> Snowball Edge Storage Optimized is a device that enables you to transfer large amounts of data into and out of AWS. It provides 80 TB of usable HDD storage.

---

### What is the storage capacity of AWS Snowmobile?

- ~~40 PB~~
- ~~60 PB~~
- ~~80 PB~~
- **100 PB**

> **Explanation:**
> The correct response option is **100 PB**.
>
> AWS Snowmobile is a service that is used for transferring up to 100 PB of data to AWS. Each Snowmobile is a 45-foot long shipping container that is pulled by a semi trailer truck.
