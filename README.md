# ELV_OleoRefrigerante
Este repositório foi criado com os arquivos de termo para ELV de mistura binária

[1] - Os arquivos foram finalizados ao em dez/2017 e desde então não sofreram alterações. Todos os arquivos estão rodando corretamente.
[2] - Os arquivos que aqui estão são uma cópia dos arquivos que estavam no meu correio 
[3] - Abaixo alguns comentários que inseri no e-mail quando fiz o upload desses arquivos no gmail:

  Testei os dados(*) com o novo modelo termodinâmico 

Os dados testados foram:
a - R-600a/AB ISO 5: do artigo (estão em anexo) - foram capturados pelo Carlos
b - R-600a/POE ISO 7: do artigo - capturados pelo Carlos; e também da dissertação do Moisés

As misturas:
R-600a/AB ISO 5: temos muitas dúvidas quanto aos dados
R-600a/POE ISO 7: deu melhor concordância com os dados da dissertação


O modelo:
- entalpia está "batendo" bem com os do artigo; a entropia nem tanto
- nos arquivo zData8 e zData9 (R-600a/AB ISO 5 e R-600a/POE ISO 7, respectivamente) já contam com um orientado a objeto para estimar o parâmetro kij (ver 11-80 do livro Sanford Klein).
- levanta pB para um único ponto (Bubble.py) e para uma curva de pontos (BubbleP_curvepoints.py). E para fazer isso foi criada a classe BubbleP_class que está dentro do Bubble.py
- o EnthalpyEntropy.py é onde se faz os cálculos de h e s. Para tanto, foi criada a função getting_the_results_from_FlashAlgorithm_main() que veio do arquivo FlashAlgorithm_main.py.
