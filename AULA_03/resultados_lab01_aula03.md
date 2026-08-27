--- RESULTADOS DO LAB 01 (AULA 03) ---
Mensagem: 'Preciso urgente da segunda via da fatura'
Intenção Predita: [segunda_via]
Vocabulário Filtrado (sem stopwords): ['2a', '2a via', 'aberto', 'acordo', 'acordo pagar', 'alterar', 'alterar endereço', 'app', 'atrasada', 'atualizo', 'atualizo dados', 'boleto', 'cadastramento', 'dados', 'dados residenciais', 'débito', 'débito aberto', 'dívida', 'emitir', 'emitir segunda', 'endereço', 'endereço cadastramento', 'fatura', 'fatura atrasada', 'fazer', 'fazer um', 'gostaria', 'gostaria alterar', 'negociar', 'negociar pagamento', 'no', 'no app', 'onde', 'onde atualizo', 'pagamento', 'pagamento dívida', 'pagar', 'pagar débito', 'posso', 'posso emitir', 'residenciais', 'residenciais no', 'segunda', 'segunda via', 'um', 'um acordo', 'via', 'via boleto', 'via fatura']

#========== PRODUÇÃO DO RELATÓRIO:==============
# 1 - Qual o impacto da remoção de stopwords no tamanho do vocabulário do modelo?
Processamento mais longos e má interpretaçao dos comandos.

# 2 - O que significa a configuração ngram_range=(1, 2) no TfidfVectorizer?
Faz com o sistema interpretar palavras individuas e em pares para verificar o peso das palavras.


# 3 - Como a remoção de palavras genéricas ajuda a evitar classificações incorretas?
Filtrando melhor as entradas, atribuindo a classes corretas. 


[2]
0s
#========== FIM ==============
--- RESULTADOS DO LAB 02 (AULA 03) ---

--- Relatório de Classificação ---
                     precision    recall  f1-score   support

horario_atendimento       0.50      1.00      0.67         1
        localizacao       0.00      0.00      0.00         1
    troca_devolucao       0.00      0.00      0.00         1

           accuracy                           0.33         3
          macro avg       0.17      0.33      0.22         3
       weighted avg       0.17      0.33      0.22         3

--- Matriz de Confusão ---
[[1 0 0]
 [1 0 0]
 [0 1 0]]

#========== PRODUÇÃO DO RELATÓRIO:==============
# 1 - O que representam as métricas Precision, Recall e F1-Score no relatório?
Precision e quantas resposta corretas foram feitas para o retorno das perguntas, Recall e as intenções dos comandos e 
o f1-score são a media de respostas corretas.


# 2 - Como interpretar a diagonal principal da Matriz de Confusão?
A matriz mostra que o bot so consegui interpretar corretamente apenas o horario_atendimento com essa quantidade de dados.



# 3 - Por que a acurácia isolada pode ser enganosa quando temos classes desbalanceadas?
Ela pode mentir por não interpretar todas as classificações corretamente. 

 
