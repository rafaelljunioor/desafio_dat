##### Solução 1 <h5>

  1. Em uma janela de horário permitida (Para evitar sobrecarda e concorrência com os sistemas transacionais), utilizaria uma base stage com a copia dos dados dos sistemas transacionais referentes a D-1. 
  2. O processo de schedule e acompanhamento do job de processamento poderia ser feito com o apache Airflow.
  3. Armazenaria de forma incremental e sumarizada os dados com os cálculos realizados em D-1 em um ambiente hadoop.
 
