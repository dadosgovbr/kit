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


### Glossário de Formatos:


