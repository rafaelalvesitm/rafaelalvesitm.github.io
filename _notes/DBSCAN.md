---
---

Links: [[Aprendizado não supervisionado]]

O algoritmo DBSCAN avalia regiões com grande densidade de pontos. Ele funciona nas seguintes etapas: Para cada instância são calculadas quantos pontos existem até uma distancia $\epsilon$; se a instancia contiver ao menos um valor mínimo de vizinhos ela é considerada como central; todas as instâncias visinhas a central são agrupadas no mesmo grupo; Todas as instâncias que não pertencem a um grupo são consideradas outliers. 

![[Exemplo de DBSCAN.png]]