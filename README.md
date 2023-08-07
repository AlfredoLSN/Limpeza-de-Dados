[![NPM](https://img.shields.io/npm/l/react)](https://github.com/AlfredoLSN/Limpeza-de-Dados/blob/main/LICENSE) 
# Exploração e Limpeza de Dados

Análise e Limpeza de Dados com Pandas e Plotly

## Descrição

Este projeto tem como objetivo realizar uma análise exploratória e limpeza de dados utilizando a biblioteca Pandas para manipulação dos dados e a biblioteca Plotly Express para visualização dos resultados. A base de dados utilizada contém informações sobre clientes, incluindo características como idade, gênero, estado civil, classificação de risco, categoria do cartão e categoria VIP.

## Instruções de Uso

1. **Instalação das Bibliotecas:**
   Certifique-se de ter o Python instalado em seu ambiente. Em seguida, instale as bibliotecas necessárias com os seguintes comandos:
```bash
pip install pandas
pip install plotly
```


3. **Execução do Código:**
- Faça o download do arquivo "ChavesClientes.xlsx" contendo a base de dados.
- Abra o código em um ambiente Python compatível (Jupyter Notebook, por exemplo).
- Execute as células do código em ordem para carregar, limpar e visualizar os dados.

3. **Visualização dos Gráficos:**
- Os gráficos gerados exibem as associações entre colunas da base de dados, como pagamento em relação à chave de situação, classificação de risco, categoria do cliente e categoria VIP.

## Informações da Base de Dados

- **Características dos Dados:**
- **ChaveSituacao:** formado por:
 - Idade do cliente (a idade mínima para ser cliente é 18 anos)
 - Gênero do cliente:
   - M: Masculino
   - F: Feminino
 - Estado civil do cliente:
   - S: solteiro
   - C: casado
   - D: divorciado
   - V: viúvo
- **ClassRisco:** formado por:
 - Classificação do cliente como (A, B, C) e indicador (+, - ou vazio)
 - Cor do cliente de acordo com um modelo de churn interno da empresa
- **CatCliente:** formado por:
 - Categoria do cartão: qual o tipo de cartão do cliente:
   - Basic
   - Black
   - Platinum
 - Categoria VIP: categoria do cliente VIP (caso exista):
   - Alpha
   - Beta

## Limpeza dos Dados

- **Coluna ChaveSituação:**
- Criou-se três novas colunas: Idade, Gênero e EstadoCivil, a partir da coluna original.
- Convertido o campo Idade para numérico.
- Removida a coluna ChaveSituação.

- **Coluna CatCliente:**
- Criaram-se as colunas CategoriaCartao e CategoriaVip a partir da coluna original.
- Substituídos os valores NaN (não informados) na coluna CategoriaVip por "Comum".

- **Coluna ClassRisco:**
- Criadas as colunas Classificação e Cor a partir da coluna original, utilizando expressões regulares.

## Visualização de Correlações

- Foram gerados gráficos treemap para visualizar as associações entre algumas colunas da base de dados, tais como:
- Gênero e Pagamento
- Categoria do Cartão e Pagamento
- Categoria VIP e Pagamento

## Informações Adicionais

Para mais informações sobre o projeto, acesse o código completo no arquivo "DataCleaning.ipynb". Caso queira contribuir, fique à vontade para enviar pull requests.

## Licença

Este projeto é disponibilizado sob a Licença MIT. Veja o arquivo "LICENSE" para mais detalhes.

## Contato

Se tiver alguma dúvida ou sugestão, sinta-se à vontade para entrar em contato através do email: alfredolsn@hotmail.com



