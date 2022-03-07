---
---

WOFOST é um modelo de simulação para a análise quantitativa do crescimento e produção de safras anuais. Com WOFOST, você pode calcular o rendimento atingível da colheita, biomassa total, uso de água, etc. para um local com conhecimento sobre solo, cultura, clima e manejo de cultura.

É um modelo mecanicista e dinâmico que explica o crescimento diário da cultura com base nos processos subjacentes, como fotossíntese, respiração e como esses processos são influenciados pelas condições ambientais. 

O crescimento da cultura é calculado em intervalos de tempo de um dia, com base no conhecimento de processos em um nível inferior de integração. Em seguida, os processos de baixo nível são integrados e combinados com outros processos (fenologia, respiração) para explicar o comportamento do sistema em um nível mais alto de integração. No entanto, algumas partes do modelo são descritivas e / ou estáticas. Isso ocorre principalmente porque alguns dos processos envolvidos ainda não foram adequadamente compreendidos.

Avaliação de 3 níveis de produção e crescimento dos cultivos:
- [[Crescimento potencial]]
- [[Crescimento limitado]]
- [[Crescimento reduzido]] - Não avaliada pelo WOFOST

![[Modelo simplificado do WOFOST.png]]

Processos implementados pelo modelo:
- [[Assimilação e respiração]]
- [[Desenvolvimento fenológico]]
- [[Particionamento de matéria seca]]
- [[Transpiração]]

Variáveis de saída:
- Estágio de desnvolvimento dos cultivos.
- Indice de área do cultivo.
- Produção total acima da terra -> Desconta-se raizes.
- Peso total dos orgãos de armazenamento.
- Peso total dos troncos. 
- Peso total das raízes.
- Transpiração do cultivo. 
- Comprimento da raiz
- Umidade do solo -> depende do modelo utilizado.
- Quantidade de água presente no solo. 
- 