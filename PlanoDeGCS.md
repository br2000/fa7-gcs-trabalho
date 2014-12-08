<Nome do Projeto>
=================
Plano de Gerenciamento de Configuração
======================================
Versão &lt;1.0&gt;
------------------

_[Observação: O template a seguir é fornecido para uso com o Rational Unified Process (RUP).  O texto exibido entre colchetes e em itálico foi incluído para orientar o autor e deve ser excluído antes da publicação do documento._

_Este documento utiliza a formatação da linguagem [Markdown] (http://daringfireball.net/projects/markdown/). Você pode encontrar um guia de referência rápido [aqui] (https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet).]_

Histórico de Versões
--------------------

|Data                |Versão       |Descrição               |Autor          |
|--------------------|-------------|------------------------|---------------|
|_&lt;05/12/2104&gt;_|_&lt;1.0&gt;_|_&lt;Versão inicial&gt;_|_&lt;Bruno Camargo&gt;_|
|_&lt;07/12/2014&gt;_|_&lt;1.1&gt;_|_&lt;Outra versão&gt;_  |_&lt;Felipe Andrade&gt;_|
|_&lt;07/12/2014&gt;_|_&lt;1.2&gt;_|_&lt;Outra versão&gt;_  |_&lt;Carlos Bezerra&gt;_|



1. Introdução
==============

_[A introdução do Plano de Gerenciamento de Configuração  oferece uma visão geral de todo o documento. 
Ela inclui a finalidade, o escopo, as definições, os acrônimos, as abreviações, as referências e uma visão geral deste
Plano de Gerenciamento de Configuração.]_

O Plano de Gerenciamento de Configuração tem como objetivo principal documentar o sistema de gestão de configuração definido para o Projeto XYZ, apresentando todas as tarefas, os seu padrões, procedimentos, atividades e responsáveis. Portanto, podemos afirmar que a aplicação deste plano visa garantir a integridade de códigos-fonte e demais produtos do sistema XYZ, permitindo acompanhamento destes itens durante todo o ciclo de vida do projeto, preservando o histórico de evolução dos sistemas da instituição.

1.1 Finalidade
---------------
_[Especifique a finalidade deste Plano de Gerenciamento de Configuração.]_

Este Plano de Gerenciamento de Configuração destina-se a todos os projetos iniciados no ambiente de desenvolvimento da empresa XYZ e tem como obejtivo principal descrever a organização, nomeclatura e regras para versionamento do projeto XYZ. Portanto, o plano auxiliará os profissionais de desenvolvimento e produção a gerenciar o estado dos itens de configuração, controlar  as mudanças em itens de configuração e principalmente rastrear tais modificações ao longo do ciclo de vida do projeto.

1.2 Escopo
----------
_[Uma breve descrição do escopo deste Plano de Gerenciamento de Configuração; o modelo ao qual ele está associado e tudo o que é afetado ou influenciado por este documento.]_

Este plano é destinado a todos os profissionais responsáveis pelo desenvolvimento do sistema XYZ, e deverá ser seguido durante todo o ciclo de vida do produto. O referido plano abrangerá todos os dados relevantes definidos nos projetos relacionados ao sistema XYZ, incluindo ferramentes, hardware, responsabilidades, cronogramas, e dará subsídios a equipe para controlar as etapas de desenvolvimento do software XYZ.

1.3 Definições, Acrônimos e Abreviações
---------------------------------------
_[Esta subseção apresenta as definições de todos os termos, acrônimos e abreviações necessários para a correta interpretação do Plano de Gerenciamento de Configuração.  Essas informações podem ser fornecidas mediante referência ao Glossário do projeto.]_

|Sigla	 |Descrição                                                                             |
|--------|----------------------------------------------------------------------------------------|                                                                                                                            
|BASELINE|Conjunto de itens de configuração que conseguiram um estado comprovado de estabilidade. |
|CCM	 |Comitê para o Controle de Mudanças.  |
|CM | Controle de Mudanças |
|GC	 |Gerência de Configuração |
|PGC | Plano de Gerenciamento de Configuração | 
|RUP	 |Rational Unified Process |   
|SM	 |Solicitação de mudança                                                                 
|XYZ    |Sistema... |




1.4 Referências
---------------
_[Esta subseção apresenta uma lista completa de todos os documentos mencionados no Plano de Gerenciamento de Configuração. Identifique os documentos por título, número de relatório (se aplicável), data e organização responsável pela publicação. Especifique as fontes a partir das quais as referências podem ser obtidas. Essas informações podem ser fornecidas por um anexo ou outro documento.]_

1.5 Visão Geral
---------------
_[Esta subseção descreve o conteúdo restante do Plano de Gerenciamento de Configuração e explica como o documento está organizado.]_



2. Gerenciamento de Configuração de Software
============================================

2.1 Organização, Responsabilidades e Interfaces
------------------------------------------------
_[Descreva quem será o responsável pela execução das diversas atividades de Gerenciamento de Configuração (CM) descritas no Processo de CM.]_

|Papéis | Equipe | Responsabilidade |                                                             
|-----------------------------------|----------------------------------------------------------------------------------------|                                                                                                                            
|Gerente de Configuração |Carlos Bezerra |Estabelecer Políticas de GC, Escrever Plano de GC, Configurar Ambiente de GC, Criar Espaços de Trabalho de Integração, Criar Baselines e Promover Baselines|
|CCM | Bruno Camargo e Carlos Bezerra | Estabelecer Processo de Controle de Mudanças e Revisar Solicitação de Mudança |
|Desenvolvedor | Carlos Bezerra e Felipe Andrade | Seguir os padrões e procedimentos definidos no Plano de Gerência e Configuração |
|Todos os Papéis | Bruno Camargo, Carlos Bezerra e Felipe Andrade | Enviar Solicitação de Mudança e Atualizar Solicitação de Mudança |

2.2 Ferramentas, Ambiente e Infra-estrutura
-------------------------------------------
_[Descreva o ambiente de computação e as ferramentas de software a serem utilizadas para desempenhar as funções de CM em todo o ciclo de vida do projeto ou produto._
_Descreva as ferramentas e os procedimentos necessários utilizados para o controle de versão dos itens de configuração gerados no ciclo de vida do projeto ou produto._
_As questões envolvidas na configuração do ambiente de CM incluem:_
* _tamanho previsto dos dados do produto_
* _distribuição da equipe do produto_
* _localização física dos servidores e clientes]_
 
### 2.2.1 Ferramentas a serem utilizadas para a Gerência de Configuração
----------------------------------

|Ferramenta | Tipo | Descrição | Versão |                                                            
|-----------------------------------|----------------------------------------------------------------------------------------|                                                                                                                            
|IDE Eclipse | Plataforma de Desenvolvimento | É uma IDE para desenvolvimento Java, com suporte a diversas linguagens e plugins. | Eclipse Luna 4.4.1 |
|Git | Controle de Versão |Sistems para Controle de Verão |1.9.4 |
|Egit Plugin | Acesso ao Repositório | Cliente para o Git Integrado ao Windows | 1.4.8.121 |

### 2.2.2 Ferramentas do ambiente de desenvolvimento
----------------------------------

|Tipo | Ferramenta | Versão |                                                            
|-----------------------------------|----------------------------------------------------------------------------------------|                                                                                                                            
|Sistema Operacional | Windows 7 Professional | SP1 |
|Cronograma | Microsoft Office Project | 2013 |
|Planilha | Microsoft Office Excel | 2010 |
|Editor de Texto | Microsoft Office Word | 2010 |
|Controle de Versão | Git | 1.9.4 |
|Plataforma de Desenvolvimento | Eclipse Luna | 4.4.1 |
|Planilha | Microsoft Office Excel | 2010 |
|Banco de Dados | MySQL | 5.0 |
|Comunicação | E-mail / Skype / Whatsapp |  |


### 2.2.3 Estrutura do Ambiente
----------------------------------

|Ambiente | Descrição | Transição |                                                            
|-----------------------------------|----------------------------------------------------------------------------------------|                                                                                                                            
|Desenvolvimento | É o ambiente que será utilizado para a codificação do sistema. | O componente atingirá a maturidade quando os requisitos forem supridos e testados pelos desenvolvedores através dos testes unitários. |
|Integração | É o ambiente que servirá para os testes de integração | Quando a comunicação entre os módulos atinge um estágio aceitável de funcionamento. |
|Banco de Dados | É o ambiente onde os dados serão armazenados | Ambiente que conterá o banco de dados do sistema. |

### 2.2.4 Estrutura dos Equipamentos
----------------------------------

|QTD | Ambientes | Configuração de Hardware |  Configuração do Software                                                          
|-----------------------------------|----------------------------------------------------------------------------------------|                                                                                                                            
|3 | Desenvolvedor | Processador 2.3GHz, Memória de 4GB ou Superior, Disco Rígido de 500GB ou Superior e IP 192.168.0.50 ~ 52| Windows 7 Professional SP1, Eclipse Luna 4.4.1, Git 1.9.4, Egit 1.4.8.121, Office 2010, Mysql 5.0 e Skype |
|1 | Integração | Processador 3.0GHz, Memória de 16GB ou Superior, Disco Rígido de 2TB ou Superior e IP 192.168.0.10 | Centos 6.5 64 bits, Java 1.8 SDK, Git 1.9.4, Maven Plugin 2.8, MySQL Database Plugin 1.0 e Jenkins 1.588 |
|1 | Banco de Dados | Processador 2.3 GHz ou Superior, Memória de 8GB ou Superior, Disco Rígido de 1TB ou Superior e IP 192.168.0.20 | Centos 6.5 64 bits e MySQL 5.0 |

3. O Programa de Gerenciamento de Configuração
==============================================

3.1 Identificação da Configuração
---------------------------------
### 3.1.1 Métodos de Identificação
----------------------------------
_[Descreva como os artefatos do projeto ou produto devem ser nomeados, marcados e numerados. O esquema de identificação deve abranger o hardware, o software do sistema, os produtos de terceiros (COTS) e todos os artefatos de desenvolvimento de aplicativos listados na estrutura de diretórios do produto; por exemplo, planos, modelos, componentes, software de teste, resultados e dados, executáveis e assim por diante.]_

### 3.1.2 Itens de Configuração
_[Relacionar os artefatos ou grupos de artefatos, separando por tipo, modulo ou subsistema, responsável ou momento em que deverão ser incluídos em baselines._
* _“Inclusão em Baseline” em branco significa que o grupo de artefatos não participará de baseline. Pode ser expresso como uma data ou identificador de uma baseline, fase ou ponto de controle_
* _“Responsável”: indicar nominalmente, sempre que possível]_

| Item (ou Tipo de Item)                 | Responsável na equipe	     | Inclusão em Baseline |
|----------------------------------------|-----------------------------|----------------------|
|_&lt;grupo de itens de configuração&gt;_|_&lt;nome do responsável&gt;_|_&lt;momento a partir do qual o conjunto de artefatos será incluído em baseline&gt;_|


### 3.1.3 Baselines do Projeto

_[As baselines funcionam como um padrão oficial no qual os trabalhos subseqüentes são baseados. Somente mudanças autorizadas podem ser efetuadas nas baselines._
_Descreva em que pontos do ciclo de vida do projeto ou produto as baselines devem ser estabelecidas. As baselines mais comuns devem ser definidas ao final de cada uma das fases de Iniciação, Elaboração, Construção e Transição. Elas também podem ser geradas no final de iterações ocorridas dentro das várias fases ou com freqüência ainda maior._
_Descreva quem autoriza uma baseline e o que ela contém.]_

### 3.1.4 Estrutura do Repositório de Versões
_[Descreva a organização de diretórios do seu repositório e que itens/arquivos devem ser armazenados em cada diretório.]_

3.2 Controle de Configuração e Mudança
--------------------------------------

### 3.2.1 Processamento e Aprovação de Solicitações de Mudança

As solicitações de mudanças das Baselines serão realizadas através da ferramenta Jira.

**Status das Issues**

| Atividade                        			 | Descrição	     											   				| Responsabilidade      |
|----------------------------------------|------------------------------------------------|-----------------------|
|Aberto																	 | Criação da solicitação.												| Todos									|
|Em Analise															 | Análise da solicitação													| Analista de sistemas	|
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

3. As mudanças que foram classificadas como Relevante deve gerar a Solicitação de Análise Detalhada de Impacto.

4. Realizar Análise de Impacto: Estudo e análise de quais itens de configuração a mudança impactará. Relatório contendo a lista de itens de configuração e o qual impacto sofrido pelo mesmo.

5. O CCM juntamente com o cliente negocia e aprova se a mudança pode ser implementada. O resultado deste processo pode gerar as seguintes decisões: Mudança Aprovada ou Mudança Reprovada.

6. Se a mudança for Aprovada, então é gerado um relatório contendo a lista das alterações que serão implementadas. Se não for aprovada, a CCM envia ao solicitante o resultado “reprovada” ou considerada irrelevante.




4. Padrões e Procedimentos
==========================
_[Descreva os padrões e procedimentos que devem ser seguidos no projeto. Crie subseções se achar necessário, para organizá-los melhor.]_



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
