# roteiro oficina v2 abr-22

## recap

1. características dados abertos

2. escolha da base de exemplo - qual é e onde está

3. transformação da base para csv

4. transformação dos nomes dos cabeçalhos

## etapas da abertura e publicação

5. esquema das etapas (não-lineares)
	- pontuar o protagonismo do órgão publicador e auxílio da DCTA
	- comentar sobre a restrição das informações
	- 'bônus' = controle de versão (benefício de acompanhar integridade da base e visualizar validação automática online)

6. dicionário de dados
	- mostrar o site da especificação
	- explicar que vou alternar entre a linha de comando, a apresentação estática em pptx e sites de referência

7. início mão-na-massa:
	- instalação ambiente python
	- ativação ambiente python
	- instalação de pacotes

8. criação de pasta, adição do arquivo csv
	- aumentar a tela do terminal
	- explicar o pq do ambiente e a lógica de pacotes e dependências
	- mostrar o ambiente criado na pasta

9. descrição dos dados
	- frictionless describe (formato yaml)
	- mostrar especificação padrão json (yaml como experiência mais amigável de criação e edição)
	
	````frictionless describe --yaml --type package data/*
	````
	- criação de pasta 'data' para recursos como boa prática
	- mover o arquivo csv para 'data' e mostrar o datapackage.yaml 
	- abrir o datapackage.yaml no Sublime
	- mostrar o arquivo csv no excel, no sublime com rainbow csv 
	- mostrar como as colunas ficam documentadas no datapackage
	- regras de negócio dos dados não são automatizáveis
	
	- validar o datapackage: frictionless validate datapackage.yaml

10. principais erros de validação (simular):

	- name/título: do recurso e do conjunto

	- path

	- tipos de dados de cada coluna

	- lembrar que existe uma lista de erros comuns e que será enviada junto com o material de referência

	- propósito: refletir os metadados no datapackage

- **pq tudo isso?** dicionário de dados pode estar em word, em pdf; mas para o dado ser acessado por códigos, ser corretamente interpretado e reutilizado, esses metadados precisam estar nestas linguagens específicas

11. transformação do yaml para json

	````frictionless describe --type package --stats --json datapackage.yaml > datapackage.json
	````
	- mostrar o arquivo 'json' na pasta
	- validar o arquivo 'json' = frictionless validate datapackage.json
	- comentar sobre as múltiplas possibilidaddes de errar a sintaxe na edição do formato json

12. controle de versão no github
	- mostrar um conjunto versionado com validação automatizada
	- inicializar o repositório na bash com git init
	- criação do gitignore para não trackear o ambiente 'venv'
	- git add .
	- git commit -m (mensagem)
	- git branch -M main
	- git push
	- mostrar o repositório
	- adicionar as instruções para incorporar validação automática no github
	- mostrar o relatório de validação

13. publicação

	- dpckan dataset create
	- owner_org

	````frictionless describe --type package --stats --json datapackage.yaml > datapackage.json
	````
	- dpckan dataset create
	- mostrar o conjunto criado

14. conversa

	- curva de aprendizado, parceria, benefícios esperados

15. próximos passos

	- máquina preparada (apoio da TI para liberação do proxy), 
	- base escolhida
	- testes
	- reunião de publicação = final do início (acordo da criação de organização e usuário)

