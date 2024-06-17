# André Borges


## Introdução

Este README documenta o processo de transformação de dados para análise. O objetivo é preparar os dados para modelagem e posterior análise.


## 1. Verificação dos Cabeçalhos e Tipos de Dados
Verificar se os cabeçalhos das colunas correspondem aos nomes das variáveis ​​esperadas.
Garantir que os tipos de dados das colunas sejam apropriados, como texto, numérico ou data.
Corrigir inconsistências nos tipos de dados, se necessário.
## 2. Conversão de Valores Monetários
Converter valores monetários para o tipo de dados double preciso para garantir precisão nos cálculos.
Padronizar a formatação dos valores monetários, como casas decimais e separadores de milhar.
## 3. Tratamento de Valores Nulos
dentificar e analisar a presença de valores nulos em cada coluna.
Decidir se os valores nulos devem ser removidos, preenchidos ou tratados de outra forma.
Considerar a causa dos valores nulos e o impacto na análise.
## 4. Análise de Funcionários sem Superiores
Identificar funcionários com valores nulos no campo Super_ssn (SSN do supervisor).
Verificar se esses funcionários representam gerentes sem subordinados.
Se existirem gerentes sem subordinados, avaliar a necessidade de manter esses registros ou preencher os valores nulos.
## 5. Análise de Departamentos sem Gerentes
Verificar se existem departamentos sem gerentes identificados (nulo no campo Manager_ssn).
Se existirem departamentos sem gerentes, investigar a causa e avaliar as opções:
Remover departamentos sem gerentes.
Atribuir gerentes a esses departamentos com base em informações adicionais.
Preencher os valores nulos com um valor padrão (por exemplo, "Gerente Desconhecido").
## 6. Separação de Colunas Complexas
Identificar colunas que contêm múltiplas informações em um único campo.
Separar essas colunas em campos distintos para facilitar a análise e manipulação dos dados.
Exemplo: separar uma coluna "Nome Completo" em colunas separadas para "Nome" e "Sobrenome".
## 7. Mesclagem de Tabelas Employee e Department
Criar uma nova tabela mesclando as tabelas employee e department com base no campo department_id.
Essa tabela conterá informações de funcionários e seus departamentos associados.
Considerar o tipo de junção apropriado (interna, externa esquerda, externa direita etc.) de acordo com o objetivo da análise.
## 8. Eliminação de Colunas Desnecessárias
Identificar e remover colunas que não sejam relevantes para a análise ou que estejam duplicadas em outras colunas.
Eliminar colunas com valores nulos em grande parte ou que não forneçam informações úteis.
Manter apenas as colunas que contribuem para os objetivos da análise.
