# 📍 Buscador de CEP em Java

Este projeto é um **buscador de CEP** que consulta informações de endereço a partir de um **CEP informado pelo usuário**, utilizando uma **API externa**, exibindo os dados no terminal e salvando o resultado em um **arquivo JSON**.

Projeto focado na prática de **consumo de APIs**, **tratamento de exceções** e **manipulação de arquivos** em Java.

---

## 📌 Funcionalidades

- 🔎 Buscar endereço a partir do CEP
- 🌐 Consumir API de consulta de CEP
- 📄 Exibir endereço no terminal
- 💾 Salvar endereço em arquivo `.json`
- ⚠️ Tratar erros de requisição e entrada inválida

---

▶️ Execução do Programa

Ao executar o programa, o usuário informa um CEP válido e o sistema retorna os dados do endereço

```txt
Digite um número de CEP para consulta:

01001000

Endereco:
cep: 01001-000.
logradouro: Praça da Sé.
bairro: Sé.
 cidade: São Paulo.
 uf: SP.

Arquivo gerado com sucesso!
Process finished with exit code 0

```

---

## 🏠 Endereço

A classe Endereco representa os dados retornados pela API:

- 📮 CEP
- 🛣️ Logradouro
- 🏘️ Bairro
- 🌆 Cidade
- 🗺️ UF

Essas informações são exibidas no terminal e utilizadas para gerar o arquivo JSON.

---

## 🌐 Consulta de CEP

- A classe ConsultaCep é responsável por:
- Realizar a requisição HTTP para a API de CEP
- Converter a resposta JSON em um objeto Endereco
- Tratar erros de CEP inválido ou inexistente

---

## ⚠️ Tratamento de Erros

- O sistema trata:
- CEP inválido
- Erros de conexão

Problemas de leitura/gravação de arquivos

```txt

CEP inválido ou não encontrado
Finalizando a aplicação

```
---

## 🧱 Estrutura do Projeto

```txt
src
├── Principal.java
├── ConsultaCep.java
├── Endereco.java
└── GeradorDeArquivo.java


```txt
```

