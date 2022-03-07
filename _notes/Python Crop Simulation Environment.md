---
---

O pacote Python Crop Simulation Environment é uma biblioteca desenvolvida pela Wageningen University (Holanda). O PCSE fornece o ambiente para implementar modelos de simulação de cultura, as ferramentas para leitura de dados auxiliares (clima, solo, agromanejo) e os componentes para simular processos biofísicos como fenologia, respiração e evapotranspiração.

Trabalha principalmente com 2 modelos:
- [[WOFOST - World Food Studies]]
- [[LINUTL3]]

Para rodar um modelo com dados próprios é preciso 3 coisas:
- Parâmetros do modelo como: Um conjunto de parâmetros de cultura (https://github.com/ajwdewit/WOFOST_crop_parameters), um conjunto de parâmetros de solo e um conjunto de parâmetros de local. 
- Variáveis de condução representadas por dados meteorológicos que podem ser derivados de várias fontes.
- Ações de gestão da cultura que especificam as atividades agrícolas que ocorrerão no campo que é simulado pelo PCSE.

A simulação é possível para alguns cultivos específicos descritos no base de dados do WOFOST. Não existem muitas informações sobre Microgreens e outros vegetais. 

Licensa: [[Licença Pública da União Europeia]]. Uso livre e gratuito 