---
---

O algoritmo de backpropagation funciona através dos seguintes passos:

- Opera através de pequenos lotes, sendo que o algoritmo percorre todo o conjunto de dados de treinamento em cada época. 
- Cada pequeno lote é passado pela rede neural para que os valores de saída sejam calculados. Chamado de passagem para frente. 
- O algoritmo calcula o erro da rede comparando os valores preditos com os valores reais. 
- Em seguida o algorimtmo calcula quanto cada saída contribuiu para o erro. 
- Depois o algoritmo calcula quanto de cada erro foi contribuido peas conexões nas camadas anteriores. 
- Por fim o algoritmo realiza a [[Descida de gradiente]] para ajustar todos os pesos das conexões da rede utilizando os erros calculados do fim para o começo da rede. 