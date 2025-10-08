# Tech Challenge – RAG com GPT-3.5-turbo

Este projeto utiliza a abordagem Retrieval-Augmented Generation (RAG) com o modelo GPT-3.5-turbo da OpenAI para responder perguntas sobre produtos da Amazon com base no dataset AmazonTitles-1.3MM.

## Etapas do projeto
- Leitura e preparação do dataset `trn.json`
- Geração de embeddings com `text-embedding-ada-002`
- Indexação com FAISS
- Recuperação de contexto relevante
- Geração de respostas com GPT-3.5-turbo

## Execução
Abra o notebook no Google Colab e siga as instruções passo a passo.

## Requisitos
- Conta na OpenAI com créditos ativos
- Google Drive com o arquivo `trn.json`
