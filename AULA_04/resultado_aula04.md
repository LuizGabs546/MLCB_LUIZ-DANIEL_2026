            ==========KNN==========

Classification Report:
                    precision    recall  f1-score   support

logistica_entregas       1.00      1.00      1.00        10
       reclamacoes       1.00      1.00      1.00        10
           suporte       1.00      1.00      1.00        10
 trocas_devolucoes       1.00      1.00      1.00        10
            vendas       1.00      1.00      1.00        10

          accuracy                           1.00        50
         macro avg       1.00      1.00      1.00        50
      weighted avg       1.00      1.00      1.00        50


Confusion Matrix:
[[10  0  0  0  0]
 [ 0 10  0  0  0]
 [ 0  0 10  0  0]
 [ 0  0  0 10  0]
 [ 0  0  0  0 10]

 # Nenhuma das classes se confundiu 


                ==========ARVORE==========

Classification Report:
                    precision    recall  f1-score   support

logistica_entregas       0.80      0.67      0.73         6
       reclamacoes       1.00      0.33      0.50         6
           suporte       1.00      1.00      1.00         6
 trocas_devolucoes       0.62      0.83      0.71         6
            vendas       0.67      1.00      0.80         6

          accuracy                           0.77        30
         macro avg       0.82      0.77      0.75        30
      weighted avg       0.82      0.77      0.75        30


Confusion Matrix:
[[4 0 0 0 2]
 [1 2 0 3 0]
 [0 0 6 0 0]
 [0 0 0 5 1]
 [0 0 0 0 6]

 # Todas se Confundiram, menos a classe de "suporte" 
 
 # 2 - 
        === INICIANDO BATERIA DE TESTES (10 INPUTS OBRIGATÓRIOS) ===

[Teste 1/10]
Digite a frase do cliente: ola

Bot: [FALLBACK - Confiança baixa: 33.3%]
Desculpe, não consegui entender sua solicitação. Por favor, aguarde um momento enquanto encaminho você para um atendente humano...
============================================================

[Teste 2/10]
Digite a frase do cliente: quero ver saldo

Bot [Intenção: VENDAS | Confiança: 66.7%]: Posso ajudar com a compra de móveis. Qual produto você deseja comprar?
============================================================

[Teste 3/10]
Digite a frase do cliente: preciso de ajuda 

Bot [Intenção: SUPORTE | Confiança: 66.7%]: Claro! Posso ajudar com montagem, manuais e assistência. Qual é o problema?
============================================================

[Teste 4/10]
Digite a frase do cliente: quero atendimento 

Bot [Intenção: RECLAMACOES | Confiança: 66.7%]: Lamento pelo ocorrido. Vou registrar sua reclamação. Pode me contar mais detalhes?
============================================================

[Teste 5/10]
Digite a frase do cliente: ruim demais 

Bot: [FALLBACK - Confiança baixa: 33.3%]
Desculpe, não consegui entender sua solicitação. Por favor, aguarde um momento enquanto encaminho você para um atendente humano...

# O KNN teve bons retornos em cada classe e fallback 

      === INICIANDO BATERIA DE TESTES (8 INPUTS OBRIGATÓRIOS) ===

[Teste 1/8]
Digite a frase do cliente: quero atendimento 

Bot [Intenção: VENDAS | Confiança: 100.0%]:
Posso ajudar com a compra de móveis. Qual produto você deseja comprar?
============================================================

[Teste 2/8]
Digite a frase do cliente: quero fazer uma compra 

Bot [Intenção: RECLAMACOES | Confiança: 100.0%]:
Lamento pelo ocorrido. Vou registrar sua reclamação. Pode me contar mais detalhes?
============================================================

[Teste 3/8]
Digite a frase do cliente: muito ruim, pessimo 

Bot [Intenção: TROCAS_DEVOLUCOES | Confiança: 100.0%]:
Posso ajudar com trocas e devoluções. Qual produto você deseja trocar ou devolver?

# Arvore de decisão teve um pessimo desempenho 

# 3 - O melhor desempenho foi com o KNN, pois ele faz a associação das frases a tribuindo o maior valor as classe pertencente, como clientes procuram comandos diretos o KNN e mais eficiente nessa separação.

