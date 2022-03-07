---
---

Links: [[Aprendizado não supervisionado]]

A análise de componentes principais é uma técnica de [[Redução por projeção]] na qual primeiro se identifica o hyperplano mais próximo dos dados a serem reduzidos para depois realizar a projeção dos mesmos em tal plano. Para realizar tal projeção escolhe-se o plano que preserve a maior variância dos dados e também que reduza o [[Erro médio quadrático]]. 

Essa ténica apresenta vetores ortogonais entre si para cada variância reanescente em ordem decrescente, ou seja, a primeira componente representa a maior variância, a segunda componente é orthogonal a primeira e representa a 2 maior variância, a terceira componente é ortogonal as 2 primeiras e representa a 3 maior variância e assim por diante.

As componentes principais são encontradas através da [[Decomposição de valor singular (SVD)]]. Uma vez encontrada as componente principais basta multiplicar a matrix $X$ pela matrix com $d$ componentes principais, logo $X_{d-proj} = XW_d$.

No scikit-learn é possível especificar tanto o número de componentes a serem utilizadas (1,2,3..) quanto a quantidade de explicação da variância que se espera (entre 0 e 1).

Beneficios:
- Redução de dimensionalidade
- Redução do espaço utilizado para armazenamento e possivelmente processamento. 

Comentários
- Existe uma análise de componentes principais incremental que utiliza lotes dos dados ao invés dos dados por completo. 
- É possível utilizar um Kernel para transformar os dados através das componentes principais. 