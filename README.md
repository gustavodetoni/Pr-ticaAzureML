[pontosazure.json.txt](https://github.com/gustavodetoni/Pr-ticaAzureML/files/14089711/pontosazure.json.txt)
# Prática Azure ML
Estudo pela DIO.me, Machine Learning na Prática no Azure ML.

##Passo a passo
Após a criação do modelo, foi possível ter acesso as Métricas
![scre1](https://github.com/gustavodetoni/Pr-ticaAzureML/assets/106715191/72d38ab9-a6f0-4334-aa03-1625c797f58e)

Em pontos de extremidade, foi feita a implementação do mslearnbike. Agora vamos testar o serviço implantado
- No estúdio Azure Machine Learning, no menu esquerdo, selecionei Endpoints e abri o ponto final em tempo real de previsão de alugueres
- Na página do endpoint em tempo real de previsão de aluguel, visualizei a guia Teste
- No painel Dados de entrada para testar o endpoint, substitui o modelo JSON pelo meu modelo de teste

[Upload {
   "Inputs": { 
     "data": [
       {
         "day": 1,
         "mnth": 1,   
         "year": 2022,
         "season": 2,
         "holiday": 0,
         "weekday": 1,
         "workingday": 1,
         "weathersit": 2, 
         "temp": 0.3, 
         "atemp": 0.3,
         "hum": 0.3,
         "windspeed": 0.3 
       }
     ]    
   },   
   "GlobalParameters": 1.0
 }ing pontosazure.json.txt…]()

 -Resultado esperado e obtido
  {
   "Results": [
     444.27799000000000
   ]
 }

##Sites usados:
```bash
https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/01-machine-learning.html
https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/02-content-safety.html
