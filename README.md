# Comparação de modelos de Visão Computacional no reconhecimento de sinais de línguas de sinais

Este projeto comparou três modelos de Visão Computacional treinados sobre imagens do alfabeto manual de línguas de sinais a fim de verificar a sua eficácia em reconhecer estes sinais.

## Modelos utilizados

1. Modelo gerado pela plataforma Teachable Machine, usa o padrão Rede Neural Convolucional e é pretreinado no conjunto de dados ImageNet.   
Foi treinado sobre sinais da Língua brasileira de sinais ou Libras.
2. Modelo encontrado na plataforma Hugging Face, usa o padrão Vision Transformer e é pretreinado no conjunto de dados ImageNet.  
Foi treinado sobre sinais da Língua indiana de sinais (Indian Sign Language - ISL).
3. Modelo treinado com base em um notebook encontrado na plataforma Kaggle, utiliza o padrão Rede Neural Convolucional.  
Foi treinado sobre sinais da Língua americana de sinais (American Sign Language - ASL).

## Conjuntos de dados
- Teachable Machine - RNC (Rede Neural Convolucional)
  - [Conjunto de dados B - Desconhecido pelo modelo.](https://www.kaggle.com/datasets/allanpardinho/libras-cnn)
- Hugging Face - VIT-ISLC (Vision Transformer - Indian Sign Language Classifier)
  - [Conjunto de dados C - Dados de treinamento.](https://www.kaggle.com/datasets/prathumarikeri/indian-sign-language-isl)
  - [Conjunto de dados D - Desconhecido pelo modelo.](https://huggingface.co/datasets/akritRihal/Indian_Sign_Language_dataset)
- Kaggle - RNC (Rede Neural Convolucional)
  - [Conjunto de dados E - Dados de treinamento.](https://www.kaggle.com/datasets/datamunge/sign-language-mnist)
  - [Conjunto de dados F - Desconhecido pelo modelo.](https://www.kaggle.com/datasets/grassknoted/asl-alphabet)

> OBS: O conjunto de dados A, dataset de treinamento do modelo, foi criado a partir da plataforma Teachable Machine e não está disponível para consulta no momento.

## Resultados

| Modelo                  | Acurácia nos datasets de treinamento e teste | Acurácia em datasets desconhecidos pelos modelos |
| ----------------------- | -------------------------------------------- | ------------------------------------------------ |
| RNC (Teachable Machine) | Dataset A - 100%                             | Dataset B - 4,76%                                |
| VIT-ISLC (Hugging Face) | Dataset C - 100%                             | Dataset D - 7,67%                                |
| RNC (Kaggle)            | Dataset E - 99,64%                           | Dataset F - 10,99%                               |

## Conclusão

Acredita-se que é necessário encontrar ou realizar a construção de datasets maiores e mais diversos para treinar os modelos a fim de testar a real capacidade de modelos de Visão Computacional em reconhecer sinais de línguas de sinais. Conforme as comparações feitas aqui, não foi possível verificar alta capacidade nessa tarefa.
