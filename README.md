# Relat-rio-de-implementa-o-da-Farm-cia
Relatório de implemantação

# RELATÓRIO DE IMPLEMENTAÇÃO DE SERVIÇOS AWS

**Data:** 30 de maio de 2026  
**Empresa:** Abstergo Industries  
**Responsável:** Jorge Luís da Silva Inácio.  

## Introdução
Este relatório apresenta o processo de implementação de ferramentas na empresa Abstergo Industries, realizado por [Seu Nome Completo]. O objetivo do projeto foi elencar 3 serviços AWS, com a finalidade de realizar a diminuição de custos operacionais e de infraestrutura imediatos.

## Descrição do Projeto
O projeto de implementação de ferramentas foi dividido em 3 etapas estratégicas de otimização financeira. A seguir, são descritas as etapas do projeto:

### Etapa 1: Otimização de Armazenamento Dinâmico
* **Nome da ferramenta:** Amazon S3 Intelligent-Tiering
* **Foco da ferramenta:** Armazenamento de objetos com gerenciamento automático de custos.
* **Descrição de caso de uso:** A Abstergo Industries possui um volume massivo de arquivos de mídia e logs com padrões de acesso desconhecidos ou imprevisíveis. Ao migrar esses dados para a classe *Intelligent-Tiering*, o monitoramento automatizado moverá os objetos não acessados por mais de 30 dias para camadas de acesso infrequente. Isso gera uma economia imediata no custo por gigabyte sem comprometer a performance ou exigir intervenção manual da equipe de engenharia.

### Etapa 2: Migração e Consolidação de Banco de Dados
* **Nome da ferramenta:** Amazon Aurora (compatível com PostgreSQL/MySQL)
* **Foco da ferramenta:** Banco de dados relacional totalmente gerenciado de alto desempenho.
* **Descrição de caso de uso:** Substituição de instâncias de bancos de dados tradicionais on-premises ou em instâncias EC2 superdimensionadas. O Amazon Aurora escala o armazenamento de forma automática e sob demanda (sem desperdício de provisionamento) e oferece até 5x mais desempenho que o MySQL padrão. Isso permite consolidar múltiplos servidores antigos em menos recursos de nuvem, reduzindo gastos com licenciamento e infraestrutura.

### Etapa 3: Arquitetura de Cache de Alta Performance
* **Nome da ferramenta:** Amazon DynamoDB Accelerator (DAX)
* **Foco da ferramenta:** Cache em memória integrado para tabelas NoSQL.
* **Descrição de caso de uso:** Para evitar o custo elevado de escalabilidade vertical de tabelas do DynamoDB que sofrem com picos de leitura repetitivos, foi implementada a camada de cache do DAX. Ele reduz o tempo de resposta de milissegundos para microssegundos. Com isso, a empresa consegue diminuir drasticamente as unidades de capacidade de leitura (RCUs) provisionadas na tabela principal, gerando uma redução de custos direta na fatura mensal do DynamoDB.

## Conclusão
A implementação das ferramentas na empresa Abstergo Industries tem como esperado uma redução de custos imediata em armazenamento, banco de dados e processamento de consultas, além de aumentar a eficiência e a alta disponibilidade da infraestrutura. Recomenda-se a continuidade da utilização das ferramentas implementadas e o monitoramento contínuo através do AWS Cost Explorer para identificar novas oportunidades de otimização de gastos.

## Anexos
* [Diagrama de Arquitetura de Rede da VPC no Figma](https://figma.com.
* [Repositório do Projeto Prático no GitHub]https://github.com/JORGETURBO/Relat-rio-de-implementa-o-da-Farm-cia/edit/main/README.md. 
* Guia de Boas Práticas AWS Well-Architected - Pilar de Otimização de Custos.

**Assinatura do Responsável pelo Projeto:**  
Jorge Luís da Silva Inácio.
