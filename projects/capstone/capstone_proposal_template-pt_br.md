# Nanodegree Engenheiro de Machine Learning
## Proposta de projeto final
Everton Alexandre
08 de abril de 2018

## Proposta

### Histórico do assunto

O presente artigo descreve de forma sucinta a proposta de trabalho final do grupo Nanodegree Engenheiro de Machine Learning. O assunto escolhido para este trabalho está relacionado com a utilização de Machine Learning para a previsão do preço no mercado de ações. Fundos de investimento e bancos tem usado técnicas de aprendizado de máquina de forma a ter um entendimento melhor sobre o comportamento do mercado financeiro. Existem muitas API's que fornecem dados históricos sobre este tema. Além disso, tenho negociado no mercado de ações e mercado futuro há mais de 5 anos, fato que me motivou a escolher este tema para o projeto final sobre Machine Learning.

### Descrição do problema

O mercado de ações no Brasil movimenta bilhões de reais todos os dias. Milhões de negocios são fechados a cada dia. O nosso objetivo nesse trabalho será prever o comportamento dos preços das ações do mercado financeiro brasileiro. Como dados de entrada serão utilizados os preços de abertura, máxima, mínima, fechamento e volume negociado.

### Conjuntos de dados e entradas

Para este trabalho serão utilizados os dados do Google Finance, pois é uma ferramenta livre, ou seja, qualquer indivíduo pode entrar no Google Finance e obter dados históricos da Bovespa.
Será utilizado como dados de entrada o preço de abertura da ação, o preço máximo no dia, o preço mínimo no dia, o preço de fechamento, o volume financeiro negociado no dia e a data. Será utilizado o horizonte de tempo diário. Ou seja, cada dia útil terá uma abertura, um fechamento, uma máxima, uma mínima e um dado volume financeiro. Será utilizado dados históricos de 7 anos aproximadamente. O objetivo é, através dos dados de entrada anteriormente citados, realizar uma previsão no preço do próximo dia.

### Descrição da solução
_(aprox. 1 parágrafo)_

Tentar prever o mercado de ações é uma perspectiva atraente para os cientistas de dados, motivados não apenas pelo desejo de ganho material, mas pelo desafio. Vemos os altos e baixos diários do mercado e imaginamos que deve haver padrões. Este contexto me motivou a utilizar uma solução de Machine Learning aplicada ao mercado financeiro.
Basicamente, realizaremos a previsão do preço de fechamento da ação, ou seja, o fechamento será a variável alvo e o preço de abertura, preço máximo, preço mínimo e volume serão os dados de entrada.
Primeiramente iremos obter os dados utilizando a ferramenta Google Finance. Será analisado um horizonte de 9 a 10 anos. Após, iremos realizar a manipulação dos dados através da biblioteca Pandas e Numpy. Nesta etapa será realizada a preparação dos dados, identificação dos atributos e variáveis alvo. Após, utilizaremos a bibliteca sklearn.cross_validation para separação dos dados em treinamento e teste. Cerca de 75% dos dados serão utilizados para treinamento e 25% para teste. Em seguida, será o momento de realizar a escolha do modelo e realizar treinamento e testes. Após escolher o melhor modelo será o momento que realizar os ajustes finos no modelo, configurando e calibrando os parâmetros. Por fim, utilizaremos sklearn.metrics para verificar a pontuação do modelo no treinamento e teste. 

### Modelo de referência (benchmark)
_(aproximadamente 1-2 parágrafos)_

Nesta seção, forneça os detalhes de um modelo ou resultado de referência que esteja relacionado ao assunto, definição do problema e solução proposta. Idealmente, o resultado ou modelo de referência contextualiza os métodos existentes ou informações conhecidas sobre o assunto e problema propostos, que podem então ser objetivamente comparados à solução. Descreva detalhadamente como o resultado ou modelo de referência é mensurável (pode ser medido por alguma métrica e claramente observado).

### Métricas de avaliação
_(aprox. 1-2 parágrafos)_

Como, na minha concepção, estamos tratando de um problema de regressão e não de classificação o modelo não irá acertar a previsão no número exato. Ou seja, provavelmente o número previsto não será o número real. Entretanto, o que se espera desse modelo é que apresente uma taxa de erro baixa. Dessa forma, iremos utilizar como métrica o "Root Mean Square Error". Para maiores detalhes sobre essa métrica podemos acessar o seguinte link: https://en.wikipedia.org/wiki/Root-mean-square_deviation.

### Design do projeto
_(aprox. 1 página)_

Nesta seção final, sintetize um fluxo de trabalho teórico para obtenção de uma solução para o problema em questão. Discuta detalhadamente quais estratégias você considera utilizar, quais análises de dados podem ser necessárias de antemão e quais algoritmos serão considerados na sua implementação. O fluxo de trabalho e discussão propostos devem estar alinhados com as seções anteriores. Adicionalmente, você poderá incluir pequenas visualizações, pseudocódigo ou diagramas para auxiliar na descrição do design do projeto, mas não é obrigatório. A discussão deve seguir claramente o fluxo de trabalho proposto para o projeto de conclusão.

-----------

**Antes de enviar sua proposta, pergunte-se. . .**

- A proposta que você escreveu segue uma estrutura bem organizada, similar ao modelo de projeto?
- Todas as seções (em especial, **Descrição da solução** e **Design do projeto**) estão escritas de uma forma clara, concisa e específica? Existe algum termo ou frase ambígua que precise de esclarecimento?
- O público-alvo de seu projeto será capaz de entender sua proposta?
- Você revisou sua proposta de projeto adequadamente, de forma a minimizar a quantidade de erros gramaticais e ortográficos?
- Todos os recursos usados neste projeto foram corretamente citados e referenciados?
