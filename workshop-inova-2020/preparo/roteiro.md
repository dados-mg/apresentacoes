# Roteiro hands-on

## pressupostos: 

	- mesmo arquivo (CSV)

	- operações somente em ferramentas online (datapackage creator, github e goodtables.io)

	- distinção do nível de metadados na apresentação (dataset, resource e schema); verificar distinção de metadados de negócio e técnicos

	- preenchimento do datapackage creator com os conceitos de cada campo

	- não é o foco exaurir dúvidas concretas das pessoas ao vivo e lembrar que o material vai estar dispónível com comentários mais detalhados e atualizados com dúvidas que chegarem

1. Preparação da documentação do conjunto de dados 

	1.1. Datapackage creator - explicar os campos (comentar a possibilidade de tb carregar o arquivo pela URL do raw data) e fazer o preenchimento dos metadados em nível de dataset com os conceitos de cada campo, antes de fazer upload do arquivo csv. Enfoque na versão - (retomar material Vitor curso OKBR)

	1.2. Mostrar csv e pedir para pessoas baixarem o arquivo

	1.3. Datapackage creator - fazer upload do csv baixado e preencher o schema panel e resource infos (preencher somente um resource e comentar sobre a possibilidade de carregar mais de um recurso); 

	PAUSA PARA PREENCHIMENTO (2 min)

	1.4. Mostrar que é possível e preciso validar o preview do arquivo gerado. Fazer um erro proposital de deixar maiúsculo o nome do recurso . A validação aqui não faz confronto dos dados com os metadados (ex. tipo do dado - date, integer, number = isso é função do goodtables). Mostrar que é possível fazer o upload de um arquivo de datapackage.json já existente

	PAUSA PARA TESTES (1 min)

	1.5. Baixar o arquivo datapackage.json 

2. Github: criar repositório novo (VAZIO)

	PAUSA PARA CRIAÇÃO DO REPO (1 min)

3. Validando o datapackage criado com Goodtables

	3.1. Logar com github e sincronizar novo repositório (manage sources = avaliable repositories)

	PAUSA PARA SINCRONIZAÇÃO

	![image](workshop-inova/goodtables-github-1stauthorization.png)

 	3.2. Fazer upload do arquivo csv com seu datapackage.json no github

 	PAUSA PARA UPLOAD

	3.3. Verificar resultado da validação (dashboard)

	3.4. Comentar principais erros de validação e citar referência da documentação do pacote frictionless data py

		3.4.1. sobre o arquivo: 

			- header; 

			- extra value;

			- blak row; 

			- duplicate row;

		3.4.2. sobre as variáveis:

			- formato de data (ISO X excell X default goodtables.io)

			- formato dos números: separador de milhar e de decimais 

	3.5. Colar referência em markdown do badge de validação no readme do repo do guthub


## Comentários úteis:

1. Link do arquivo para leitura e interpretação das ferramentas online (datapackage creator e goodtables) deve ser sempre o do raw, [caso contrário há o risco de ser interpretado como HTML em vez de arquivo com formato tabular (CSV)](https://github.com/dados-mg/apresentacoes/issues/2)

2. Renderização automática de CSV no github: [somente arquivos com vírgulas como separadores](https://github.com/dados-mg/projetos-abertura-conjuntos-dados/pull/1) permitem o github apresentar o arquivo com visualização tabular, similar a que se tem quando se abre o csv no excell 

3. Explicar o delay entre o resultado da validação automática e a sinalização do badge de validação

## Follow up

1. Atualizar [guia para conferêcia de arquivos tabulares](https://github.com/dados-mg/inventario-de-dados/blob/master/guia-para-conferencia-de-dados-abertos.md) no inventário de dados
