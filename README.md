# analise-de-dados-pib-world-bank
## Objetivo:
Funções para exibir gráficos de linha a partir dos dados de PIB disponibilizados no site do banco mundial (https://www.worldbank.org/en/home).

### 1. Importando dados baixados:
Utiliza a biblioteca pandas para ler o arquivo CSV e visualizá-lo.

### 2. Funções:
Um conjunto de quatro funções que tratam os dados do arquivo CSV e exibe as informações de PIB dos países desejados no intervalo de anos definido.

#### read_csv_as_nested_dict(filename, keyfield, separator, quote):
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
