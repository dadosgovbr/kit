Elaboração do Plano de Dados Abertos
====

O Conteúdo que orienta a criação de um PDA está estruturado no [Manual para elaboração de Plano de Dados Abertos](http://www.planejamento.gov.br/secretarias/upload/Arquivos/governo_aberto/manual_elaboracao_plano_dados_abertos.pdf). Este guia se dispõe a resumir os principais passos do manual e trazer novas referências.

Antes de mergulhar na construção do PDA, há uma etapa anterior muito importante: Definir quem serão os responsáveis pela iniciativa e juntar as pessoas relevantes para as atividades em questão. Essas atividades estão estruturadas no [processo sistêmico](https://github.com/dadosgovbr/kit/blob/master/Processo-sist%C3%AAmico.md), vale a pena conferir antes de começar.

De maneira resumida, o processo de criação do PDA se resume a 4 etapas:

## Organizar Inventário de Dados

Antes de definir quais dados são publicados é imprescindível que a organização faça um levantamento de quais dados possui. Por incrível que pareça, poucos órgãos públicos tem esse levantamento feito.

Existem algumas formas de fazer esse levantamento, provavelmente a melhor estratégia é uma combinação delas:

* Levantar, junto com os representantes das diversas áreas, quais são os sistemas usados por cada uma
* Fazer uma lista com os dados pedidos pelo SIC
* Caso a manutenção de todos os sistemas seja centralizada em uma única área de TI, obter a lista dos sistemas com a área


## Priorizar os dados que serão abertos

A priorização ocorre porque não vale a pena a organização fazer um esforço para publicar todos os seus dados simultaneamente, o custo é muito alto e isso não implica necessariamente na publicação de **dados relevantes para o público**. 

Conforme o [manual para elaboração de PDA](http://www.planejamento.gov.br/secretarias/upload/Arquivos/governo_aberto/manual_elaboracao_plano_dados_abertos.pdf), a etapa de priorização deve considerar esses critérios:

1. O grau de relevância para o cidadão, observando-se especialmente as **demandas encaminhadas via e-SIC**, bem como os setores e serviços mais procurados nos sítios eletrônicos do órgão. Adicionalmente, a organização pode também realizar um encontro com os principais consumidores de seus dados (ex: organizações da sociedade civil, ONGs, pesquisadores, outros órgãos públicos) para entender aonde concentram-se suas necessidades;
2. Os normativos legais e os compromissos formalmente assumidos pelo órgão, inclusive perante organismos internacionais (ex: [OGP](http://www.cgu.gov.br/governoaberto/)); 
3. O alinhamento perante o Planejamento Estratégico Institucional (PEI) e os planejamentos setoriais, bem como os relacionados às áreas de tecnologia da informação;
4. O conjunto de informações e sistemas sob a gestão do órgão, em especial, se houver, sistemas estruturadores que são de uso obrigatório transversal para os órgãos da APF;
5. O nível de maturidade e organização das informações e dados existentes.

Outra fonte importante para basear-se é a definição de [conjuntos de dados de alto valor](https://www.gov.uk/government/publications/open-data-charter/g8-open-data-charter-and-technical-annex#action-2-release-of-high-value-data), 
trazida pelo [Open Data Charter](https://www.gov.uk/government/publications/open-data-charter) do [G8](http://en.wikipedia.org/wiki/G8).

## Definir estratégias de abertura

Priorizados os dados mais importantes, é hora de definir de que maneira eles serão publicados. Essa maneira será influenciada pelos seguintes fatores:

* Local onde os dados estão estruturados
* Forma como os dados estão estruturados
* Capacidade técnica da organização
* Capacidade orçamentária da organização

Na prática, esses fatores se traduzem em possíveis cenários de status dos dados, como dados estruturados em várias planilhas, bancos de dados locais, bancos de dados situados no fornecedor, conjuntos muito volumosos, plataforma alta ou baixa, data warehouse, etc. 

Cada cenário envolve uma tática diferente, em casos de dados muito volumosos, uma separação em diversos arquivos compactados, por exemplo, ou a criação de API, a depender também da capacidade dos órgãos. Dados de data warehouse devem ser evitados por causa dos princípios dos dados brutos e primários, mas excepcionalmente podem ser utilizados quando a extração direta não for viável.

Além da forma de publicação, a periodicidade de publicação e a forma de hospedagem precisam ser definidas, a depender das particularidades da área de negócio, dos sistemas de informação relacionados e dos recursos de infraestrutura disponíveis.


## Definir cronograma e marcos

Nesse momento já está definido, para cada um dos dados priorizados, a tática de publicação, dentro das limitações da organização e das particularidades das bases de dados. Resta agora pensar nas datas de publicação de cada um deles.

Essa é a ocasião certa para pensar em ações de comunicação e articulação com a sociedade civil para aumentar a legitimidade e potencializar a publicação dos dados. Exemplos de ação como essas são: 

* realizar encontros com os interessados nos dados
* realizar concursos de aplicativos
* utilizar os dados mais pedidos do SIC
* estimular o uso interno e por outros órgãos públicos dos dados publicados
* disseminar na organização a cultura de acesso à informação e de disponibilização de dados públicos.


