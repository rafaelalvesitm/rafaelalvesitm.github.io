---
---

Um mosfet é composto por regiões denominadas Drain (D), Source (S), Gate (G) e Body (B). A origem do termo FET (Field-effect resistor) se dá pois um "capacitor" é formado entre o gate e a região do canal n induzido devido a presença do óxido (isolante). 

![[MOSFET.png]]

- Operação com tensão zero no gate
	- Com tensão zero no gate o transistor opera como um série de dois diodos com resistência MUITO alta e portanto nenhuma corrente passa pelo dispositivo
- Operação com tensão positiva e baixa entre draine source
 - Com a tensão positiva no gate ($V_{GS}$) os portadores majoritarios do substrato tipo p (Lacunas) são enviados para o Body do dispositivo enquanto os portadores minoritários são atraidos para a região próxima ao Gate. Assim quando uma qunatidade suficiente de portadores minoritários está presente nessa região um canal entre o Source e o Drain é criada de forma que é possivel passar corrente por tal canal desde que aplicada uma tensão $V_{DS}$. Nota-se que ($V_{GS}$) também é chamada de tensão limite.
- Operação com tensão positiva e aumentando entre drain e source
	- Neste caso conforme $v_{DS}$ vai aumentando o canal se torna em forma de cunha e portanto a corrente não varia masi uniformente com o aumento da tensão, sendo proporcional a $v_{OV} \times v{DS} - 1/2v_{DS}$\. Também conhecida como região de triodo. 
- Operação com tensão positiva e tensão entre drain e source maior que a efetiva. 
	- Nesta situação a tensão entre dreno e source é igual a tensão efetiva e a tensão entre gate e drain é a tensão limite, logo a profundidade do canal drain é reduzidada a zero e portanto um aumento na tensão entre dreno e source não aumenta a corrente que passa pelo dispositivo. Também conhecida como região de saturação 

## Resumo das operações do Mosfets. 

![[Resumo operação mosfet.png]]

## Operação considerando Vgs fixo

![[Operação mosfets VGS fixo.png]]

## Operação considerando Vds fixo

![[Operação considerando VDS fixo.png]]