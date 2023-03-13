# ROTEIRO SUGERIDO INOVA 2021

## objetivos: o que/como

0. (já foi tópico do INOVA 2020) garantir a qualidade dos dados abertos publicados / a partir da validação contínua de um dataset - pré-requisito

1. minimizar os custos da validação dos dados / com o uso de schemas e automação de validação 

2. gerenciar datasets com grande volume de dados / com uso de ferramenta git large files 

3. automatizar a catalogação de dados abertos / com o uso do pacote dpckan

## requisitos

- oficina de Dados Abertos sem Fricção do INOVA 2020 [vídeo](https://www.youtube.com/watch?v=tZ0bmlnqMuY) e [apresentação](https://ead.prodemge.gov.br/pluginfile.php/19736/mod_resource/content/2/Dados%20Abertos%20sem%20friccao-DCTA-CGE.pdf) 
		
- [instalação do git](https://git-scm.com/) 

- [configuração do proxy para uso do git](https://stackoverflow.com/questions/18356502/github-failed-to-connect-to-github-443-windows-failed-to-connect-to-github)

- [git large files](https://git-lfs.github.com/)

- [python](https://github.com/dados-mg/fluxo-ETL/blob/master/setup-maquina.md#para-rodar-pacote-dpckan)

- [dpckan](https://github.com/dados-mg/dpckan#data-package-manager-para-ckan-dpckan)

- OBS.: o atendimento dos requisitos pode levar muito tempo, o que inviabilizaria a execução simultânea do passo-a-passo pelos participantes, caso o setup completo não tenha sido realizado com sucesso

## tópicos apresentação:

0. sensibilizar para a importância de manutenção do padrão de qualidade dos dados - exemplos

1. retomar definição da qualidade ISO e associação com adoção de padrão de especificação de metadados

2. citar e situar as etapas de um fluxo hipotético de ETL (lembrando que já documentamos um datapackage.json no INOVA 2020), contextualizando como o custo (esforço, tempo) das atividades de validação e publicação pode ser alto, face a outras etapas do fluxo a serem vencidas

3. apresentar o dataset no github 

  3.1. apresentar os schemas em `yaml`

4. configurar o git LFS 

5. configurar o github actions com o pacote frictionless

6. publicar o dataset com o pacote `dpckan`

7. executar uma modificação do dataset que provoque erros de validação

8. apresentar e interpretar os erros

9. corrigir os erros

10. apresentar o novo relatório

11. atualizar o dataset corrigido com o pacote `dpckan`
