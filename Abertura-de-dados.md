Processo de abertura de dados
====

Este é o processo que será executado em cada projeto de abertura de dados
(por exemplo, o projeto da abertura de uma base de dados de um sistema de
informação de uma área de negócio específica). A depender da capacidade
da instituição, poderá ser executada uma ou mais instâncias desse processo
simultaneamente em um dado momento.

[<img alt="Diagrama do processo de abertura de um conjunto de dados" src="https://raw.githubusercontent.com/dadosgovbr/kit/master/public/img/Processo%20Publica%C3%A7%C3%A3o%20Dados%20Abertos.png">](https://raw.githubusercontent.com/dadosgovbr/kit/master/public/img/Processo%20Publica%C3%A7%C3%A3o%20Dados%20Abertos%20-%20com%20titulo.png)

(árvore de decisões)

## Documento Plano de Dados Abertos

O Plano de Dados Abertos da instituição norteará o processo de abertura de
dados quanto ao escopo, prazo, partes interessadas, etc.

*Insumo para:* Solicitar documentação

## Solicitar documentação

Solicitar esquema e documentação da base de dados. Ex.: modelos UML ou
entidade-relacionamento, dicionário de dados, etc.

*Próximo passo:* Definir estrutura dos dados

## Definir estrutura dos dados

Definir campos e estrutura dos dados. XML, CSV e JSON são úteis para situações
específicas.

*Próximo passo:* Decidir qualidade mínima

## Decidir qualidade mínima

Definir por acordo entre as partes interessadas a qualidade mínima dos dados
abertos publicados, de forma a viabilizar a sua publicação tempestiva dentro
da capacidade da instituição.

*Próximo passo:* Realizar extração

## Realizar extração

Realizar extração dos dados, a partir do ambiente de produção da base de dados,
para o local onde a base será disponibilizada como dados abertos.

Por exemplo, se tiver sido decidido publicar os dados em arquivos csv, essa
etapa contempla hospedar a extração em csv em um servidor de arquivos para a
web. Se tiver sido decidido publicar uma API de dados abertos, essa etapa
contempla a carga da base de dados que é acessada diretamente pela camada de
aplicação da API.

*Próximo passo:* Atualização automática

## Atualização automática

Definir e implementar processo automático de atualização dos dados. Inclui a
negociação da periodicidade e forma de acesso aos dados, bem como a criação de
scripts de transformação carga (ETL).

*Próximo passo:* Publicar na web

## Publicar na web

Publicar os dados na web. Inclui homologar a forma como os dados são
apresentados e disponibilizar o acesso ao público externo.

*Próximo passo:* Catalogar no dados.gov.br

## Catalogar no dados.gov.br

Catalogar o novo conjunto de dados no Portal Brasileiro de Dados Abertos.

