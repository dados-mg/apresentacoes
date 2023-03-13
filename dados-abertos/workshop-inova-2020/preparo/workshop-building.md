## Apresentação: ppt ou md ()


## Para usuários: requisitos/programas - deixar para usar todos na nuvem


[GitHub](https://github.com/) - fazer conta?

[Datapackage creator](https://create.frictionlessdata.io/)

[Goodtables.io](https://goodtables.io/)

Editores de texto?

[CKAN](dados.mg.gov.br) - mostrar?


## Roteiro de apresentação e hands-on: tempo aprox.: 1:10 - referência: Workshop Data Frictionless Open Knowledge Foundation (7 minutos de apresentação + 20 minutos de conteúdo introdutório + 40 minutos de hands-on + 10 minutos de dúvidas)

1. Apresentação da Open Knowledge Foundation, apresentações pessoais e introdução ao fellowship program (até 7 min)

2. Apresentação dos objetivos do workshop: introduzir ferramentas (datapackage creator e goodtables) + comunicar a importância de boas práticas de dados e metadados (1min)

3. Objetivos: criar um data package usando o web app do Frictionless Data; criar um arquivo de schema e utilizá-lo usando o web app do goodtables; estar preparado para corrigir erros mais comuns do fluxo de validação de dados (1 min)

4. Dataset - explicação de um dataset a partir de exemplo prático de pesquisa (1 min)

5. Introdução ao datapackage - o que é ? Dado, metadado, esquema (5 min)

6. Justificativas para uso do datapackage: transportar e reusar dados; reduzir fricção em data workflows; possibilitar a pesquisa reprodutível e validação (2 min)

7. Criando um data package: ferramenta online (falar sobre exemplos de interfaces de programação disponíveis - Python, R) e que a base do datapackage é no formato JSON (2 min)

8. Fazendo seu prórpio datapackage: por que metadados? Formas de metadados, upload local, validação e download sem fricção (2 min)

9. Datapackage Creator - Painel de recursos: o que é um recurso? Name, path, settings, adição de recurso (3 min)

10. Datapackage Creator - Painel de esquema: por que formato JSON (legível por máquina e utilizável em qq software)? Que tipo de erro pode ser encontrado? Uso em editores de texto (1 min)

11. Como um datapackage pode ser útil? Formato preciso de arquivo; facimente compartilhado; reprodutibiliade de dados; acessível, interoperável, reusável; validação da integridade dos dados (2 min)

# questões importantes a partir do [Data Frictionless Workshop da OKF](https://www.youtube.com/watch?v=EFQmudQP4io&feature=youtu.be&t=616)

* 40 minutos para hands-on no datapackage creator + goodtables (sem logar e commitar no github), apenas copiaram a URL do raw data num repo de um membro da OKF - por outro lado, a apresentação que precedeu o hands-on foi mais suscinta e a parte do hands-on teve muita descrição sobre cada ferramenta antes de se iniciarem os procedimentos, de fato

* vamos mostrar as especificações ou apenas indicar o local e deixar referências para consultas posteriores (vide limitação do tempo)?

* até qual nível dedetalhe mostrar os significados e possibilidades de cada chave/propriedade? como vamos abordar a propriedade da licença, p. ex.? lembrar de propriedades que não estão como default no datapackage creator, como as do ``csv dialect``

* em vez de baixar o arquivo de datapackage criado, copiaram o schema manualmente e salvaram num editor de texto como formato json

* primeira abertura para dúvidas foi feita após mostrar o datapackage creator e a cópia manual da parte do schema do json; dúvidas foram verbalizadas em vez de escritas no chat (o tempo poderá limitar a leitura e resposta de todas as dúvidas, se feitas via chat) 

* houve a demonstração de um erro de validação de tipo string em vez de number, e a correção não passou pela troca do valor da propriedade no arquivo json, mas simplesmente colar a URL de outro schema.json que já estava pronto no repo

* a recomendação para o erro 'missing values' foi retirar a verificação do goodtables (!?), mas sem explicar como desabilitar essa checagem na interface gráfica ou no arquivo ``goodtables.yml`` 


## Conceitos

1. Datapackage

2. Metadado

3. Schema

4. JSON

5. Recurso

6. Linguagem markdown


## Erros comuns

1. Nome do datapackage contém caracteres especiais, espaços ou letras maiúsculas