[Link para visualização da apresentação do projeto](https://www.canva.com/design/DAFbxA7mwsw/cFhP-ZCdNYL3HtN2hTXz2A/view?utm_content=DAFbxA7mwsw&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton)

Qual ator apareceu em mais episódios?  
SELECT Atores, Participacoes from personagens  
order by Participacoes desc  
limit 3 ;    
    
----------------------------------------------------------------------------------------------------------------------------------------------  
Qual episódio com maior duração?  
select Titulo_ep,Temporada ,Ep_temporada, Duracao from episodios_got  
order by Duracao desc  
limit 1;    
  
  
----------------------------------------------------------------------------------------------------------------------------------------------  
Qual personagens participaram em 2012?  
select Temporada, Ep_temporada, Data_lancamento from episodios_got  
where Data_lancamento between '01-jan-12' AND '31-dec-12'  
order by Data_lancamento;   
      
    
----------------------------------------------------------------------------------------------------------------------------------------------  
Qual escritor escreveu o maior número de episódios?  
select Escritor_1, Count(*) as QtdRepeticoes FROM episodios_got  
group BY Escritor_1  
having Count(*) > 1  
order by QtdRepeticoes desc  
limit 1;   

----------------------------------------------------------------------------------------------------------------------------------------------  
Quais as casas da região "North"?  
select * FROM got.casas_got where Regiao = 'North';  
  
----------------------------------------------------------------------------------------------------------------------------------------------  
Quais avaliações de usuário são maiores que 1000?  
select e.Titulo_ep, e.Ep_temporada, e.Data_lancamento, e.Avaliacao_usuario from episodios_got as e where Avaliacao_usuario > 1000;  
  
  
----------------------------------------------------------------------------------------------------------------------------------------------  
Qual o episodio de maior avaliação e qual foi a maior avaliação?  
The Rains of Castamere, Hardhome, Battle of the Bastards, The Winds of Winter   
  
select Avaliacao, Titulo_ep from episodios_got where Avaliacao between '9.9' and '10';  
  
  
  
 
