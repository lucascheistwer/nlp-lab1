# nlp-lab1
## LUCAS CHEISTWER :+1:
1. Cuál	es	el	número	de	tokens	en	Moby	Dick?  
MD_cant_tokens = len(moby_dick_tokens_nonpunct)  
MD_cant_tokens  
218621  

2.	Cuál	es	el	número	de	types	en	Moby	Dick?	
MD_cant_types = len(set(moby_dick_tokens_nonpunct))  
MD_cant_types  
17140  

3.	Moby	Dick	type-token	ratio
MD_type_token_ratio = MD_cant_types / MD_cant_tokens  
MD_type_token_ratio  
0.07840051962071347  

4.	WSJ	type-token	ratio
wjs_type_token_ratio = wjs_cant_types / wjs_cant_tokens  
wjs_type_token_ratio  
0.129748424801388  

5. Cuál	de	los	dos	tiene	más	diversidad	léxica?	  
El Wall Street Journal tiene mayor diversidad léxica ya que su ratio es mayor que el de Moby Dick.  

6. Puede pensar una razón por por la cual ese corpus es más diverso que el otro?  
El Wall Street Journal tiene una mayor diversidad léxica ya que al ser un diario, seguramente tenga muchas secciones de diferentes topicos cada una. Esto quiere decir que hay una mayor cantidad de palabras diferentes, en relacion a las palabras totales que hay en el corpus. Moby Dick, al ser una novela, tiene menor diversidad de topicos y por ende de palabras diferentes en relacion a las totales.

7.	Cual	es el	“Maximum	Likelikhood	Estimate	(MLE)” de	la	palabra	“whale” (ballena)	en	Moby	Dick?
\>\>\> cant_Whale_md = text1.count("whale")
\>\>\> cant_whale_md
906
\>\>\> prob_whale_md = (cant_whale_md / MD_cant_types) * 100
\>\>\> prob_whale_md
5.285880980163361

8.	Cuál	es	el MLE	de	“whale”	en	el	corpus	de	WSJ?
\>\>\> cant_whale_wjs = text7.count("whale")
\>\>\> cant_whale_wjs
0
\>\>\> prob_whale_wjs = (cant_whale_wjs / wjs_cant_types) * 100
\>\>\> prob_whale_wjs
0.0
