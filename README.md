# Calendario Mestre

O Calendario mestre é uma tabela de dados onde temos todas as informações de datas e todas as suas atribuições.
Por exemplo, você tem uma data e quer extrair todas as informações de anos, mêses e dias, trimestre, semestre.
Ela vai pegar estes dados acima e vai criar uma lista / autocalendario até da data de hoje e hoje que você para atualizar o seu controle essa formula vai serpre pegar a data do dia atual. Independente de quando você usar o intervalo destes dados estarão formatados para você.


## Let's Go

Vamos iniciar importando os dados 

![image](https://user-images.githubusercontent.com/112008347/188286650-0494aac0-c716-4124-a0ae-dc2fed13fc58.png)

Vamos em Outro > Consulta Nula

![image](https://user-images.githubusercontent.com/112008347/188286670-5f75ed09-ae9a-4fde-af34-8efe260dc7df.png)

Vamos utilizar a formula: =#date (1900,1,1) 
Para identifiar a primeira data do calendario que o excel consegue identificar 

Em seguida vamos utilizar a formula: =List.Dates(Fonte, Number.From(DateTime.LocalNow()) - Number.From(Fonte), #duration (1,0,0,0))

Ela vai pegar esta data acima e vai criar uma lista / autocalendario até da data de hoje e toda vez que você for atualizar o seu controle essa formula vai serpre pegar a data do dia atual.
Idependente de quando você for utilizar o range destas datas vai estar formatado para você.

![image](https://user-images.githubusercontent.com/112008347/188286915-75d14126-59f0-48bb-b058-ed9f9ba19ee5.png)

## ► Tranformando a lista em tabela 

![image](https://user-images.githubusercontent.com/112008347/188286978-6cdb6bde-c8aa-4a07-a58c-f760f7490c86.png)

Vamos adicionar colunas importantes para as nossas analises 

![image](https://user-images.githubusercontent.com/112008347/188287157-fb482dcf-603c-4f23-8fad-9284d6c019c9.png)

![image](https://user-images.githubusercontent.com/112008347/188287178-b26164d8-c9c4-4c5d-ad26-436b6131f902.png)

## Relacionando as tabelas e a cardinalidade

![image](https://user-images.githubusercontent.com/112008347/188289531-b043919c-7b6d-4148-958d-b5cf605258ec.png)

