# Aplicação de Previsão de Agrupamentos para Análise de Marketing

## Visão Geral
Este projeto é uma aplicação web interativa desenvolvida com Streamlit para auxiliar na análise de marketing. O objetivo principal é segmentar futuros clientes em três grupos distintos, utilizando técnicas de aprendizado de máquina. A aplicação utiliza modelos pré-treinados (como KMeans, encoder e scaler) para classificar os clientes com base em seus dados e interesses.

## Grupos de Clientes
- Grupo 0:
  Focado em um público jovem, com forte interesse em moda, música e aparência.
- Grupo 1:
  Associado a esportes, especialmente futebol americano, basquete, além de atividades culturais como banda e rock.
- Grupo 2:
  Segmento mais equilibrado, com interesses variados em música, dança e moda.

## Funcionalidades
- Entrada de Dados:
  A aplicação aceita arquivos no formato `.csv` que devem seguir o padrão presente no arquivo de exemplo `novas_entradas.csv`.
- Processamento e Agrupamento:
  Utiliza modelos de aprendizado de máquina para distribuir os dados dos clientes nos três grupos definidos.
- Visualização:
  Os resultados da segmentação podem ser visualizados em uma tabela interativa diretamente no app.
- Exportação dos Resultados:
  A tabela gerada pode ser baixada como um arquivo `Grupos_interesse.csv` para posterior análise ou uso em outras ferramentas.

## Requisitos
- Python: Versão 3.7 ou superior.
- Bibliotecas:
  As dependências necessárias estão listadas no arquivo requirements.txt e incluem, por exemplo:
  - Streamlit
  - scikit-learn
  - pandas
  - Outras dependências necessárias para o funcionamento da aplicação.

## Instalação e Execução
Siga os passos abaixo para executar a aplicação localmente:

1. Clone este repositório e até o diretório do projeto:
   ```bash
   git clone https://github.com/VitorOnofreRamos/Aplicacao-previsao-de-agrupamentos.git
   cd Aplicacao-previsao-de-agrupamentos
   ```

2. Instale as dependências:
   ```bash
   pip install -r requirements.txt
   ```

3. Execute a aplicação:
   ```bash
   streamlit run App.py
   ```

4. Acesse a aplicação:
  Você poderá acessar a aplicação localmente conforme o endereço exibido no terminal ou utilizar a versão online disponível em:
  [aplicacao-previsao-de-agrupamentos-fipr3haapaxz3bar3qu8b7.streamlit.app](aplicacao-previsao-de-agrupamentos-fipr3haapaxz3bar3qu8b7.streamlit.app)

## Formato de Entrada de Dados:
A aplicação foi desenvolvida para aceitar arquivos `.csv` que sigam o padrão do anexo `novas_entradas.csv` presente nesse repositório.
*Atenção: Certifique-se de que os dados estejam corretamente formatados conforme o exemplo para evitar erros durante o processamento.*

## Modelos Utilizados
- **KMeans**: Utilizado para a previsão de agrupamentos.
- **Scaler**: Para normalização dos dados antes da previsão.
- **Encoder**: Codificação de dados categóricos.

## Estrutura do Repositório
```
.
├── App.py               # Script principal da aplicação
├── encoder.pkl           # Arquivo pickle do encoder
├── kmeans.pkl            # Arquivo pickle do modelo KMeans
├── scaler.pkl            # Arquivo pickle do scaler
├── requirements.txt      # Lista de dependências
├── novas_entradas.csv    # Arquivo de exemplo de entrada de dados
└── README.md             # Documentação do projeto
```

## Base do Projeto
Este projeto foi desenvolvido seguindo as instruções da formação da **Alura**, aplicando conceitos de aprendizado de máquina e análise de dados para fornecer insights úteis para estratégias de marketing.

## Licença
Este projeto está licenciado sob a [MIT License](LICENSE).

