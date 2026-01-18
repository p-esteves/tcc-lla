# 🧠 Detecção de Leucemia Linfoblástica Aguda com Redes Neurais Convolucionais

Este repositório contém o código desenvolvido no âmbito do Trabalho de Conclusão de Curso (TCC)
**“Uso de redes neurais convolucionais no diagnóstico de leucemia linfoblástica aguda”**, apresentado ao curso de Bacharelado em Estatística da **Universidade Federal do Ceará (UFC)**.

📄 Monografia disponível em:  
http://repositorio.ufc.br/handle/riufc/83725

O objetivo deste repositório é **tornar público o código utilizado nos experimentos**, documentar as principais decisões técnicas adotadas e **complementar o trabalho acadêmico**, servindo também como **material de portfólio**.

---

## 🎯 Objetivo do Projeto

Investigar a aplicação de **Redes Neurais Convolucionais (CNNs)** na **classificação automática de imagens de esfregaço de sangue periférico**, com foco na detecção de **Leucemia Linfoblástica Aguda (LLA)**.

O projeto avalia se arquiteturas modernas de deep learning conseguem atingir **alto desempenho preditivo** a partir de imagens microscópicas, explorando técnicas de transfer learning e fine-tuning.

---

## 🧬 Contexto

A Leucemia Linfoblástica Aguda é um câncer hematológico agressivo, cujo diagnóstico tradicional envolve métodos invasivos, custosos e nem sempre amplamente disponíveis.

Neste trabalho, é explorada uma abordagem baseada em **visão computacional e aprendizado profundo**, utilizando imagens de células sanguíneas para apoiar a triagem automatizada da doença.

---

## 📊 Conjunto de Dados

Os experimentos utilizam o dataset público disponível no Kaggle:

🔗 https://www.kaggle.com/datasets/mehradaria/leukemia

O conjunto de dados é composto por **imagens de células sanguíneas**, organizadas em classes relacionadas a diferentes estágios da leucemia linfoblástica aguda, sendo amplamente utilizado em estudos acadêmicos sobre diagnóstico assistido por computador.

O uso deste dataset permite **comparabilidade com trabalhos da literatura** e reprodutibilidade dos experimentos.

---

## 🧠 Decisões de Modelagem

Algumas decisões técnicas relevantes adotadas no projeto:

- **Arquitetura EfficientNet-B3**, escolhida pelo bom equilíbrio entre desempenho e custo computacional.
- **Transfer learning**, com pesos pré-treinados ajustados ao domínio das imagens hematológicas.
- Uso do **framework FastAI**, visando acelerar a experimentação e facilitar o fine-tuning.
- Avaliação focada no desempenho global do modelo no conjunto de teste, conforme descrito na monografia.

---

## 🔄 Pipeline do Projeto

O fluxo experimental seguido no notebook pode ser resumido em:

1. Organização e carregamento do dataset de imagens
2. Pré-processamento e normalização
3. Construção do DataLoader
4. Definição da arquitetura e configuração do treinamento
5. Treinamento do modelo com fine-tuning
6. Avaliação no conjunto de teste
7. Análise dos resultados e comparação com abordagem da literatura

---

## 📈 Resultados

O modelo baseado em **EfficientNet-B3** alcançou:

- **98,92 % de acurácia no conjunto de teste**

Os resultados são discutidos em detalhes no TCC, incluindo comparação com uma abordagem de referência baseada em **DenseNet-201 combinada com segmentação de cor HSV**.

---

## 🗂 Estrutura do Repositório

tcc-lla/
- README.md
- tcc.ipynb
- data/ (dados não versionados no repositório)

---

## 🚀 Reprodutibilidade e Execução

Este projeto foi desenvolvido e executado originalmente no **Google Colab**. 
O notebook é autossuficiente, sendo responsável por instalar dependências, baixar o conjunto de dados e organizar os arquivos no ambiente de execução.

O dataset é obtido dinamicamente a partir do Kaggle, utilizando a API oficial do Kaggle, e armazenado temporariamente no ambiente do Colab ou no Google Drive. Por esse motivo, os dados não são versionados neste repositório.

Para reproduzir os experimentos, recomenda-se:

- Abrir o arquivo `tcc.ipynb` no Google Colab
- Executar as células sequencialmente, conforme descrito no notebook

A execução em ambiente local não é o foco deste projeto e pode exigir adaptações no código, especialmente em relação ao gerenciamento de caminhos, dependências e download dos dados.

---

## ⚠️ Escopo e Limitações

- Projeto desenvolvido com **fins acadêmicos e de pesquisa**
- Não substitui diagnóstico clínico profissional
- Resultados dependem do dataset e do protocolo experimental adotado
- O dataset utilizado possui licença própria definida pelos autores no Kaggle

---

## 🎓 Relação com o TCC

A monografia discute os **fundamentos teóricos, revisão de literatura e análise crítica dos resultados**.  
Este repositório concentra-se na **implementação prática do pipeline experimental**, servindo como complemento técnico ao trabalho escrito.

---

## 👤 Autor

**Pietro de Oliveira Esteves**  
Bacharel em Estatística — UFC  
GitHub: https://github.com/p-esteves  
Lattes: http://lattes.cnpq.br/7195442117723445
