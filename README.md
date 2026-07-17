# Projeto de Análise e Previsão de Preços de Carros Usados

Este projeto tem como objetivo criar uma API para prever o preço de carros usados com base em características como ano, quilometragem, motor e número de revisões. A aplicação utiliza Machine Learning para aprender padrões a partir de um dataset e fornecer uma estimativa de valor de forma rápida e automatizada.

## 📌 O que este projeto faz?

O sistema recebe informações de um carro e retorna uma previsão de preço. Isso pode ser útil para:

- estimar o valor de um veículo antes de vender;
- auxiliar compradores e vendedores em negociações;
- servir como base para sistemas de avaliação automática.

---

## 🧠 Como o projeto funciona

O fluxo do projeto é simples:

1. O arquivo de dados com informações de carros usados é carregado.
2. As variáveis importantes são selecionadas para treinar o modelo.
3. Um algoritmo de regressão linear é treinado para aprender a relação entre as características do carro e o preço.
4. A API recebe uma solicitação com os dados do veículo e retorna uma previsão.

### Conceitos usados de forma breve

- Dataset: é o conjunto de dados usado para ensinar o modelo. Neste caso, ele contém informações históricas sobre carros usados.
- Regressão linear: é uma técnica de Machine Learning que tenta encontrar uma relação entre entradas e um valor contínuo, como o preço.
- API: é uma interface que permite que outros sistemas enviem dados para o modelo e recebam a resposta em formato estruturado.

---

## 🛠️ Tecnologias e bibliotecas utilizadas

O projeto foi construído com:

- Python
- Lovable
- -Render
- Postman
- Flask: para criar a API web
- Flask-CORS: para permitir comunicação entre diferentes origens
- Pandas: para manipular e processar os dados
- Scikit-learn: para treinar o modelo de Machine Learning

---

## 📁 Estrutura do projeto

O projeto contém os seguintes arquivos principais:

- app.py: código principal da API e treinamento do modelo
- dataset_carros_usados.csv: arquivo com os dados utilizados para treinar o modelo
- requirements.txt: dependências necessárias para rodar o projeto
- README.md: documentação do projeto

---

## 🚀 Como usar o projeto

### 1. Instalar as dependências

No terminal, dentro da pasta do projeto, execute:

```bash
pip install -r requirements.txt
```

### 2. Rodar a API localmente

```bash
python app.py
```

A API ficará disponível em:

```text
http://127.0.0.1:8000
```

---

## 🌐 Endpoints da API

### GET /

Retorna uma mensagem simples confirmando que a API está online.

Link da API (método GET):

https://projeto-final-analise-dados.onrender.com

### POST /prever

Recebe um JSON com os dados do carro e retorna o preço previsto.

Link da API (método POST):

https://projeto-final-analise-dados.onrender.com/prever

### Exemplo de requisição

```json
{
  "ano": 2018,
  "quilometragem": 65000,
  "motor": 1.6,
  "num_revisoes": 3
}
```

### Exemplo de resposta

```json
{
  "preco": 65000.0
}
```
---

## 🌍 Site do projeto

O projeto também possui uma interface web disponível em:

https://road-worth-tool.lovable.app/

---

## 🎯 Para que este projeto pode ser usado?

Este projeto pode ser utilizado para:

- prever o valor de carros usados;
- apoiar decisões de compra e venda;
- servir como base para sistemas de avaliação automática;
- demonstrar na prática o uso de Machine Learning em problemas reais.

---

## 🧩 Resumo do desenvolvimento

O projeto foi desenvolvido em etapas simples:

1. coleta e organização dos dados;
2. escolha das variáveis mais relevantes;
3. treinamento de um modelo preditivo;
4. criação de uma API para disponibilizar a previsão;
5. implantação para acesso pela internet.

Esse tipo de solução combina análise de dados, aprendizado de máquina e desenvolvimento web, sendo uma excelente forma de transformar dados em uma aplicação prática e útil.

---

## ✅ Observação final

Este projeto mostra como é possível transformar um conjunto de dados em uma ferramenta funcional, capaz de gerar previsões de forma automática e acessível por meio de uma API.
