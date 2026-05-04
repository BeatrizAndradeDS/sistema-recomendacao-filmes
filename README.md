# 🎬 Sistema de Recomendação de Filmes

[![Python](https://img.shields.io/badge/Python-3.13-blue.svg)](https://www.python.org/)
[![scikit-learn](https://img.shields.io/badge/scikit--learn-1.7.1-orange.svg)](https://scikit-learn.org/)
[![Pandas](https://img.shields.io/badge/Pandas-2.3.0-green.svg)](https://pandas.pydata.org/)

Esse é um Sistema de recomendação de filmes baseado em filtragem por conteúdo usando Machine Learning. O sistema analisa características de filmes (gênero, elenco, diretor, sinopse) e recomenda títulos similares através de vetorização de texto e cálculo de similaridade de cosseno.

<br/>

---

## Demonstração

![Sistema em Ação](images/demo.gif)

<br/>

---

**Exemplo de recomendação:**
```python
sistema_recomendacao('Avatar')

# Resultado:
# Aliens vs Predator: Requiem
# Aliens
# Falcon Rising
# Independence Day
# Titan A.E.
```

<br/>

<details>
<summary> <b>Ver mais exemplos de recomendações</b></summary>

<br/>
 
| Filme Consultado | Top 5 Recomendações |
|------------------|---------------------|
| **Avengers: Age of Ultron** | Iron Man 3, Iron Man 2, Iron Man, Thor, The Avengers |
| **Jurassic World** | Jurassic Park, The Lost World, Walking With Dinosaurs, Terminator Genisys, Jurassic Park III |

</details>

<br/>


---

## Sobre o Projeto

### **Objetivo**
Construir um sistema inteligente que recomende 5 filmes similares ao que o usuário assistiu, mantendo-o engajado na plataforma.

### **Metodologia**
1. **Preparação de Dados:** Merge de datasets, extração de features (gênero, elenco, diretor, sinopse)
2. **NLP:** Stemming, normalização e remoção de stop words
3. **Vetorização:** CountVectorizer com 5.000 features, transformação de texto em matriz numérica esparsa
4. **Similaridade:** Cosine similarity para medir distância entre filmes

### **Dataset**
- **Fonte:** [The Movie Database (TMDb)](https://developer.themoviedb.org/docs)
- **Total:** 4.806 filmes processados

<br/>

---

## Outras Aplicações

Esta mesma arquitetura de **filtragem baseada em conteúdo** pode ser aplicada em diversos contextos:

- **E-commerce:** Recomendar produtos similares com base em descrição, categoria e especificações
- **Notícias:** Sugerir artigos relacionados usando tags, autor e conteúdo
- **Música:** Recomendar músicas por gênero, artista e características do áudio
- **Livros:** Sugerir títulos similares baseado em autor, gênero e sinopse
- **Imóveis:** Recomendar propriedades por localização, características e valor
- **Vagas:** Sugerir oportunidades baseado em skills, área e descrição
- **Games:** Recomendar jogos similares por gênero, desenvolvedora e gameplay

**Conceito-chave:** Qualquer problema onde você precise encontrar itens similares baseado nas suas características é possível usar essa técnica.

<br/>

---

## Tecnologias

```python
Python 3.13
├── pandas 2.3.0          # Manipulação de dados
├── numpy 2.3.1           # Computação numérica
├── scikit-learn 1.7.1    # Machine Learning
│   ├── CountVectorizer   # Vetorização
│   └── cosine_similarity # Distância de cosseno
└── nltk 3.9.1            # NLP e stemming
```

<br/>

---

## Como Executar

<details>
<summary><b> Clique para ver as instruções de instalação</b></summary>

### **Pré-requisitos**
- Python 3.8 ou superior
- pip instalado
- Jupyter Notebook

### **Passo a passo**

```bash
# 1. Clone o repositório
git clone https://github.com/BeatrizAndradeDS/sistema-recomendacao-filmes.git

# 2. Entre na pasta do projeto
cd sistema-recomendacao-filmes

# 3. Instale as dependências
pip install -r requirements.txt

# 4. Obtenha os dados (ver seção abaixo)

# 5. Abra o Jupyter Notebook
jupyter notebook Projeto1_Filme_BeatrizAndrade.ipynb
```

### **Obtendo os Dados**

⚠️ Os arquivos CSV não estão incluídos no repositório devido ao tamanho (>25MB).

**Opção 1:** Baixe da fonte original
- [TMDb API](https://developer.themoviedb.org/docs)

**Opção 2:** Entre em contato
- biasandrade@gmail.com
- [LinkedIn](https://www.linkedin.com/in/andrade-beatriz/)

Coloque os arquivos na pasta `dados/`:
```
dados/
├── dataset_filmes.csv
└── dataset_elenco.csv
```
<br/>

</details>

<br/>

---

## Conceitos Aplicados

<details>
<summary><b>Clique para expandir os conceitos técnicos</b></summary>

<br/>

| Área | Técnicas |
|---|---|
| Matemática & Estatística | Álgebra linear, distância de cosseno, similaridade vetorial |
| Machine Learning | Aprendizado não supervisionado, filtragem por conteúdo, feature engineering |
| NLP | Tokenização, stemming, Bag of Words, Term Frequency |


</details>

<br/>

---

## Melhorias Futuras

- [ ] Implementar TF-IDF para melhor ponderação (frequência e raridade da aparição da palavra)
- [ ] Interface web com Streamlit
- [ ] Incluir avaliações de usuários (ratings)

<br/>

---

## Sobre mim

**Beatriz Andrade**  
18 anos trabalhando com dados e agora também com Machine Learning

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Beatriz%20Andrade-blue?style=flat&logo=linkedin)](https://www.linkedin.com/in/andrade-beatriz/)
[![Email](https://img.shields.io/badge/Email-biasandrade%40gmail.com-red?style=flat&logo=gmail)](mailto:biasandrade@gmail.com)

<br/>

---

## Licença

Este projeto está sob a licença MIT.

<br/>

---

⭐ Se este projeto te ajudou, considere dar uma estrela no repositório!
