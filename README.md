# Santander Dev Week 2023 - Pipeline ETL com Python e IA Generativa

Este repositório contém a implementação de um pipeline **ETL (Extract, Transform, Load)** desenvolvido em Python durante a **Santander Dev Week 2023**. O projeto integra consumo de APIs REST, manipulação de dados com Pandas e personalização de campanhas de marketing utilizando Inteligência Artificial Generativa.

---

## 🎯 Contexto do Projeto

O objetivo principal é atuar como cientista de dados no Santander para engajar os clientes de maneira totalmente personalizada. Utilizando dados de uma base de IDs de usuários, o sistema consome uma API REST para buscar informações bancárias, processa esses dados e atualiza o perfil de cada cliente com mensagens customizadas de marketing focadas em investimentos.

---

## 🔄 Arquitetura do Pipeline ETL

### 1. Extract (Extração)
- Leitura de uma planilha em formato CSV (`SDW2023.csv`) contendo a lista de IDs dos usuários do banco.
- Consulta via requisição HTTP `GET` na API oficial do evento para resgatar os dados cadastrais, contas, cartões e histórico de notícias de cada cliente.

### 2. Transform (Transformação)
- Processamento e estruturação dos dados utilizando bibliotecas Python como `Pandas` e `NumPy`.
- Geração ou integração de mensagens de marketing personalizadas (como frases motivacionais e conteúdos voltados para educação financeira e investimentos) estruturadas para compor o feed de notícias do cliente.

### 3. Load (Carregamento)
- Envio das informações atualizadas de volta para o servidor através de requisições HTTP `PUT`.
- Inserção dinâmica das novas mensagens de marketing diretamente na propriedade `news` do perfil de cada usuário na API.

---

## 🛠️ Tecnologias e Bibliotecas Utilizadas

- **Python 3.x**
- **Pandas** (Manipulação e normalização de dados tabulares)
- **Requests** (Consumo e atualização via API REST)
- **JSON** (Serialização e manipulação de estruturas de dados)
- **Matplotlib** (Visualização auxiliar de dados, quando aplicável)

---

## 🚀 Como Executar o Projeto

1. Clone o repositório para o seu ambiente local:
   ```bash
   git clone [https://github.com/LeonardoCorreia08/seu-repositorio.git](https://github.com/LeonardoCorreia08/seu-repositorio.git)
