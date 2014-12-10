<Nome do Projeto>
=================
Plano de Gerenciamento de Configuração
======================================
Versão &lt;4.00&gt;
------------------


Histórico de Versões
--------------------

|Data                |Versão       |Descrição               |Autor          |
|--------------------|-------------|------------------------|---------------|
|_&lt;05/12/2104&gt;_|_&lt;1.00&gt;_|_&lt;Versão inicial&gt;_|_&lt;Bruno Camargo&gt;_|
|_&lt;07/12/2014&gt;_|_&lt;2.00&gt;_|_&lt;Nova Versão&gt;_  |_&lt;Felipe Andrade&gt;_|
|_&lt;09/12/2014&gt;_|_&lt;3.00&gt;_|_&lt;Nova Versão&gt;_  |_&lt;Carlos Bezerra&gt;_|
|_&lt;10/12/2014&gt;_|_&lt;4.00&gt;_|_&lt;Nova Versão&gt;_  |_&lt;Felipe Andrade&gt;_|



1. Introdução
==============

O Plano de Gerenciamento de Configuração tem como objetivo principal documentar o sistema de gestão de configuração definido para o Projeto SPT-SIS, apresentando todas as tarefas, os seu padrões, procedimentos, atividades e responsáveis. Portanto, podemos afirmar que a aplicação deste plano visa garantir a integridade de códigos fonte e demais produtos do sistema SPT-SIS, permitindo acompanhamento destes itens durante todo o ciclo de vida do projeto, preservando o histórico de evolução dos sistemas da instituição.

1.1 Finalidade
---------------
Este Plano de Gerenciamento de Configuração destina-se a todos os projetos iniciados no ambiente de desenvolvimento da empresa SPT-SIS e tem como obejtivo principal descrever a organização, nomeclatura e regras para versionamento do projeto SPT-SIS. Portanto, o plano auxiliará os profissionais de desenvolvimento e produção a gerenciar o estado dos itens de configuração, controlar  as mudanças em itens de configuração e principalmente rastrear tais modificações ao longo do ciclo de vida do projeto.

1.2 Escopo
----------
Este plano é destinado a todos os profissionais responsáveis pelo desenvolvimento do sistema SPT-SIS, e deverá ser seguido durante todo o ciclo de vida do produto. O referido plano abrangerá todos os dados relevantes definidos nos projetos relacionados ao sistema SPT-SIS, incluindo ferramentes, hardware, responsabilidades, cronogramas, e dará subsídios a equipe para controlar as etapas de desenvolvimento do software SPT-SIS.

1.3 Definições, Acrônimos e Abreviações
---------------------------------------

|Sigla	  |Descrição    |                                                           
|---------|-------------|                                                                                                                            
|BASELINE|Conjunto de itens de configuração que conseguiram um estado comprovado de estabilidade. |
|CCM	 |Comitê para o Controle de Mudanças.  |
|CM | Controle de Mudanças |
|GC	 |Gerência de Configuração |
|PGC | Plano de Gerenciamento de Configuração | 
|RUP	 |Rational Unified Process |   
|SM	 |Solicitação de mudança                                                                 
|SPT-SIS    |Sistema de Proteção de Trânsito |

Tabela 01 - definições, acrônimos e abreviações.

1.4 Referências
---------------
Não se aplica.

1.5 Visão Geral
---------------
O documento referente ao plano de configuração esta organizado em seções e sub-seções, citando os itens de configuração, a organização da estrutura dos diretórios e a organização dos papéis e responsabilidades.

Seção 2 - nesta seção são definidos os papéis, equipes, responsabilidades,ferramentas, ambiente e infra-estrutura necessários ao pleno gerenciamento de configuração de software.

Seção 3 - nesta seção são definidos os métodos de identificação dos documentos, artefatos e itens de configuração, as baselines, a estrutura de diretórios do repositório onde os itens serão armazenados e o padrão para criação de tags.

Seção 4 - nesta seção são definidos os padrões e procedimentos que deverão ser seguidos para aprovação e liberação de uma versão dos itens de configuração.

Seção 5 - nesta seção são definidos as ferramentas, recusros e treinamentos necessários para que a equipe possa implementar as atividades definidas no PGS.

Seção 6 - nesta seção são definidos em que momento as auditorias serão realizadas, o que será verificado e como os problemas serão reportados.


2. Gerenciamento de Configuração de Software
============================================

2.1 Organização, Responsabilidades e Interfaces
------------------------------------------------
|Papéis | Equipe | Responsabilidade |                                                             
|-------|---------|-----------------|                                                                                                                            
|Gerente de Configuração |Carlos Bezerra |Estabelecer Políticas de GC, Escrever Plano de GC, Configurar Ambiente de GC, Criar Espaços de Trabalho de Integração, Criar Baselines e Promover Baselines|
|CCM | Bruno Camargo e Carlos Bezerra | Estabelecer Processo de Controle de Mudanças e Revisar Solicitação de Mudança |
|Desenvolvedor | Carlos Bezerra e Felipe Andrade | Seguir os padrões e procedimentos definidos no Plano de Gerência e Configuração |
|Todos os Papéis | Bruno Camargo, Carlos Bezerra e Felipe Andrade | Enviar Solicitação de Mudança e Atualizar Solicitação de Mudança |

Tabela 02 - organização, responsabilidades e interfaces.

2.2 Ferramentas, Ambiente e Infra-estrutura
-------------------------------------------
 
### 2.2.1 Ferramentas a serem utilizadas para a Gerência de Configuração
----------------------------------

|Ferramenta | Tipo | Descrição | Versão |                                                            
|-----------|------|-----------|---------|                                                                                                                            
|IDE Eclipse | Plataforma de Desenvolvimento | É uma IDE para desenvolvimento Java, com suporte a diversas linguagens e plugins. | Eclipse Luna 4.4.1 |
|Git | Controle de Versão |Sistema para Controle de Verão |1.9.4 |
|Egit Plugin | Acesso ao Repositório | Cliente para o Git Integrado ao Windows | 1.4.8.121 |

Tabela 03 - ferramentas para a gerência de configuração.

### 2.2.2 Ferramentas do ambiente de desenvolvimento
----------------------------------

|Tipo | Ferramenta | Versão |                                                            
|-----|------------|--------|                                                                                                                            
|Sistema Operacional | Windows 7 Professional | SP1 |
|Cronograma | Microsoft Office Project | 2013 |
|Planilha | Microsoft Office Excel | 2010 |
|Editor de Texto | Microsoft Office Word | 2010 |
|Controle de Versão | Git | 1.9.4 |
|Plataforma de Desenvolvimento | Eclipse Luna | 4.4.1 |
|Planilha | Microsoft Office Excel | 2010 |
|Banco de Dados | MySQL | 5.0 |
|Comunicação | E-mail / Skype / Whatsapp |  |

Tabela 04 - ferramentas para o desenvolvimento.


### 2.2.3 Estrutura do Ambiente
----------------------------------

|Ambiente | Descrição | Transição |                                                            
|---------|-----------|-----------|                                                                                                                            
|Desenvolvimento | É o ambiente que será utilizado para a codificação do sistema. | O componente atingirá a maturidade quando os requisitos forem supridos e testados pelos desenvolvedores através dos testes unitários. |
|Integração | É o ambiente que servirá para os testes de integração | Quando a comunicação entre os módulos atinge um estágio aceitável de funcionamento. |
|Banco de Dados | É o ambiente onde os dados serão armazenados | Ambiente que conterá o banco de dados do sistema. |

Tabela 05 - estrutura do ambiente.

### 2.2.4 Estrutura dos Equipamentos
----------------------------------

|QTD | Ambientes | Configuração de Hardware |  Configuração do Software |                                                         
|----|-----------|--------------------------|--------------------------|                                                                                                                           
|3 | Desenvolvedor | Processador 2.3GHz, Memória de 4GB ou Superior, Disco Rígido de 500GB ou Superior e IP 192.168.0.50 ~ 52| Windows 7 Professional SP1, Eclipse Luna 4.4.1, Git 1.9.4, Egit 1.4.8.121, Office 2010, Mysql 5.0 e Skype |
|1 | Integração | Processador 3.0GHz, Memória de 16GB ou Superior, Disco Rígido de 2TB ou Superior e IP 192.168.0.10 | Centos 6.5 64 bits, Java 1.8 SDK, Git 1.9.4, Maven Plugin 2.8, MySQL Database Plugin 1.0 e Jenkins 1.588 |
|1 | Banco de Dados | Processador 2.3 GHz ou Superior, Memória de 8GB ou Superior, Disco Rígido de 1TB ou Superior e IP 192.168.0.20 | Centos 6.5 64 bits e MySQL 5.0 |

Tabela 06 - estrutura dos equipamentos.

3. O Programa de Gerenciamento de Configuração
==============================================

3.1 Identificação da Configuração
---------------------------------
### 3.1.1 Métodos de Identificação
----------------------------------
Todos os documentos, artefatos e itens de configuração, devem ser nomeados com as iniciais do sistema SPT-SIS, com base na nomenclatura descrita a seguir:

&lt;SPT-SIS&gt;-&lt;ID_ARTEFATO&gt;-&lt;DATA&gt;-&lt;VERSÃO&gt;
 
Onde: 
 
| Nomenclatura | Descrição |
|--------------|-----------|
|SPT-SIS       | Iniciais do sistema|
|ID_ARTEFATO   | Identificação do item de configuração conforme tabela 08.|
|VERSÃO        |Conforme tabela 09.|

Tabela 07 - nomenclatura.

|ID             | Item de Configuração   |
|---------------|------------------------|
|REQ            |Documento de Requisitos |
|PT             |Plano de Testes         |
|CF             |Código Fonte            |

Tabela 08 - id e itens de configuração.

| Versão       | Padrão   |
|--------------|-----------|
|Modificações Importantes |X          |
|Correções Planejadas     |Y          |
|Coreções de Bugs         |Z          |
|Exemplo                  |X.Y.Z      |

Tabela 09 - padrão de versionamento.

Sempre que o dígito X for incrementado, os dígitos Y e Z deverão ser setados novamente para 0.

Sempre que o Y for incrementado, o dígito Z deverá ser setado para 0.

É importante salientar que todas as letras dos nomes que compõem os documentos, artefatos e itens de configuração devem estar em caixa alta, os espaços em branco e sem acentuação.

### 3.1.2 Itens de Configuração

| Item de Configuração                 | Responsável na equipe	     | Inclusão em Baseline |
|----------------------------------------|-----------------------------|----------------------|
|Documento de Requisitos|Carlos Bezerra|Quando o cliente validar e aprovar.|
|Plano de Testes|Carlos Bezerra e Felipe Andrade|Após liberação por parte do gerente de testes.|
|Código Fonte|Carlos Bezerra e Felipe Andrade|Após realização dos testes e aprovação por parte do cliente. |

Tabela 10 - itens de configuração.


### 3.1.3 Baselines do Projeto

As baselines são geradas assim que uma vesão de homologação do sistema SPT-SIS é aceita formalmente pelo cliente. Dessa forma, é gerada uma versão para baseline do sistema contemplando documento de requisitos, casos de testes e código fonte do sistema.

| Baseline            | Responsável na equipe | Itens |
|---------------------|-----------------------|-------|
|Requisitos           |Carlos Bezerra         |Documento de Requisitos|
|Desenvolvimento      |Carlos Bezerra         |Código Fonte|
|Testes               |Carlos Bezerra         |Plano de Testes|

Tabela 11 - baselines.

As tags devem ser geradas a cada nova versão seguindo o padrão abaixo:

&lt;SPT-SIS&gt;-&lt;RELEASE&gt;-&lt;VERSÃO&gt;

Onde: 
 
| Nomenclatura | Descrição |
|--------------|-----------|
|SPT-SIS       | Iniciais do sistema|
|RELEASE       | Palavra chave
|VERSÃO        | Conforme tabela 09.|

Tabela 12 - nomenclatura tags.


### 3.1.4 Estrutura do Repositório de Versões

| Diretório                | Arquivos     | 
|--------------------------|--------------|
| /SPT-SIS/Documentação    | Documento de Requisitos e Plano de Testes |
| /SPT-SIS/Fontes          | Código Fonte |

Tabela 13 - estrutura de diretórios.




3.2 Controle de Configuração e Mudança
--------------------------------------

### 3.2.1 Processamento e Aprovação de Solicitações de Mudança

As solicitações de mudanças das Baselines serão realizadas através da ferramenta Jira.

**Status das Issues**

| Atividade                        			 | Descrição	     											   				| Responsabilidade      |
|----------------------------------------|------------------------------------------------|-----------------------|
|Aberto																	 | Criação da solicitação.												| Todos									|
|Em Análise															 | Análise da solicitação													| Analista de sistemas	|
|Analisado															 | Aguardando desenvolvimento											| Analista de sistemas	|
|Em desenvolvimento											 | Solicitação sendo desenvolvida									| Desenvolvedor					|
|Desenvolvido														 | Aguardando teste																| Desenvolvedor					|
|Em testes															 | Solicitação em teste														| Testador							|
|Testado com erro												 | Aguardando desenvolvimento											| Testador							|
|Testado sem erro												 | Solicitação esperando finalização pelo analista|	Testador							|
|Finalizado															 | Solicitação finalizada													| Analista							|


### 3.2.2 Comitê de Controle de Mudança (CCB)

O comitê de Controle de Mudanças (CCM) será formado por Analista de Sistemas e Gerente de Projetos.

As requisições de mudança devem ocorrer da seguinte forma:

1. Pedido Formal de Mudança: O solicitante preenche o Pedido Formal de Mudança, e envia para a Comissão de Controle de Mudança.

2. A CCM com apoio da Equipe Técnica realiza a triagem definindo a relevância e possível impacto da mudança: Com Impacto Significativo, Sem Impacto Significativo e Mudança Irrelevante - Rejeitada.

3. As mudanças que foram classificadas como Relevante devem gerar a Solicitação de Análise Detalhada de Impacto.

4. Realizar Análise de Impacto: Estudo e análise de quais itens de configuração a mudança impactará. Relatório contendo a lista de itens de configuração e qual o impacto sofrido pelo mesmo.

5. O CCM juntamente com o cliente negocia e aprova se a mudança pode ser implementada. O resultado deste processo pode gerar as seguintes decisões: Mudança Aprovada ou Mudança Reprovada.

6. Se a mudança for Aprovada, então é gerado um relatório contendo a lista das alterações que serão implementadas. Se não for aprovada, a CCM envia ao solicitante o resultado “reprovada” ou considerada irrelevante.




4. Padrões e Procedimentos
==========================

O Processo de liberação de versão para homologação se inicia com a revisão técnica do líder de desenvolvimento e em seguida com a liberação para a infra-estrutura.



5. Treinamento e Recursos
=========================
Descrição dos treinamentos efetuados para os integrantes do Grupo.

| Treinamento     | Objetivo                                                                                                                                                                                                      | Público Alvo      |
| --------------- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------| :-----------------|
| Repositório     | Treinamento ensina como acessar o repositório através de uma máquina cliente, como dar os comandos principais do repositório,  como incluir novos itens dentro do repositório e também como remover do mesmo. | Toda a equipe     |
| Ferramenta JIRA | Capacitar a equipe no tratamento das issues (tasks, bug, improvment entre outros e divulgar o workflow que será utilizado no projeto.																																					| Toda a equipe     |


6. Auditorias de Configuração
=============================
A auditoria da configuração deve ser conduzida para verificar se um item de configuração está em conformidade com um padrão ou requisito especificado. 

A auditoria de configuração deve ser executada antes que uma baseline seja definida, para certificar que o produto está de acordo com os requisitos (de especificação e contratuais) e também para garantir que está precisamente descrito em seus documentos técnicos.

Toda alteração também precisa ser auditada para garantir a integridade do produto que está sendo produzido.

São exemplos de itens de configuração sob gerência de configuração que o sistema deve incluir:

* Documentos gerenciais; 
* Requisitos, especificações;
* Códigos fonte;
* Arquivos de configuração;
* Executáveis;

Havendo necessidade de gerência de outros itens não listados acima, os itens faltantes devem ser definidos pelo Gerente de Configuração e inseridos no repositório do sistema.
