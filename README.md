Qual ator apareceu em mais episódios?  
  
  
----------------------------------------------------------------------------------------------------------------------------------------------  
Gabriel respondeu metade        |     select Participacoes, Atores from personagens;   
  
  
----------------------------------------------------------------------------------------------------------------------------------------------  
Qual episódio com menor duração?  
  
  
----------------------------------------------------------------------------------------------------------------------------------------------  
Qual região com mais casas?  
  
  
----------------------------------------------------------------------------------------------------------------------------------------------  
Quais personagens tiveram sua primeira participação entre 2012 e 2013?  
    
  
----------------------------------------------------------------------------------------------------------------------------------------------  
Qual escritor escreveu o maior número de episódios?  
  
----------------------------------------------------------------------------------------------------------------------------------------------  
Quais as casas da região "North"?  
SELECT * FROM got.casas_got where Regiao = 'North';  
  
----------------------------------------------------------------------------------------------------------------------------------------------  
Quais avaliações de usuário são maiores que 1000?  
SELECT e.Titulo_ep, e.Ep_temporada, e.Data_lancamento, e.Avaliacao_usuario from episodios_got as e where Avaliacao_usuario > 1000;  
  
  
----------------------------------------------------------------------------------------------------------------------------------------------  
Qual o episodio de maior avaliação e qual foi a maior avaliação?  
The Rains of Castamere, Hardhome, Battle of the Bastards, The Winds of Winter   
  
select Avaliacao, Titulo_ep from episodios_got where Avaliacao between '9.9' and '10';  
