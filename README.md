# Classificação de Fake News com WELFake

Este projeto visa a detecção de notícias falsas utilizando o dataset WELFake e técnicas de processamento de linguagem natural (NLP). O modelo utiliza TF-IDF para vetorização de texto e SVM (Máquinas de Vetores de Suporte) para classificação. Além disso, o projeto explora análise de tópicos com LDA (Latent Dirichlet Allocation).

## Pontos Abordados
- Carregamento e processamento inicial dos dados do WELFake
- Análise exploratória detalhada dos dados
- Criação de um pipeline de classificação utilizando TF-IDF e SVM
- Avaliação da influência do tamanho do dataset na performance do modelo
- Análise de tópicos utilizando LDA (Latent Dirichlet Allocation)

## Requisitos
- Python 3.7 ou superior
- Jupyter Notebook
- Bibliotecas mencionadas em requirements.txt

## Estrutura do Projeto

- `data/`: Diretório contendo o dataset WELFake.
- `notebooks/projeto.ipynb`: Notebook Jupyter para execução do projeto.
- `requirements.txt`: Lista de dependências necessárias para o projeto.
- `IEE_artigo.pdf`: Artigo no modelo IEEE do projeto.

## Instalação do projeto

Clone o repositório:
```bash
git clone https://github.com/marlonsp/Fake-News-Classification
cd Fake-News-Classification
```
Crie um ambiente virtual para isolar as dependências:
```bash
python -m venv env
env\Scripts\activate
```
Instale as dependências:
```bash
pip install -r requirements.txt
```
Certifique-se de ter as seguintes bibliotecas instaladas:

- pandas
- numpy
- matplotlib
- nltk
- scikit-learn

## Utilização

Para executar o projeto, primeiro realize o download dos [dados](https://www.kaggle.com/datasets/saurabhshahane/fake-news-classification/data), salve o arquivo "WELFake_Dataset.csv" no diretório "/data".
Depois, acesse o jupyter notebook "projeto.ipynb" e execute cada uma das células sequencialmente.

## Preparação dos Dados
Os dados são carregados a partir de um arquivo CSV, onde as colunas principais incluem:

title: Título da notícia.
text: Corpo da notícia.
label: Rótulo indicando se a notícia é verdadeira ou falsa.
Os dados são preprocessados para remover stopwords e aplicar lematização.

## Modelagem
O modelo utiliza TF-IDF para vetorização e SVM para classificação. A performance é avaliada utilizando a métrica de acurácia balanceada.

## Análise de Tópicos
O projeto também realiza uma análise de tópicos utilizando LDA, permitindo a interpretação das principais características associadas a diferentes tópicos de notícias.

## Conclusão
Este projeto explora a detecção de fake news utilizando técnicas avançadas de processamento de linguagem natural. Os resultados mostram a eficácia do modelo SVM combinado com vetorização TF-IDF.

## Referência
Verma, P. K., Agrawal, P., Amorim, I., & Prodan, R. (2021). WELFake: Word Embedding Over Linguistic Features for Fake News Detection. IEEE Transactions on Computational Social Systems, 8(4), 881–893. doi:10.1109/TCSS.2021.3068519.

https://www.kaggle.com/datasets/saurabhshahane/fake-news-classification/data
