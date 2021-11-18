# oficina ciclo de abertura de dados 

## 1. etapa de transformação do arquivo para csv (manualmente - não desejada):

- exclusão de células mescladas

- inclusão de coluna mês

- inclusão de coluna ano

- realinhamento das linhas conforme novas colunas

- edição dos nomes das colunas: UNDERSCORE em vez de HÍFEN

- exportação para o formato csv (2 arquivos diferentes)

- salvar arquivos numa pasta nova em C, mover arquivos de dados para pasta \data

- abrir pasta nova no Sublime

- mostrar arquivos csv no Sublime

  - recursos no Sublime para visualização: rainbow csv (marcação de colunas)

- salvar com UTF-8 e mostrar o erro de encoding do acento no mês 

- salvar com UTF-8 + BOM (problema encoding windows)


## 2. etapa de documentação 

- dicionário de dados no datapackage creator https://create.frictionlessdata.io/

	- MARKDOWN = usar descrição com hiperlink no datapackage vai ter o texto sobrescrito pela regra do `dpckan` de trazer o texto do `readme` do repo a ser criado

- salvar datapackage na nova pasta criada

- apartar schema do datapackage, pois têm a mesma estrutura

- corrigir path e comentar convenções não-obrigatórias do design da pasta do repo

- mostrar algumas funcionalidades do json,  

	- mostrar a extensão do validador de json no sublime pretty json (erros de sintaxe - chaves, vírgulas) 

- erros 'didáticos'

	- inclusão dos decimalChar e groupChar e mudança de integer para number

	- inclusão do OWNER_ORG APÓS PUBLICAÇÃO VIA DPCKAN DETECTAR ERRO


## 3. inclusão no repo git

- criar novo repo site github e copiar o https

- configuração github actions (VERIFICAR MASTER OU MAIN)

- na bash, da pasta que será o repo: 

  - git init > git status > git add . > git remote add origin <URL repo> > git commit -m "commit inicial > "git push <URL repo>

- inclusão do texto readme com badge de validação github actions

	- MARKDOWN = usar descrição com hiperlink no datapackage 


## 4.validação inicial com github actions

- mostrar os erros de validação no relatório frictionless e comentar

- inclusão dos decimalChar e groupChar e mudança de integer para number APÓS VALIDAÇÃO DETECTAR ERRO

- correção a partir da mensagem de erro (e replicar para as demais, comentando que é difícil e que tem que abrir o arquivo, via excel ou editor de texto, se não tiver o relatório vistual no site da validação via actions)


## 5. publicação no homologa CGE com dpckan

* REQUISITOS: 
	python, etc 
	ambiente (venv) + 
	inclusão da propriedade owner_org

- criar ambiente 

 	- configuração do ambiente = `$ pyhton -m venv venv`; para ativar, `$ source venv/Scripts/activate`

- instalar pacote `pip install dpckan`

- conferir ambiente de homologação antes de rodar o comando de publicação

	`echo $HOMOLOGA_HOST`

	- mostrar chave de usuário no ckan HOMOLOGA

- publicar

	`dpckan dataset create-H $HOMOLOGA_HOST -k $HOMOLOGA_KEY`

- mostrar o dataest, a badge de validação, os recursos, os dicionários e o datapackage no homologa

- realizar alteração na description da primeira coluna e executar 

# para segundo encontro

- descrição campos variáveis

- textos changelog, contributting

- schema yaml

- git large files

   