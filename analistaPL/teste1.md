# Teste Estabilis: Analista de Infraestrutura Pleno

* _Criar uma infraestrutura como código (IaC) e em seguida orquestrar um ambiente com [Docker Swarm](https://docs.docker.com/engine/swarm/)._

## Informações:

* Você receberá no seu e-mail o Access Key/Secret Key para poder acessar/criar sua infraestrutura na [Amazon AWS](https://aws.amazon.com/pt/).
* Você deverá publicar o seu projeto no GitHub e informar por e-mail o link do projeto.

## Instruções:

* **Criar uma infraestrutura na Amazon AWS utilizando o [Terraform](https://www.terraform.io/).**
    
    * Subir a VPC com Nat Gateway
    * Subir 3 instâncias EC2 t2.micro com EBS attached de 20GB na rede pública
    * Subir 3 instâncias EC2 t2.micro com EBS attached de 20GB na rede privada

* **Construção do Cluster Docker Swarm.**

    * Orquestrar o Cluster Docker Swarm utilizando o [Ansible](https://www.ansible.com/).
    * Estrutura do Cluster:
    
        * _3 Manager na rede pública_
        * _3 Worker na rede privada_

* **Criar uma serviço (service) no Cluster de Docker Swarm.**

    * Construir o [Dockerfile](https://docs.docker.com/engine/reference/builder/) do projeto utilizando uma imagem default do [Nginx](https://nginx.org/en/)
    * Gerar uma imagem com o "seu nome" e publicá-la no [Hub Docker](https://hub.docker.com/)
    * Gerar o [Docker Compose](https://docs.docker.com/compose/) da sua aplicação Web "seu nome" expondo a porta 80
    * Subir um serviço (service) "seu nome" no Cluster Docker Swarm

## O que será avaliado?

* Organização do projeto
* Lógica do código
* Uso do Terraform, Ansible, Docker e Git
* Documentação do projeto (README)

## Classificação

* Porcentagem das etapas (25%) Terraform - (25%) Ansible - (25%) Docker
* Projeto entregue no prazo estipulado (25%)

