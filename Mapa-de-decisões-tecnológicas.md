---
published: true
permalink: /Mapa-de-decisões-tecnológicas/
layout: slate
filename: Mapa-de-decisões-tecnológicas.md
title: Mapa de decisões - Kit de Dados Abertos
desc: Neste mapa são apresentadas diversas formas de publicação de dados abertos, dando ao gestor parâmetros de apoio à decisão.
---

## Mapa de decisões tecnológicas

A tabela abaixo mostra as soluções mais comuns para publicar dados abertos, ordenadas por complexidade e prazo de implementação.

<!---
Abaixo o código HTML da tabela, markdown não suporta colspan.
--->

<table class="tabela-decisoes-tecnologicas">
    <!--<colgroup>
      <col width="118" />
      <col width="424" />
      <col width="302" />
      <col width="200" />
    </colgroup>-->

    <tr>

      <th>
        Solu&ccedil;&atilde;o
      </th>

      <th>
        Pr&eacute;-requisitos
      </th>

      <th>
        Prazo
      </th>

    </tr>

    <tr>

      <td rowspan="2">
        <a href="#publicar-dump-da-base-de-dados">Publicar dump da base de dados</a>
      </td>

      <td class="celula-meio">
        Acesso &agrave; base de dados
      </td>

      <td rowspan="2">
        Curto<br />
      </td>

    </tr>

    <tr>
      <td>
        Servidor web para arquivos
      </td>

    </tr>

    <tr>

      <td rowspan="2">
        <a href="#publicar-dados-em-arquivos-csv">Publicar dados em arquivos CSV</a>
      </td>

      <td class="celula-meio">
        Mecanismo de ETL (caso esteja em banco relacional)
      </td>

      <td rowspan="2">
        Curto<br />
      </td>

    </tr>

    <tr>
      <td>
        Servidor web para arquivos
      </td>

    </tr>

    <tr>

      <td rowspan="3">
        <a href="#publicar-dados-em-arquivos-json--xml">Publicar dados em arquivos JSON / XML</a>
      </td>

      <td class="celula-meio">
        Mecanismo de ETL (caso esteja em banco relacional)
      </td>

      <td rowspan="3">
        M&eacute;dio
      </td>

    </tr>

    <tr>
      <td class="celula-meio">
        Servi&ccedil;o de desenvolvimento
      </td>

    </tr>

    <tr>
      <td>
        Servidor web para arquivos
      </td>

    </tr>

    <tr>

      <td rowspan="2">
        <a href="#desenvolver-mdulo-de-dados-abertos-em-sistema-existente">Desenvolver m&oacute;dulo de dados abertos em sistema existente</a>
      </td>

      <td class="celula-meio">
        Servi&ccedil;o de desenvolvimento
      </td>

      <td rowspan="2">
        Longo
      </td>

    </tr>

    <tr>
      <td>
        Servidor web para deploy da nova solu&ccedil;&atilde;o
      </td>

    </tr>

    <tr>

      <td rowspan="3">
        <a href="#desenvolver-api-restful-de-dados-abertos-desacoplada-da-soluo">Desenvolver API RESTful de dados abertos desacoplada da
        solu&ccedil;&atilde;o</a>
      </td>

      <td class="celula-meio">
        Mecanismo de ETL
      </td>

      <td rowspan="3">
        Longo
      </td>

    </tr>

    <tr>
      <td class="celula-meio">
        Servi&ccedil;o de desenvolvimento
      </td>

    </tr>

    <tr>
      <td>
        Servidor web para deploy da nova solu&ccedil;&atilde;o
      </td>

    </tr>

    <tr>

      <td rowspan="3">
        <a href="#novo-sistema-com-a-gesto-de-dados-incorporados-em-sua-arquitetura">Novo Sistema, com a gest&atilde;o de dados incorporados em sua arquitetura</a>
      </td>

      <td class="celula-meio">
        Mecanismo de ETL
      </td>

      <td rowspan="3">
        Longo
      </td>

    </tr>

    <tr>
      <td class="celula-meio">
        Servi&ccedil;o de desenvolvimento
      </td>

    </tr>

    <tr>
      <td>
        Servidor web para deploy da nova solu&ccedil;&atilde;o
      </td>

    </tr>

    <tr>

      <td rowspan="3">
        <a href="#publicar-dados-em-arquivos-rdf">Publicar dados em arquivos RDF</a>
      </td>

      <td class="celula-meio">
        Ontologia da &aacute;rea do conhecimento do sistema
      </td>

      <td rowspan="3">
        Longo
      </td>

    </tr>

    <tr>
      <td class="celula-meio">
        Mecanismo de ETL
      </td>

    </tr>

    <tr>
      <td>
        Servidor web para arquivos
      </td>

    </tr>

    <tr>

      <td rowspan="3">
        <a href="#disponibilizar-dados-por-endpoint-sparql">Disponibilizar dados por Endpoint SPARQL</a>
      </td>

      <td class="celula-meio">
        Ontologia da &aacute;rea do conhecimento do sistema
      </td>

      <td rowspan="3">
        Mais Longo
      </td>

    </tr>

    <tr>
      <td class="celula-meio">
        Mecanismo de ETL
      </td>

    </tr>

    <tr>
      <td>
        Banco de dados de triplas
      </td>

    </tr>

    <tr>

      <td rowspan="5">
        <a href="#publicar-dados-em-api-de-dados-ligados-linked-data">Publicar dados em API de dados ligados (Linked Data)</a>
      </td>

      <td class="celula-meio">
        Ontologia da &aacute;rea do conhecimento do sistema
      </td>

      <td rowspan="5">
        Mais Longo
      </td>

    </tr>

    <tr>
      <td class="celula-meio">
        Banco de dados de triplas
      </td>

    </tr>

    <tr>
      <td class="celula-meio">
        Servi&ccedil;o de desenvolvimento
      </td>

    </tr>

    <tr>
      <td class="celula-meio">
        Mecanismo de ETL
      </td>

    </tr>

    <tr>
      <td>
        Servidor web para deploy da nova solu&ccedil;&atilde;o
      </td>

    </tr>
  </table>

### Lista de Soluções

#### Publicar dump da base de dados

Essa é a forma mais simples de publicação, caso a base de dados não esteja em ambiente próprio, basta pedir extração ao prestador de serviços, disponibilizar no servidor web e providenciar domínio + URL persistente.

**Vantagens e Desvantagens:** curto prazo de implementação, difícil visualização dos dados.

#### Publicar dados em arquivos CSV

Para essa publicação é necessário um mecanismo mínimo de ETL, para poder transformar as tabelas do SGBD em 'tabelas' CSV.

**Vantagens e Desvantagens:** curto prazo, fácil visualização através de ferramentas conhecidas.

#### Publicar dados em arquivos JSON / XML

No caso do CSV bastaria transformar e normalizar uma tabela em outra tabela (SGBD -> SQL). Para essa publicação, será necessária uma transformação mais customizada, respeitando as estruturas dos formatos JSON e XML.

**Vantagens e Desvantagens:** mais trabalhoso de implementar, facilidade de se trabalhar com esses formatos nas linguagens de programação e apis de visualização.

#### Desenvolver módulo de dados abertos em sistema existente

Essa opção só é viável caso o sistema tenha uma arquitetura modular.

**Vantagens e Desvantagens:** coesão da solução; interface única para usuários; maior custo de desenvolvimento.

#### Desenvolver API RESTful de dados abertos desacoplada da solução

Uma decisão importante para essa opção é a separação ou não do banco de dados da API do de produção, que possui várias implicações (performance, atualidade dos dados etc)

**Vantagens e Desvantagens:** possibilidade de consultas mais específicas; Custo de desenvolvimento.

#### Novo Sistema, com a gestão de dados incorporados em sua arquitetura

**Vantagens e Desvantagens:** Sistema desenhado prevendo atendimento da Lei de Acesso à informação, automatização da extração de dados

#### Publicar dados em arquivos RDF


#### Disponibilizar dados por Endpoint SPARQL


#### Publicar dados em API de dados ligados (Linked Data)


### Glossário de Formatos

#### Formatos básicos

##### Dump SQL

`++++++`: 
* Forma menos trabalhosa de se publicar os dados
* Curto prazo para produção
* Preserva a estrutura dos dados como o são em produção

`------`:
* Provável necessidade de remoção prévia de dados pessoais
* Necessidade de realizar carga dos dados em SGBD para acessá-los
* Despadronização entre dumps de SGBSs diferentes: necessita do mesmo software e versão que gerou o dump

##### CSV

Pode significar [Comma-Separated Values](https://pt.wikipedia.org/wiki/Comma-separated_values)
(valores separados por vírgula), ou
ainda, Character-Separated Values (valores separados por caractere). É um
formato para armazenamento de dados tabulares em texto. A codificação é
muito simples: cada linha do arquivo representa uma linha na tabela, e as
colunas são separadas por vírgula. Campos que podem conter vírgula devem ser
delimitados por aspas. CSV é recomendado para representação de estrutura de
dados mais simples, de natureza tabular, onde não existem subpropriedades ou
listas, gerando um arquivo menor e mais leve para processamento. Arquivos CSV
são processáveis diretamente por editores de planilhas, como o OpenOffice e o
MS Excel. (do [Glossário](/Gloss%C3%A1rio/#csv))

`++++++`:
* Simplicidade. Registros em estrutura tabular.
* Facilidade de geração (qualquer banco de dados exporta)
* Facilidade de consumo (qualquer editor de planilhas manipula)
* Sucinto (os arquivos gerados são menores)

`------`:
* Falta de padronização do formato
* Não suporta tipagem de valores
* Dificuldade em se representar ligações entre os dados

##### JSON

É um acrônimo para
[_JavaScript Object Notation_](https://pt.wikipedia.org/wiki/JSON).
É um padrão aberto de estruturação de dados baseado em texto e legível por
humano. A especificação é a [RFC 7159](https://tools.ietf.org/html/rfc7159).
JSON ganhou maior utilização com a utilização de carga dinâmica de conteúdo
em páginas web com Javascript (técnica denominada "Ajax"). A serialização em
JSON é muito simples e resulta em uma
estrutura pouco verbosa o que se mostra uma ótima alternativa para o XML.
JSON possibilita serialização de estrutura de objetos complexos, como listas e
subpropriedades. JSON está se tornando o padrão mais utilizado para integração
de dados entre repositórios e frameworks, também está se tornando o padrão
nativo de armazenamento em alguns bancos de dados modernos.
(do [Glossário](/Gloss%C3%A1rio/#json))

`++++++`:
* Facilidade para representar hierarquias
* Suporta tipagem de valores
* Facilidade de consumo (qualquer linguagem de programação lê com facilidade)
* Utilizável diretamente em navegadores (leitura por javascript)
* Formato padronizado ([RFC 7159 do IETF](https://tools.ietf.org/html/rfc7159), [ECMA-404](http://www.ecma-international.org/publications/files/ECMA-ST/ECMA-404.pdf))
* Possibilidade de definir esquema de validação
* Mais leve para processar que o XML

`------`:

##### XML

XML significa Extensible Markup Language, e é uma sintaxe para codificar
documentos em um formato legível por máquina. É baseado em texto e tem como
principais objetivos [fontes?] simplicidade, extensibilidade e usabilidade.
XML é largamente utilizado como formato de troca de dados nos clássicos Web
Services SOAP. Apesar da larga utilização, é cada vez menos encorajada a
utilização desse formato para integração de aplicações. Em substituição,
recomenda-se utilizar JSON, por economizar banda e ser de processamento mais
leve. (do [Glossário](/Gloss%C3%A1rio/#xml)).

`++++++`:
* Facilidade para representar hierarquias
* Suporta tipagem de valores
* Amplo suporte de ferramentas
* Formato padronizado ([W3C](http://www.w3.org/TR/2006/REC-xml11-20060816/))
* Possilidade de definir esquema de validação

`------`:
* Prolixo (os arquivos gerados são maiores)
* Maior gasto de processamento para geração e consumo em relação ao JSON.

#### Foramtos geo

Alguns formatos de arquivo servem especificamente para representar dados
geográficos. A seguir, são relacionados os principais padrões abertos para
dados geo, juntamente com as vantagens e desvantagens de cada um.

##### GeoJSON

É um formato aberto baseado em [JSON](#json) para representar informações
geográficas. Possibilita representar formas como pontos, linhas e polígonos
com coordenadas geográficas, juntamente com seus atributos não-espaciais.
O GeoJSON não é mantido por um órgão formal de padronização, como alguns
outros formatos para informações geográficas. Em vez disso, ele é especificado
por um grupo de trabalho de desenvolvedores.
(do [Glossário](/Gloss%C3%A1rio/#geojson)).

`++++++`:
* Todos os benefícios do JSON
* Bom suporte de ferramentas
* Leve para processamento

`------`:
* Falta padronização (embora a especificação seja aberta)

##### KML

`++++++`:
* Formato padronizado
* Bom suporte de ferramentas

`------`:
* Mais pesado para processamento que o GeoJSON

##### Shapefile ESRI

`++++++`:
* Amplo suporte de ferramentas
----`------`:
* Falta padronização (embora a especificação seja aberta)
* Necessita múltiplos arquivos para um único mapa
* Possui limitações no armazenamento de atributos

#### Formatos baseados em RDF

`++++++`:
* possibilidade de utilizar semântica para descrever os dados
* facilita o cruzamento e ligação de dados entre fontes diversas
* potencializa a reutilização de ferramentas especializadas em dados de determinado domínio da informação
* facilita a descoberta de conhecimento ao possibilitar queries mais complexas usando dados de diversos domínios

`------`:
* necessita desenvolver ontologia que descreve os conceitos relacionados aos dados [link para algo sobre ontologias]
* maior complexidade do meta-modelo (grafos)
* maior heterogeneidade nas estrutura dos dados

##### tipo: RDF/Turtle

`++++++`:
* Sucinto (os arquivos gerados são menores)
* Simplicidade de leitura por humanos
* Formato padronizado
* Bom suporte de ferramentas
* Leve para processamento

`------`:

##### tipo: RDF/XML

`++++++`:
* Formato padronizado
* Amplo suporte de ferramentas

`------`:
* Dificuldade de leitura por humanos
* Utiliza estrutura hierárquica para representar um modelo de grafos
* Prolixo (os arquivos gerados são maiores)
* Mais pesado para processamento

##### JSON-LD

`++++++`:
* Formato padronizado
* Leve para processamento
* Utilizável diretamente em navegadores (leitura por javascript)

`------`:
* Menor suporte de ferramentas por ser um padrão mais recente

