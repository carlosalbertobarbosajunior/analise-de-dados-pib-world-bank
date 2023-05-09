# graficos-series-temporais-pib-world-bank
## Objetivo:
Funções para exibir gráficos de linha a partir dos dados de PIB disponibilizados no site do banco mundial (https://www.worldbank.org/en/home).

### 1. Importando dados baixados:
Utiliza a biblioteca pandas para ler o arquivo CSV e visualizá-lo.

### 2. Funções:
Um conjunto de quatro funções que tratam os dados do arquivo CSV e exibe as informações de PIB dos países desejados no intervalo de anos definido.

#### read_csv_as_nested_dict(filename, keyfield, separator, quote):
    """
    Inputs:
      filename  - Nome do arquivo CSV
      keyfield  - Coluna a ser usada como chave do dicionário
      separator - Caractere utilizado na separação de informações do arquivo CSV
      quote     - Caractere utilizado em citação no arquivo CSV

    Output:
      Retorna um dicionário de dicionários, onde o dicionário externo
      mapeia a coluna keyfield para a linha correspondente no arquivo
      CSV. Os dicionários internos mapeiam os nomes dos campos para os
      valores da respectiva linha.
    """
    

#### build_plot_values(gdpinfo, gdpdata):
    """
    Inputs:
      gdpinfo - Dicionário de informações do arquivo de dados do PIB
      gdpdata - PIB de um único país, armazenado em um dicionário onde
                as chaves são strings indicando o ano, e seus valores são
                strings indicando o respectivo PIB daquele ano.

    Output: 
      Retorna uma lista de tuplas no formato (ano, PIB) para os anos
      entre 'min_year' e 'max_year' (incluso), baseado nas informações
      das variáveis gdpinfo e gdpdata. O ano será um int e o PIB será um 
      float.
    """
    
    
#### build_plot_dict(gdpinfo, country_list):
    """
    Inputs:
      gdpinfo      - Dicionário de informações do arquivo de dados do PIB.
      country_list - Lista de strings contendo nomes dos países.

    Output:
      Retorna um dicionário onde as chaves são os nomes dos países
      do input country_list, e seus valores são listas com pares 
      ordenados de tuplas (X, Y) com ano e valor do PIB respectivamente, 
      computados do arquivo CSV descrito no input gdpinfo.

      Países do input country_list que não aparecem no arquivo CSV
      ainda aparecem no dicionário, mas com uma lista vazia em seu
      valor.
    """
    
    
#### render_xy_plot(gdpinfo, country_list, plot_file):
    """
    Inputs:
      gdpinfo      - Dicionário de informações do arquivo de dados do PIB.
      country_list - Lista de strings contendo nomes dos países.
      plot_file    - String que é o nome do arquivo SVG de saída.

    Output:
      Retorna None.

    Ação:
      Cria uma imagem SVG de um gráfico de linha para
      os dados de PIB especificados no input gdpinfo. Leva
      em consideração os países do input country_list.
      A imagem é salva em um arquivo com o nome do input
      plot_file
    """


