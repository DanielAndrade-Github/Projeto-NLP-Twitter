# Projeto-NLP-Twitter
Projeto de Análise de sentimentos em Tweets
Os segundo projeto do módulo de Dados não estruturados II será focado no processamento de linguagem natural! Usaremos os algoritmos aprendidos e as técnicas vistas na segunda parte do curso para extrairmos informações relevantes de texto. Mais precisamente, de publicações no Twitter.

Os Dados
Utilizaremos um Dataset obtido do Twitter com 100K postagens entre os dias 01/08/2018 e 20/10/2018. Cada postagem é classificada como positiva, negativa ou neutra.

Dois arquivos serão disponilizados para o desenvolvimento dos modelos, um para treino/validação e outro para submissão. Os arquivos se encontram na pasta /Dados/train e /Dados/subm, respectivamente.

Descrição das colunas:

id: ID único para o tweet
tweet_text: Texto da publicação no Twitter
tweet_date: Data da publicação no Twitter
sentiment: 0, se negativo; 1, se positivo; 2, se neutro
query_used: Filtro utilizado para buscar a publicação
O Problema
Você deverá desenvolver um modelo para detectar o sentimento de uma publicação do Twitter a classificando em uma das três categorias: positiva, negativa ou neutra. O texto da publicação está disponível na coluna "tweet_text". Teste pelo menos 2 técnicas de NLP diferentes e escolha a métrica de avaliação que julgar mais pertinente.

Escolha o melhor modelo e gere uma base a partir dos dados de submissão, que estão no caminho Dados/subm/Subm3Classes.csv, com o seguinte formato:

id	sentiment_predict
12123232	0
323212	1
342235	2
Salve essa tabela como um arquivo csv com o nome <nome>_<sobrenome>_nlp_degree.csv e submeta-o como parte da entrega final do projeto.

Para ajudar no desenvolvimento, é possível dividir o projeto em algumas fases:

Análise de consistência dos dados: analise se os dados estão fazendo sentido, se os campos estão completos e se há dados duplicados ou faltantes. Se julgar necessário, trate-os.
Análise exploratória: analise a sua base como um todo, verifique o balanceamento entre as classes e foque, principalmente, na coluna tweet_text.
Pré-processamento e transformações: projetos de NLP exigem um considerável pré-processamento. Foque no tratamento da string do texto. Procure começar com tratamentos simples e adicione complexidade gradualmente. Nessa etapa você testará diferentes técnicas de transformações, como o Bag Of Words e o TF-IDF.
Treinamento do modelo: depois das transformações, você poderá executar o treinamento do modelo classificador. Nessa etapa o problema se torna semelhante aos abordados nos módulos anteriores. Você pode testar diversos classificadores como RandomForest, AdaBoost, entre outros. Otimize os hiperparâmetros do modelo com técnicas como a GridSearch e a RandomizedSearch.
Conclusões: descreva, em texto, as conclusões sobre os seus estudos. O modelo é capaz de identificar o sentimento das publicações? É possível extrapolar o modelo para outros contextos, como a análise de sentimento de uma frase qualquer? Pense em questões pertinentes e relevantes que você tenha obtido durante o desenvolvimento do projeto!
