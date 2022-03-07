---
---

dam, que significa estimativa de momento adaptável, combina as ideias de [[Otimização de momento]]e [[RMSProp]]: assim como a otimização de momento, ele mantém o controle de uma média exponencialmente decadente de gradientes anteriores e, assim como RMSProp, mantém trilha de uma média exponencialmente decadente de gradientes quadrados anteriores. Dada pelas equações :

1. $$ m \leftarrow \beta_1m - (1 - \beta_1)\nabla_\theta J(\theta)$$
2. $$s \leftarrow \beta_2 s + (1 - \beta_2) \nabla_\theta J(\theta) ⊗  \nabla_\theta J(\theta)  $$
3. $$\hat{m} \leftarrow \frac{m}{1 - \beta_1^t}$$ 
4. $$\hat{s} \leftarrow \frac{s}{1 - \beta_2^t} $$ 
5. $$\theta \leftarrow \theta + \eta \hat{m} ⊘ \sqrt{\hat{s} +\epsilon)}$$