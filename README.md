[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/solenya1/CCS_PREDICTION/blob/main/RC_MODEL.ipynb)

# Prevendo a Resistência à Compressão do Concreto Utilizando Machine Learning


![image](https://www.dsigners.net/wp-content/uploads/2019/10/image1.jpg)

Determinar a resistência à compressão do concreto implica a determinar a qualidade do concreto, normalmente para se obter a medida dessa resistência é realizado um teste de laboratório em que um equipamento mede essa resistência.

A resistencia a compressão do concreto é altamente um função não-linear entre a idade do concreto e seus outros ingredientes como:

* Cimento;
* Agregados;
* Água.

Para realização desse trabalho foram utilizados dados fornecidos pelo Prof. I-Cheng Yeh da Universidade de Chun-Hua. 
Todo os dados podem ser encontrado no [site da universidade](https://archive.ics.uci.edu/ml/datasets/concrete+compressive+strength).


### Source:
_Acknowledgment_
_Many thanks to Prof. I-Cheng Yeh_
_Department of Information Management_
_Chung-Hua University,_
_Hsin Chu, Taiwan 30067, R.O.C._A

### Resumo dos dados:
Número de instancias: 1030
Número de atributos: 9
Atributos divididos entre 8 quantitativos de entrada, e 1 variavel de saida.

### Informações dos atributos:

Given are the variable name, variable type, the measurement unit and a brief description. The concrete compressive strength is the regression problem. The order of this listing corresponds to the order of numerals along the rows of the database.

Name -- Data Type -- Measurement -- Description

Cement (component 1) -- quantitative -- kg in a m3 mixture -- Input Variable
Blast Furnace Slag (component 2) -- quantitative -- kg in a m3 mixture -- Input Variable
Fly Ash (component 3) -- quantitative -- kg in a m3 mixture -- Input Variable
Water (component 4) -- quantitative -- kg in a m3 mixture -- Input Variable
Superplasticizer (component 5) -- quantitative -- kg in a m3 mixture -- Input Variable
Coarse Aggregate (component 6) -- quantitative -- kg in a m3 mixture -- Input Variable
Fine Aggregate (component 7) -- quantitative -- kg in a m3 mixture -- Input Variable
Age -- quantitative -- Day (1~365) -- Input Variable
Concrete compressive strength -- quantitative -- MPa -- Output Variable

### Artigos relevantes do criador dos dados:

Relevant Papers:

**Main**
_1. I-Cheng Yeh, "Modeling of strength of high performance concrete using artificial neural networks," Cement and Concrete Research, Vol. 28, No. 12, pp. 1797-1808 (1998)._

**Others**
_2. I-Cheng Yeh, "Modeling Concrete Strength with Augment-Neuron Networks," J. of Materials in Civil Engineering, ASCE, Vol. 10, No. 4, pp. 263-268 (1998)._

_3. I-Cheng Yeh, "Design of High Performance Concrete Mixture Using Neural Networks," J. of Computing in Civil Engineering, ASCE, Vol. 13, No. 1, pp. 36-42 (1999)._

_4. I-Cheng Yeh, "Prediction of Strength of Fly Ash and Slag Concrete By The Use of Artificial Neural Networks," Journal of the Chinese Institute of Civil and Hydraulic Engineering, Vol. 15, No. 4, pp. 659-663 (2003)._

_5. I-Cheng Yeh, "A mix Proportioning Methodology for Fly Ash and Slag Concrete Using Artificial Neural Networks," Chung Hua Journal of Science and Engineering, Vol. 1, No. 1, pp. 77-84 (2003)._

_6. Yeh, I-Cheng, "Analysis of strength of concrete using design of experiments and neural networks," Journal of Materials in Civil Engineering, ASCE, Vol.18, No.4, pp.597-604 (2006)._


## Confira o notebook

* [RC_MODEL NOTEBOOK](https://github.com/solenya1/CCS_PREDICTION/blob/main/RC_MODEL.ipynb) 
>Notebook contém doda a parte de pré-processamento dos dados e análise juntamente com o teste realizado para verificar o melhor algoritmo separadamente.

*[RC_MODEL_COMPRESSED](https://github.com/solenya1/CCS_PREDICTION/blob/main/RC_MODEL_COMPRESSED.ipynb) 
> Este notebook contém toda a parte de pré-processamento resumida e foca em explorar diferentes combinações de separação de dados para obter o melhor resultado. Digamos que possui um melhor trabalho no algoritmo escolhido para as predições.


 ## Próximos passos

- [x] Melhorar leitura do arquivo com markdown
- [x] verificar em box plot os outliers entre as features
- [x] Verificar além do coef_R2 O RMSE de cada algoritmo
- [ ] Plotar a regressão realizada
- [ ] Fazer deploy do algoritmo no streamlit
