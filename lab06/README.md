# Aluno
* 216741: George Gigilas Junior

# Análise do Artigo G-FranC: A dataset of Criminal Activities mapped as a Complex Network in a Relational DBMS

| campo | valor |
|------------|----------------------------------------|
| referência | Scabora, L., Spadon, G., Rodrigues, L. S., Cazzolato, M. T., Araújo, M. V. S., Sousa, E. P. M., Traina, A. J. M., Rodrigues-Jr, J. F., & Traina-Jr, C. (2019). G-FranC: A dataset of Criminal Activities mapped as a Complex Network in a Relational DBMS. Dataset Showcase Workshop, SBBD 2019. https://sites.google.com/view/sbbd-dsw/artigos?authuser=0 |
| link       | [url para acesso à página do artigo](https://drive.google.com/file/d/1aDWRGteO0y5WwL6zl509YBEY8BulAwht/view) |
| dataset | [link para o repositório público onde está hospedado o dataset](https://bitbucket.org/gbdi/g-franc/.) |
| formato | csv |

## Resumo

> O artigo consiste da criação do dataset G-FranC, que mapeia atividades criminais como um grafo em um banco de dados relacional. Ao longo de sua introdução, os autores explicam a utilidade de utilizar esse grafo para tomar decisões para melhorar a segurança local, a partir de dados criminais. O artigo explica que os dados são sobre a cidade de São Francisco, Califórnia (EUA), e que o dataset relaciona o grafo da cidade com dados de crimes de vários tipos. Nessa seção, também é discutido como esses dados são guardados em um banco de dados relacional, com tabelas para os vértices do grafo e para as arestas.
> 
> Após a introdução, o artigo detalha os passos para criação do dataset, desde a aquisição dos dados (e suas fontes), até o mapeamento de dados criminais para um grafo georeferenciado, detecção de comunidades criminosas e a estrutura do dataset. Os autores explicam, detalhadamente, as fontes utilizadas, os algoritmos utilizados para cada etapa, formalismos matemáticos para alguns conceitos utilizados, tecnologias e linguagens de programação utilizadas e os campos de cada tabela do banco de dados.
> 
> Então, o artigo passa por 3 exemplos de análises do dataset: análise de vizinhança (proporção das categorias criminais na vizinhança de um nó), análise de comunidade (mapeia a área das 5 maiores comunidades criminosas) e análise temporal (análise de tendências criminosas ao longo dos anos e dos meses de cada ano). Todos esses exemplos estão bastante detalhados e seus resultados são apresentados de forma bem ilustrativa.
> 
> Considerando o dataset criado, os autores falam sobre sua aplicabilidade (e compatibilidade com outras tecnologias), desafios e limitações do processamento desses dados. Nessa seção, é mostrado como pode ser importante a contribuição desse dataset para combater esses desafios, o que será mais detalhado no próximo tópico "Perguntas de pesquisa/análises". Além disso, os autores discutem sobre as limitações desse dataset, por conta da falta de dados para algumas regiões, e que isso deve melhorar ao longo dos anos.
> 
> Por fim, o artigo descreve como se pode obter e fazer download desses dados, assim como deixam explicito assuntos como licenças e direitos autorais. O artigo finaliza concluindo e retomando o que foi desenvolvido ao longo dele.

## Perguntas de pesquisa/análises

> O dataset pode contribuir para responder perguntas sobre: 
> + A evolução das comunidades criminosas ao longo do tempo, a partir da análise do número de nós e tamanho absoluto das comunidades identificadas pelo algoritmo de Nerstrand. Isso pode ser uma medida de verificação da efetividade da atuação policial para combater crimes.
> + A conexão entre crimes distintos para detectar padrões, inferir e prever relações de causa e efeito baseado no local e no tipo do crime. Isso pode ser aplicado em uma escala global para contribuir mundialmente para a redução de crimes.
> + A inclusão de métricas de grafos em análises criminais (como proximidade, vizinhança), que já são muito utilizadas em outras áreas para análises de cidade.

## Trabalhos relacionados

> O texto cita trabalhos relacionados como:
> + [Nieto-Chaupis 2018a, Nieto-Chaupis 2018b], em que os autores revisaram aspectos sociais de índices de criminalidade nas ruas associados com dados de trânsito na cidade de Lima, Peru, além de estudarem dados relacionados a identificação de anomalias sociais em algumas cidades da América Latina. Esse trabalho é bem relacionado com o artigo descrito, porém ele é mais focado na relação do crime com o trânsito, enquanto o artigo descrito foca em identificar regiões e comunidades de crime.
> + [Ferreira et al. 2018], em que os autores aplicaram grafos (igual ao estudo do artigo) para estudar assuntos de segurança pública em Bogotá, Colômbia.
> + [Spadon et al. 2016], em que os autores identificam e estudam regiões criminosas de uma cidade, revisando casos em que crimes similares se concentram em áreas próximas. Esse conceito foi explorado no artigo descrito, em que se avaliou crimes a redor de um nó.
> + [Spadon et al. 2017], em que foi proposto um algoritmo para medir a dispersão de criminalidade em áreas de muita concentração de crime, permitindo a identificação de áreas de crimes recorrentes e de espalhamento de atividades criminais ao longo da regiões da cidade, o que também pode ser explorado pelo artigo descrito, que analisa diversos nós.
> + [Galbrun et al. 2016], [Fitterer et al. 2014], [Bogomolov et al. 2014], que estimam a probabilidade de ocorrer um crime, a partir de análises específicas, que também se relacionam a um dos desafios para o qual o G-FranC pode ser útil.
