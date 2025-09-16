# dio-cloudformation-lab
Desafio DIO - Implementando sua Primeira Stack com AWS CloudFormation

# Desafio DIO - Implementando sua Primeira Stack com AWS CloudFormation

Este repositório contém a prática do laboratório proposto pela DIO, cujo objetivo é criar e gerenciar recursos na AWS por meio do **AWS CloudFormation**.  
A documentação serve como material de apoio para revisão de conceitos e para futuras implementações.

---

## Objetivos de Aprendizagem

- Aplicar os conceitos aprendidos em um ambiente prático.  
- Documentar processos técnicos de forma clara e estruturada.  
- Utilizar o GitHub como ferramenta para compartilhamento de documentação técnica.  

---

## Etapas do Desafio

### 1️. Configuração do Ambiente
Antes de iniciar, é necessário garantir:
- Conta ativa na **AWS**.  
- Usuário com permissões para usar o **CloudFormation**.  
- Acesso ao console ou AWS CLI configurada localmente.  

---

### 2️. Entendendo o CloudFormation
O **AWS CloudFormation** permite criar recursos de infraestrutura como código (IaC).  
Em vez de configurar manualmente cada serviço, você descreve a infraestrutura em um **template YAML ou JSON** e o serviço provisiona automaticamente.  

---

### 3. Criando o Template
Aqui criamos um arquivo `template.yaml` descrevendo os recursos.  
Exemplo de um bucket S3 simples:

```yaml
AWSTemplateFormatVersion: "2010-09-09"
Description: "Exemplo de Stack simples com S3"

Resources:
  MyBucket:
    Type: AWS::S3::Bucket
    Properties:
      BucketName: meu-primeiro-bucket-cloudformation

