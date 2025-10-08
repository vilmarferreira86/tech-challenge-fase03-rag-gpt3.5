# Tech Challenge – RAG com GPT-3.5-turbo e Fine-Tuning com GPT-2

Este projeto implementa uma solução de **RAG (Retrieval-Augmented Generation)** utilizando o modelo **GPT-3.5-turbo da OpenAI** para responder perguntas sobre produtos da Amazon com base no dataset `AmazonTitles-1.3MM`. Além disso, realizamos um **fine-tuning com o modelo GPT-2** para treinar uma versão personalizada com os mesmos dados.

## 🔍 Abordagens Utilizadas

### 1. RAG com GPT-3.5-turbo
- Leitura e preparação do dataset `trn.json`
- Geração de embeddings com `text-embedding-ada-002`
- Indexação dos vetores com FAISS
- Recuperação de contexto relevante via busca semântica
- Geração de respostas com o modelo `GPT-3.5-turbo` da OpenAI

### 2. Fine-Tuning com GPT-2
- Criação de pares pergunta-resposta com base nos dados do produto
- Tokenização com `GPT2Tokenizer`
- Treinamento do modelo `GPT-2` com `Trainer` da Hugging Face
- Teste do modelo fine-tuned com novas perguntas

## 🚀 Execução

Abra o notebook no Google Colab e siga as instruções passo a passo para executar as duas abordagens:
- RAG com GPT-3.5-turbo
- Fine-tuning com GPT-2

## 📦 Requisitos

- Conta na OpenAI com créditos ativos
- Google Drive com o arquivo `trn.json`
- Ambiente com suporte a GPU (opcional para acelerar o fine-tuning)
- Bibliotecas:
  - `openai`
  - `faiss-cpu`
  - `transformers`
  - `datasets`
  - `accelerate`
  - `tqdm`
  - `numpy`
  - `re`

## 📁 Estrutura do Projeto

O projeto está dividido em seções no notebook:
- Instalação de bibliotecas
- Leitura e pré-processamento dos dados
- Geração de embeddings
- Indexação com FAISS
- Geração de respostas com GPT-3.5-turbo
- Preparação e treinamento com GPT-2
- Testes dos modelos

## ✅ Conclusão

Este projeto demonstra como combinar busca semântica com geração de texto utilizando RAG e como realizar fine-tuning com modelos da Hugging Face para personalização. A arquitetura pode ser aplicada em diversos domínios como e-commerce, jurídico, saúde e atendimento ao cliente.
