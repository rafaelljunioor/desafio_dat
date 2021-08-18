##### Solução 1 (Sem necessidade de ADHOC) <h5>

  1. Em uma janela de horário permitida (Para evitar sobrecarga e concorrência com os sistemas transacionais), utilizaria uma base stage com a copia dos dados dos sistemas transacionais referentes a D-1. 
  2. O processo de schedule e acompanhamento do job de processamento poderia ser feito com o apache Airflow.
  3. Armazenaria de forma incremental e sumarizada os dados com os cálculos realizados em D-1 em uma base de dados final.
  
##### Solução 2 (ADHOC) 
  
  1. Busca de dados streaming utilizando os recursos do kafka (Producers,Consumers, topics) 
  2. Com os dados buscados em tempo real, poderia ser desenvolvido um processo em python para realizar o calculo com os dados 
  recolhidos via streaming e apresentados para o usuário final. 
  
 
