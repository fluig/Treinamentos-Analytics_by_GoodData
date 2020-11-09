# Treinamento-GoodData

Neste repositório você irá encontrar o projeto utilizado no treinamento de GoodData, permitindo que vocês façam download do respectivo arquivos e pratiquem!

---------------------------------------------------------------------------------------------------------------------------------

### Recursos úteis

* Será necessária a instalação do CloudConnect (link para download: https://analytics.totvs.com.br/download-cc.html)
* Importação do Banco de Dados GoodData (SQL Server) identificado como Fonte de Dados.
* Configuração do Agent, através do arquivo config.properties (Definindo a extração do banco de dados SQL, através do JDBC enviando as informações via FTP GoodData) 
* Criação do modelo lógico de dados (construido datasets e os dados classificados atributos e de fatos).
* Criação do relacionamento entre os datasets, através de chaves primárias e estrangeiras.
* Criação o graphs ETL para o tratamento dos dados.
* Utilizando os componentes disponíveis no graph: 
Componente Reader CSVReader (lê o arquivo de uma pasta no workspace do CloudConnect), componente Reformat (concatenou dados, formatou os números e data),  e o componente GD Dataset Writer (fez upload dos dados no projeto na nuvem GoodData).Também utilizamos outros componentes: DBInputTable, Trash, FastShort, SimpleCopy, ExtFilter, etc). 
* Criação de parâmetros no workspace e utilização do arquivo de lib no CloudConnect.
* Criação de metadados entre os componentes do graph.
* Definição da ordem de execução dos componentes utilizando "phase" no graph ETL _Main.
* Realizando Deploy do projeto na nuvem GoodData.
* Configuração do arquivo Agent para automatização do ETL.

### Origem do desenvolvimento

Projeto desenvolvido pelo time fluig Academy para o treinamento de GoodData.

###  Acesse o curso no portal fluig Academy

GoodData: http://academy.fluig.com/ng/student/courses/gooddata/

Desenvolvedor GoodData: https://academy.fluig.com/courses/desenvolvedor-gooddata


### Observações

No workspace.prm é necessário configurar os parâmetros comentados com os dados da sua conta de acesso ao projeto: 
  * E-mail
  * Senha
  * ID do Projeto 
  * Nome do arquivo zip que foi enviado para o FTP GoodData
------------------------------------------------------------------------------------------------------------------------------------
 * No arquivo config.properties do Agent é necessário substituir as tags do arquivo confome informado no treinamento. 
 * É necessário criar agendamento de tarefas apontado para o arquivo Run.bat para executar de acordo com a necessidade do negócio.

------------------------------------------------------------------------------------------------------------------------------------



### Fique ligado!

Os projetos compartilhados no repositório do GitHub não possuem suporte, pois é um ambiente de compartilhamento comunitário, sendo o modelo AS IS.  
