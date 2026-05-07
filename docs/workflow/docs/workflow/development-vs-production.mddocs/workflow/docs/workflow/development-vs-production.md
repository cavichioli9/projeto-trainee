# Desenvolvimento vs Produção

## Objetivo

Este documento descreve como a equipe realizará a separação entre o ambiente de desenvolvimento e o ambiente de produção do Sistema de Ordem de Serviço, garantindo organização, segurança e melhor controle das versões do projeto.

---

# Ambiente de Desenvolvimento

O ambiente de desenvolvimento será utilizado para:

* criação de funcionalidades;
* testes do sistema;
* correção de erros;
* desenvolvimento de telas;
* documentação do projeto;
* experimentação de melhorias.

Nesse ambiente poderão existir arquivos temporários, documentos internos e conteúdos que não devem ser disponibilizados aos usuários finais.

Arquivos utilizados apenas durante o desenvolvimento:

* documentos da equipe;
* protótipos;
* anotações;
* arquivos de teste;
* imagens de planejamento;
* backlog;
* roadmap;
* evidências da atividade acadêmica.

Esses arquivos estarão organizados principalmente nas pastas:

```bash id="d8t5r2"
docs/
tests/
```

---

# Ambiente de Produção

O ambiente de produção conterá apenas os arquivos necessários para o funcionamento final do Sistema de Ordem de Serviço.

Arquivos destinados à produção:

* frontend do sistema;
* backend;
* banco de dados;
* APIs;
* arquivos de configuração necessários para execução do sistema.

Esses arquivos ficarão organizados principalmente na pasta:

```bash id="m7k9qp"
src/
```

---

# Organização do Fluxo de Trabalho

A equipe utilizará o GitHub como plataforma principal de versionamento e colaboração.

O fluxo adotado será inspirado no GitHub Flow, utilizando branches separadas para organização do desenvolvimento.

## Branch main

Contém as versões mais estáveis do sistema.

## Branch develop

Utilizada para desenvolvimento e testes das funcionalidades.

## Branches de funcionalidades

Cada funcionalidade poderá ser desenvolvida em uma branch específica, como:

```bash id="q1w8fz"
feature/login
feature/cadastro-cliente
feature/ordem-servico
feature/relatorios
```

Após os testes e validações, as alterações serão integradas à branch principal.

---

# Controle de Arquivos Sensíveis

A equipe utilizará o arquivo `.gitignore` para impedir o envio de arquivos desnecessários ou sensíveis para o repositório.

Exemplos:

* arquivos temporários;
* cache;
* configurações locais;
* arquivos de teste.

---

# Ambientes Utilizados

## Ambiente Local

Utilizado pelos integrantes da equipe para programação e testes.

## Ambiente de Homologação

Utilizado para validar funcionalidades antes da publicação final.

## Ambiente de Produção

Versão estável do sistema disponibilizada ao usuário final.

---

# Controle de Versionamento

Os commits serão realizados com mensagens descritivas para facilitar o acompanhamento da evolução do projeto.

Exemplos:

```bash id="gq2nxt"
Cria tela de login
Adiciona cadastro de clientes
Implementa sistema de ordem de serviço
Atualiza backlog do projeto
```

---

# Justificativa da Abordagem

A separação entre desenvolvimento e produção foi escolhida para:

* melhorar a organização do projeto;
* facilitar o trabalho em equipe;
* evitar conflitos de alterações;
* impedir a publicação de arquivos internos;
* garantir maior controle sobre as versões do sistema.

Essa abordagem utiliza conceitos estudados em sala relacionados a:

* GitHub Flow;
* versionamento de software;
* branches de desenvolvimento;
* organização de ambientes;
* colaboração em equipe.
