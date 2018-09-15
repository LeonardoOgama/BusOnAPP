# BusOnAPP

Projeto Multidisciplinar Integrador.

FACULDADE CESUSC
CURSO DE GRADUAÇÃO EM ANÁLISE E DESENVOLVIMENTO
DE SISTEMAS


SISTEMA DE RASTREAMENTO EM TEMPO REAL DOS VEÍCULOS UTILIZADOS NO SISTEMA DE TRANSPORTE COLETIVO DA CIDADE DE FLORIANÓPOLIS


PROJETO MULTIDISCPLINAR INTEGRADOR IV


LEONARDO LUIS OGAMA
TOMAZ SIELSKI ROSA


SISTEMA DE RASTREAMENTO EM TEMPO REAL DOS VEÍCULOS UTILIZADOS NO SISTEMA DE TRANSPORTE COLETIVO DA CIDADE DE FLORIANÓPOLIS


Projeto Multidisciplinar Integrador apresentado à Disciplina de Projeto Multidisciplinar Integrador I do Curso de Graduação em Análise e Desenvolvimento de Sistemas da Faculdade CESUSC, exigido como requisito parcial à aprovação na disciplina de Projeto Multidisciplinar Integrador I.


1.	INTRODUÇÃO

A ideia aqui apresentada é uma solução para dispositivos Android, com o intuito de realizar o rastreamento em tempo real dos veículos utilizados no serviço de transporte coletivo da cidade de Florianópolis. Os dados de localização virão dos módulos de GPS dos smartphones e tablets dos usuários do aplicativo. Uma vez que o usuário entrar em um veículo do transporte público, ele poderá utilizar o aplicativo para providenciar ao sistema informações como o nome da linha, selecionando-o de uma lista, e autorizar a utilização dos dados de GPS, para que possa ser monitorada a rota e o posicionamento do veículo, e ainda relatar informações como lentidão causada por trânsito, acidente, entre outros fatores. 
Por outro lado, um usuário que queira utilizar o aplicativo para obter essas informações, poderá visualizar num mapa as localizações em tempo real dos veículos, bem como filtrar a visualização para linhas específicas. Caso os usuários não desejem fornecer tais informações para o aplicativo, este estará perdendo sua funcionalidade, pois ele operará através de um método colaborativo, onde os dados essenciais para seu funcionamento serão fornecidos de e para os usuários, e quanto maior for a gama de usuários, mais rico e confiável ficará o aplicativo, pois este poderá providenciar um maior número de informações sobre rotas e localizações, cobrindo cada vez mais linhas, solucionando conflitos causados por variações nos horários, auxiliando seus utilizadores.

1.1.	 IDENTIFICAÇÃO DO PROJETO

O grande avanço das tecnologias de computação móvel tem mostrado o quão importante ela se tornou para o cotidiano das pessoas. Em meados de 2015, o número de brasileiros utilizando smartphones já ultrapassava a casa dos 76 milhões, e quase 92% desses aparelhos executavam o Sistema Operacional Android. Em uma área bem distante da tecnologia, porém tão presente nas nossas vidas quanto os dispositivos móveis, está o transporte coletivo, que em Florianópolis, já contava com mais de 250 mil usuários por dia em 2012, número que vem crescendo a cada ano.
Ao utilizar o serviço, observou-se variações nos horários de passagem previstos para os veículos, causadas por mudanças climáticas, grande volume de automóveis nas estradas, concentrações de usuários nos pontos de parada, entre outros fatores. Sejam essas variações de horários, causadoras de adiantamentos ou atrasos na chegada dos ônibus, pôde-se perceber que a criação de um sistema que previsse tais variações, seria de grande ajuda para os usuários do sistema de transporte coletivo da cidade de Florianópolis, evitando eventuais transtornos. 

2. ANÁLISE DE VIABILIDADES
2.1. VIABILIDADE TÉCNICA

Segundo Dennis e Wixon (2005), a primeira técnica na análise de viabilidade é avaliar a viabilidade técnica do projeto, até onde o sistema pode ser projetado, desenvolvido e instalado com sucesso pela equipe de T.I. 
Até a presente data, ambos os autores deste projeto não possuem conhecimento aprofundado em linguagem de programação "Android", o qual será adquirido ao longo do desenvolvimento. Se trata de um projeto complexo, porém com objetivos e funcionalidades bem definidos, facilitando seu desenvolvimento. 
Tabela 1 - Análise de Viabilidade Técnica
Item analisado	Resposta dos Gerentes de TI responsáveis
Familiaridade com a aplicação	Alta
Familiaridade com a tecnologia	Baixa
Complexidade do projeto	Alta
Compatibilidade	Alta

Para o aplicativo funcionar de forma correta, este deverá ser instalado num dispositivo Android que possua módulo GPS e conexão ativa com a internet. O propósito do aplicativo engloba sua utilização durante os trajetos do transporte coletivo, logo isso acarreta na necessidade de um plano de dados móveis. Uma pesquisa realizada no Terminal de Integração do Centro (TICEN) em Florianópolis, mostrou que 92% dos respondentes utilizam seus smartphones durante os trajetos no serviço de transporte coletivo, e destes, 93% possuem internet móvel. 
Posteriormente foi realizada uma nova pesquisa, afim de obter dados sobre o sistema operacional dos smartphones dos usuários, apontando que 75% dos dispositivos operam o Sistema Operacional “Android”, sendo 74% destes, a versão 6.0 “Marshmallow”. Assim foi definido o nível de API (Application Programming Interface) em que será baseado o aplicativo, ou seja, apenas aparelhos executando a versão do Android 6.0 ou superior irão suportar o aplicativo, pois apesar de restringir o número de dispositivos, quanto maior o nível de API, maior é a gama de funcionalidades que podem ser implementadas, e melhor é a otimização do aplicativo, utilizando menos memória e dados. 
Até a presente etapa do projeto, não há a intenção de tornar o aplicativo compatível com dispositivos iOS pelo fato do desenvolvimento para esta plataforma apenas ser possível através das ferramentas Swift e X-Code, exigindo um dispositivo com o Sistema Operacional MacOS, além da Liçensa de Desenvolvedor Apple, cuja taxa anual pode chegar a U$299 (dólares) (vide item 2.3. Viabilidade Econômica).

2.2. VIABILIDADE ORGANIZACIONAL

A termos de aceitação do projeto, através de pesquisas com usuários do sistema de transporte coletivo, foi obtido um total de 354 respondentes, onde 70% definiram como 9 ou 10 numa escala de 0 a 10, seu interesse em utilizar um aplicativo que providenciasse em tempo real a localização dos veículos utilizados no transporte coletivo, através de um método colaborativo.
Através da aplicação da pesquisa, e da própria utilização do transporte coletivo, pôde-se constatar que o aplicativo aqui proposto será de grande ajuda para os usuários de ônibus da cidade, pois como foi citado na identificação do projeto, haverá um melhor aproveitamento do tempo, uma vez que imprevistos nos horários de partida e chegada dos veículos poderão ser previstos.

2.3. VIABILIDADE ECONÔMICA

Os autores do projeto desenvolverão o aplicativo, logo não haverá custos para este fim. Porém, para seu pleno funcionamento, há a necessidade de que uma parte da aplicação seja hospedada num servidor, reunindo as informações referente a rotas, disponibilizando-as no mapa do aplicativo. Há outros custos, pois publicar o aplicativo na "Play Store", loja de aplicativos do Sistema Operacional Android, exige uma Licença de Desenvolvedor Android, com uma taxa única de abertura de conta, de U$ 25 (dólares), traduzindo-se em aproximadamente R$ 82 (reais), uma vez aplicada a cotação de 3.27 (vigente em 07/06/2017). Não há necessidade de renovação, e o tempo médio necessário para a publicação do aplicativo na loja é de 24 horas. A termos de comparação, a publicação na loja de aplicativos do Sistema Operacional iOS (“App Store”) leva em torno de 15 dias, e para isto, é necessária a Licença de Desenvolvedor Apple, com três modalidades. A “Individual”, para desenvolvedores ou pessoas físicas, aplicando-se uma taxa de U$99 por ano, “Organization”, para empresas, ocorrendo de forma um pouco mais burocrática, porém com o mesmo valor do plano “Individual”, e o “Enterprise Program”, que se difere do “Organization” por permitir também o desenvolvimento de aplicativos de uso interno, sem a publicação na App Store, por U$299 ao ano.

3. TÍTULO E DESCRIÇÃO DO PROJETO

Sistema de Rastreamento em Tempo Real dos Veículos Utilizados no Serviço de Transporte Coletivo da Cidade de Florianópolis.

O projeto consiste em um aplicativo para a plataforma “Android”, cujo propósito é realizar o rastreamento em tempo real dos veículos utilizados no serviço de transporte coletivo da cidade de Florianópolis, através do módulo GPS dos smartphones e tablets dos usuários. O aplicativo dependerá de seus utilizadores, pois para um usuário usufruir de todas as suas funcionalidades, este deverá contar com a ajuda de outros usuários, que fornecerão informações para o aplicativo, como por exemplo, qual ônibus estão utilizando, onde e quando entraram no veículo, além da permissão do uso dos dados de GPS do dispositivo, para que o sistema possa reunir essas informações, gerando trajetórias dos veículos em tempo real.

4. GERENTE DE PROJETO DESIGNADO E NÍVEL DE AUTORIDADE

Gerente do Projeto (GP) designado: Tomaz Sielski Rosa 
O nível de autoridade do Gerente do Projeto, Tomaz, será total. Alguns funcionários específicos deverão deixar temporariamente suas atividades funcionais do aplicativo, para dedicar-se ao projeto do aplicativo e informar ao GP todas as informações coletadas do aplicativo pessoalmente. Caso isso não seja possível, será necessário o envio de um e-mail para o GP contendo essas devidas informações.

5. RECURSOS PRÉ-DESIGNADOS

Gerente do Projeto: Tomaz Sielski Rosa.
Owner (s): Leonardo Luis Ogama e Tomaz Sielski Rosa.
Key-User (s): Equipe de Projeto, usuários do transporte coletivo.

6. PARTES INTERESSADAS

As partes interessadas nesse projeto:
•	Prefeitura Municipal de Florianópolis;
•	Consórcio Fênix; 
•	Sistema Integrado de Mobilidade (S.I.M).

7. REQUISITOS 
7.1. REQUISITOS CONHECIDOS DAS PARTES INTERESSADAS

Como já foi citado antes, o aplicativo propõe a interatividade e colaboração de pessoas para pessoas, afim de fazê-las compartilhar dados, visando disponibilizar informações interessantes a todos os usuários do transporte coletivo, tornando a sua utilização mais rica, sabendo-se com precisão os horários de chegada e saída dos veículos, bem como sua situação em tempo real.

7.2. REQUISITOS PARA APROVAÇÃO DO PROJETO

•	Resultados satisfatórios em uma pesquisa de aceitação estruturada; 
•	Orçamento bem estabelecido e dentro das condições financeiras cabíveis.

8. PREMISSAS

•	Apoio da Prefeitura Municipal de Florianópolis;
•	Adesão dos usuários do sistema de transporte coletivo;
•	Apoio da empresa Consórcio Fênix;
•	Cooperação dos utilizadores do serviço.



9. RESTRIÇÕES

•	Usuários que utilizem seu smartphone durante a utilização do sistema de transporte coletivo;
•	Usuários que possuam planos de internet móvel;
•	Esta solução só atenderá, a princípio, a região da Grande Florianópolis;

10. OBJETIVOS MENSURÁVEIS

Desenvolver um aplicativo mobile que auxilie os usuários do sistema de transporte coletivo na cidade de Florianópolis, provendo informações sobre localização e horários em tempo real a respeito das linhas em operação, solucionando problemas causados por variações nos horários de saída e chegada dos veículos.

Tabela 2 – Carga Horaria
Cargo	Carga Horaria	Valor Hora	Subtotal
Gerente	2880 Horas	R$ 80,00	R$ 230.400,00
Desenvolvedor de Interface	1440 Horas	R$ 80,00	R$ 115.200,00
Desenvolvedor de BD	768 Horas	R$ 40,00	R$ 30.720,00
Testador 	300 Horas	R$ 40,00	R$ 12.000,00
Total	----------------------	----------------------	R$ 388.320,00
(BD: Banco de dados)

11. RISCOS DE NÍVEL MACRO PARA O PROJETO

•	Baixa adesão de usuários;
•	Usuários sem um plano de internet móvel; 
•	Perda das características do software, sendo utilizado de maneira errônea, e provendo informações incivis aos usuários.

12. PATROCINADORES ALMEJÁVEIS

•	Prefeitura de Florianópolis;
•	Consórcio Fênix;
•	Sistema Integrado de Mobilidade (S.I.M.).


13. ENTREGAS E DESCRIÇÃO DO PRODUTO

Para a entrega do projeto, visa-se desenvolver uma aplicação móvel, funcional em dispositivos que rodem o Sistema Operacional “Android” e possuam módulo GPS, capaz de auxiliar na utilização do sistema de transporte coletivo na cidade de Florianópolis, provendo informações de localização dos veículos em tempo real, através de um método colaborativo.
A entrega do projeto se dará em duas partes, sendo a primeira parte da entrega um protótipo do aplicativo para a realização de testes, estimada para dia 15 de junho de 2018. A segunda parte, sendo a versão final do projeto, tem a previsão de ser entregue até o final de novembro de 2018.
Após a entrega final do projeto, haverá atualizações no sistema, para ajustes de compatibilidade com outras versões do sistema operacional “Android” e futuras análises econômicas, para estudar a implementação da aplicação em outras plataformas mobile como o “iOS” e o “Windows Phone”, executados nos “iPhone”, e “Microsoft/Nokia Lumia” respectivamente, além da correção de eventuais bugs (erros) presentes no aplicativo.

