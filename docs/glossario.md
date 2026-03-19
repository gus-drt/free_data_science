# 📖 Glossário de Ciência de Dados e IA

Este glossário contém os termos mais comuns utilizados em Ciência de Dados e Inteligência Artificial.

---

## A

### Acurácia (Accuracy)
Métrica que indica a proporção de previsões corretas em relação ao total de previsões. É calculada como `(Verdadeiros Positivos + Verdadeiros Negativos) / Total de amostras`. Embora seja uma métrica intuitiva, pode ser enganosa em datasets com classes desbalanceadas — por exemplo, um modelo que sempre prevê a classe majoritária pode ter alta acurácia, mas ser inútil na prática. Nesses casos, métricas como F1-Score ou AUC-ROC são mais adequadas.
[Saiba mais sobre Acurácia](https://developers.google.com/machine-learning/crash-course/classification/accuracy)

### Algoritmo
Conjunto finito e ordenado de instruções passo a passo para realizar uma tarefa ou resolver um problema. Em Ciência de Dados, algoritmos definem como um modelo aprende a partir dos dados — por exemplo, o algoritmo de Gradient Descent ajusta os parâmetros de uma rede neural iterativamente para minimizar o erro. A escolha do algoritmo certo depende do tipo de problema, do volume de dados e dos recursos computacionais disponíveis.
[Saiba mais sobre Algoritmos](https://pt.wikipedia.org/wiki/Algoritmo)

### API (Application Programming Interface)
Interface que permite a comunicação entre diferentes sistemas de software por meio de um conjunto de regras e protocolos. Em IA e Ciência de Dados, APIs são amplamente usadas para consumir modelos treinados como serviços (ex.: API do ChatGPT, Google Vision API), integrar fontes de dados externas e automatizar pipelines de dados. Uma API bem projetada abstrai a complexidade interna, expondo apenas as funcionalidades necessárias.
[Saiba mais sobre APIs](https://aws.amazon.com/pt/what-is/api/)

### Aprendizado de Máquina (Machine Learning)
Subcampo da Inteligência Artificial que capacita computadores a aprender padrões a partir de dados sem serem explicitamente programados para cada regra. Em vez de seguir instruções fixas, um modelo de ML ajusta seus parâmetros internos com base em exemplos, tornando-se capaz de generalizar para novos dados. Existem três paradigmas principais: supervisionado, não supervisionado e por reforço. ML é a base de aplicações como reconhecimento de imagens, recomendações de conteúdo e detecção de fraudes.
[Saiba mais sobre Machine Learning](https://www.ibm.com/br-pt/topics/machine-learning)

### Aprendizado por Reforço (Reinforcement Learning)
Paradigma de Machine Learning onde um agente interage com um ambiente, tomando ações e recebendo recompensas ou penalidades com base nos resultados. O objetivo é maximizar a recompensa acumulada ao longo do tempo, aprendendo uma política ótima de decisão. É a técnica por trás de conquistas como o AlphaGo (jogos de tabuleiro) e sistemas de controle robótico. Difere do aprendizado supervisionado pois não há um conjunto fixo de exemplos rotulados — o aprendizado ocorre pela interação contínua.
[Saiba mais sobre Aprendizado por Reforço](https://pt.wikipedia.org/wiki/Aprendizado_por_refor%C3%A7o)

### Aprendizado Profundo (Deep Learning)
Subcampo do Machine Learning que utiliza redes neurais artificiais com múltiplas camadas ocultas (daí o "profundo") para aprender representações hierárquicas de dados. Cada camada extrai características cada vez mais abstratas: em visão computacional, as primeiras camadas detectam bordas, as intermediárias formas e as finais objetos completos. Deep Learning revolucionou áreas como reconhecimento de fala, tradução automática e geração de imagens, sendo a base de modelos como GPT e DALL-E.
[Saiba mais sobre Deep Learning](https://www.ibm.com/br-pt/topics/deep-learning)

### Aprendizado Supervisionado
Paradigma de Machine Learning onde o modelo é treinado a partir de um conjunto de dados rotulados — isto é, cada exemplo possui uma entrada (features) e uma saída esperada (label). O modelo aprende a mapear entradas para saídas, minimizando o erro em relação aos rótulos conhecidos. Exemplos de tarefas supervisionadas incluem classificação de e-mails como spam/não-spam e previsão do preço de imóveis. É o paradigma mais utilizado em aplicações práticas de ML.
[Saiba mais sobre Aprendizado Supervisionado](https://developers.google.com/machine-learning/intro-to-ml/supervised)

### Aprendizado Não Supervisionado
Paradigma de Machine Learning onde o modelo encontra estruturas e padrões em dados sem rótulos predefinidos. Sem uma "resposta certa" para guiar o aprendizado, o modelo descobre agrupamentos naturais (clustering), reduz dimensionalidade ou aprende representações compactas dos dados. Exemplos incluem segmentação de clientes por comportamento de compra, detecção de anomalias e compressão de dados. É especialmente útil quando rotular dados manualmente é caro ou impraticável.
[Saiba mais sobre Aprendizado Não Supervisionado](https://www.ibm.com/br-pt/topics/unsupervised-learning)

---

## B

### Batch
Subconjunto de amostras do dataset processadas simultaneamente em uma única iteração de treinamento. Usar batches (em vez de processar amostra por amostra) torna o treinamento mais eficiente computacionalmente e permite o uso de GPUs que paralelizam cálculos em matriz. O tamanho do batch (batch size) é um hiperparâmetro importante: batches menores introduzem mais ruído (o que pode ajudar na generalização), enquanto batches maiores tornam o treinamento mais estável, mas exigem mais memória.
[Saiba mais sobre Batch no treinamento de redes neurais](https://towardsdatascience.com/batch-mini-batch-stochastic-gradient-descent-7a62ecba642a)

### Big Data
Termo que descreve conjuntos de dados de volume, velocidade ou variedade tão elevados que ferramentas tradicionais de processamento não são suficientes para capturá-los, armazená-los e analisá-los eficientemente. Os "5 Vs" do Big Data são: Volume (quantidade de dados), Velocidade (taxa de geração), Variedade (diferentes formatos), Veracidade (qualidade) e Valor (utilidade). Tecnologias como Hadoop, Spark e sistemas de banco de dados distribuídos foram criadas para lidar com esse desafio.
[Saiba mais sobre Big Data](https://www.oracle.com/br/big-data/what-is-big-data/)

### Bias (Viés)
Tendência sistemática de um modelo a errar de uma maneira específica, independentemente do volume de dados de treinamento. O bias pode ter origem estatística — quando o modelo é muito simples para capturar a complexidade dos dados (underfitting) — ou social, quando reflete preconceitos presentes nos dados históricos. Em ML, existe o trade-off clássico entre bias e variância: aumentar a complexidade do modelo reduz o bias, mas pode aumentar a variância. Identificar e mitigar vieses é fundamental para sistemas de IA éticos e confiáveis.
[Saiba mais sobre Bias em ML](https://towardsdatascience.com/what-is-bias-in-machine-learning-5b5e1738fc17)

---

## C

### Classificação
Tarefa de Machine Learning supervisionado que consiste em atribuir uma categoria (classe) a cada entrada, a partir de um conjunto de classes predefinidas. Quando há apenas duas classes, chamamos de classificação binária (ex.: fraude / não fraude); com mais classes, é multiclasse (ex.: classificar espécies de flores). Algoritmos comuns incluem Regressão Logística, Árvores de Decisão, SVM e Redes Neurais. A qualidade do classificador é avaliada por métricas como acurácia, F1-Score e AUC-ROC.
[Saiba mais sobre Classificação em ML](https://developers.google.com/machine-learning/intro-to-ml/supervised#classification)

### Clusterização (Clustering)
Técnica de aprendizado não supervisionado que agrupa dados em clusters (grupos) de forma que amostras dentro do mesmo grupo sejam mais similares entre si do que com amostras de outros grupos. A similaridade é geralmente medida por distâncias (Euclidiana, cosseno, etc.). Algoritmos populares incluem K-Means, DBSCAN e Agglomerative Clustering. Aplicações incluem segmentação de clientes, agrupamento de documentos e detecção de comunidades em redes sociais.
[Saiba mais sobre Clustering](https://scikit-learn.org/stable/modules/clustering.html)

### CNN (Convolutional Neural Network)
Arquitetura de rede neural profunda especialmente eficaz para processar dados com estrutura de grade, como imagens e séries temporais. Ao invés de conectar todos os neurônios entre si, as CNNs aplicam filtros convolucionais que detectam padrões locais (bordas, texturas, formas) de forma hierárquica e invariante a translação. As camadas de pooling reduzem a dimensionalidade preservando as características mais relevantes. CNNs são a base de sistemas de reconhecimento de imagens, diagnóstico médico por imagem e carros autônomos.
[Saiba mais sobre CNNs](https://pt.wikipedia.org/wiki/Rede_neural_convolucional)

### Cross-Validation (Validação Cruzada)
Técnica de avaliação que estima a capacidade de generalização de um modelo ao dividir o dataset em múltiplos subconjuntos (folds). No método k-fold mais comum, os dados são divididos em k partes; o modelo é treinado k vezes, usando k-1 partes para treino e 1 para validação em cada rodada. O desempenho final é a média das k avaliações. Isso reduz o viés da avaliação causado por uma divisão única treino/teste e é especialmente útil quando o dataset é pequeno.
[Saiba mais sobre Cross-Validation](https://scikit-learn.org/stable/modules/cross_validation.html)

---

## D

### Dataset
Conjunto de dados organizado e estruturado utilizado para treinar, validar ou avaliar modelos de Machine Learning. Um dataset é tipicamente composto por amostras (linhas) e features (colunas), podendo incluir rótulos para tarefas supervisionadas. A qualidade, representatividade e tamanho do dataset têm impacto direto no desempenho do modelo — "garbage in, garbage out" é um princípio fundamental. Repositórios como Kaggle, UCI ML Repository e Hugging Face Datasets disponibilizam datasets públicos para experimentação.
[Saiba mais sobre Datasets em ML](https://developers.google.com/machine-learning/data-prep)

### Data Augmentation
Técnica para aumentar artificialmente o tamanho e a diversidade de um dataset por meio de transformações nos dados existentes, sem coletar novos exemplos. Em visão computacional, isso inclui rotações, espelhamentos, zoom e alterações de brilho em imagens. Em NLP, técnicas como substituição de sinônimos e tradução reversa são comuns. Data augmentation ajuda a prevenir overfitting, torna o modelo mais robusto a variações e é especialmente valiosa quando coletar dados reais é caro ou difícil.
[Saiba mais sobre Data Augmentation](https://towardsdatascience.com/data-augmentation-techniques-in-python-f216ef5eed69)

### Data Pipeline
Sequência automatizada de etapas para coleta, processamento e transformação de dados, desde a fonte bruta até o destino final (banco de dados, modelo, dashboard). Um pipeline típico inclui ingestão, limpeza, transformação, validação e carregamento dos dados. Ferramentas como Apache Airflow, Luigi e Prefect são usadas para orquestrar e monitorar pipelines em produção. Pipelines bem projetados garantem reprodutibilidade, escalabilidade e rastreabilidade do fluxo de dados.
[Saiba mais sobre Data Pipelines](https://www.databricks.com/glossary/data-pipeline)

### Dimensionalidade
Número de features (atributos ou variáveis) que descrevem cada amostra em um dataset. Datasets de alta dimensionalidade apresentam desafios conhecidos como a "maldição da dimensionalidade": à medida que o número de dimensões cresce, o volume do espaço aumenta exponencialmente, tornando os dados esparsos e dificultando o aprendizado. Técnicas de redução de dimensionalidade como PCA, t-SNE e UMAP são usadas para compactar a representação dos dados preservando as informações mais relevantes.
[Saiba mais sobre a Maldição da Dimensionalidade](https://pt.wikipedia.org/wiki/Maldi%C3%A7%C3%A3o_da_dimensionalidade)

### Dropout
Técnica de regularização para redes neurais que, durante o treinamento, desativa aleatoriamente uma fração dos neurônios em cada iteração (com probabilidade p, geralmente entre 0,2 e 0,5). Isso força a rede a aprender representações redundantes e distribuídas, evitando que neurônios específicos se tornem excessivamente dependentes entre si. O resultado é um modelo mais robusto e que generaliza melhor para dados não vistos. Durante a inferência, todos os neurônios são ativados, mas seus pesos são escalados de acordo com a taxa de dropout.
[Saiba mais sobre Dropout](https://jmlr.org/papers/v15/srivastava14a.html)

---

## E

### Embedding
Representação vetorial densa de dados categóricos ou textuais em um espaço contínuo de baixa dimensão, onde itens semanticamente similares são posicionados próximos uns aos outros. Por exemplo, em embeddings de palavras (como Word2Vec ou GloVe), "rei" e "rainha" estão próximos no espaço vetorial, e operações como `vetor("rei") - vetor("homem") + vetor("mulher") ≈ vetor("rainha")` são possíveis. Embeddings são fundamentais em NLP, sistemas de recomendação e qualquer tarefa que exija transformar dados discretos em representações numéricas significativas.
[Saiba mais sobre Embeddings](https://developers.google.com/machine-learning/crash-course/embeddings/video-lecture)

### Epoch (Época)
Uma passagem completa por todo o dataset de treinamento durante o processo de ajuste dos parâmetros do modelo. Em cada epoch, o modelo processa todas as amostras (divididas em batches), atualiza seus pesos e calcula o erro. Treinar por poucas épocas pode resultar em underfitting; treinar por muitas pode causar overfitting. O número de épocas é um hiperparâmetro importante, frequentemente escolhido em conjunto com técnicas de early stopping, que interrompem o treinamento quando o desempenho na validação para de melhorar.
[Saiba mais sobre Epochs](https://machinelearningmastery.com/difference-between-a-batch-and-an-epoch/)

### ETL (Extract, Transform, Load)
Processo fundamental em engenharia de dados composto por três etapas: Extração (coleta de dados de fontes diversas como bancos de dados, APIs e arquivos), Transformação (limpeza, normalização, agregação e enriquecimento dos dados para o formato desejado) e Carregamento (inserção dos dados transformados no destino final, como um data warehouse ou data lake). ETL é a espinha dorsal de sistemas de Business Intelligence e pipelines de ML em produção, garantindo que os dados estejam prontos para análise e modelagem.
[Saiba mais sobre ETL](https://aws.amazon.com/pt/what-is/etl/)

---

## F

### Feature (Característica)
Variável de entrada ou atributo individual que representa uma propriedade mensurável de uma amostra, usada como entrada para um modelo de ML. Por exemplo, para prever o preço de um imóvel, as features podem ser: área em m², número de quartos, localização e ano de construção. A qualidade e relevância das features têm impacto direto no desempenho do modelo — features irrelevantes adicionam ruído, enquanto features informativas melhoram a capacidade de aprendizado. A seleção e criação de features é uma das etapas mais importantes do processo de ML.
[Saiba mais sobre Features em ML](https://developers.google.com/machine-learning/crash-course/framing/ml-terminology)

### Feature Engineering
Processo de usar conhecimento de domínio para criar, transformar ou selecionar features a partir dos dados brutos, de forma a melhorar o desempenho do modelo. Inclui técnicas como criação de features derivadas (ex.: calcular a idade a partir da data de nascimento), codificação de variáveis categóricas, extração de informações temporais e combinação de features existentes. É considerada uma das etapas mais impactantes no ciclo de vida de um projeto de ML — modelos simples com boas features frequentemente superam modelos complexos com features ruins.
[Saiba mais sobre Feature Engineering](https://www.kaggle.com/learn/feature-engineering)

### Fine-tuning
Técnica de Transfer Learning que consiste em pegar um modelo pré-treinado em uma tarefa geral (ex.: um LLM treinado em grandes corpora de texto) e ajustar seus parâmetros — total ou parcialmente — em um dataset menor e específico para uma nova tarefa. Isso aproveita o conhecimento já adquirido pelo modelo base, reduzindo drasticamente o tempo e os dados necessários para obter bom desempenho. Fine-tuning é a abordagem padrão para adaptar modelos como BERT, GPT e ResNet a tarefas específicas de domínio.
[Saiba mais sobre Fine-tuning](https://huggingface.co/docs/transformers/training)

### F1-Score
Métrica de avaliação que combina Precisão e Recall em um único valor, calculada como a média harmônica entre as duas: `F1 = 2 × (Precisão × Recall) / (Precisão + Recall)`. É especialmente útil em cenários de classes desbalanceadas, onde a acurácia pode ser enganosa. O F1-Score varia de 0 (pior) a 1 (melhor). Existe também o F-beta score, que permite ponderar Precisão e Recall de acordo com a importância relativa de cada um para o problema em questão.
[Saiba mais sobre F1-Score](https://scikit-learn.org/stable/modules/generated/sklearn.metrics.f1_score.html)

---

## G

### GAN (Generative Adversarial Network)
Arquitetura de rede neural composta por dois modelos que competem entre si: o Gerador, que cria dados sintéticos (ex.: imagens falsas), e o Discriminador, que tenta distinguir dados reais de falsos. O treinamento adversarial faz o Gerador melhorar progressivamente até produzir dados indistinguíveis dos reais. GANs revolucionaram a geração de imagens sintéticas realistas, sendo a base de tecnologias como deepfakes, criação de arte com IA e aumento de datasets médicos onde dados reais são escassos.
[Saiba mais sobre GANs](https://developers.google.com/machine-learning/gan/gan_structure)

### Gradient Descent
Algoritmo de otimização iterativo usado para minimizar a função de perda de um modelo, ajustando os parâmetros na direção oposta ao gradiente (derivada parcial) da perda. A intuição é análoga a descer uma montanha dando passos na direção mais íngreme. A taxa de aprendizado controla o tamanho de cada passo. Variantes como SGD (Stochastic Gradient Descent), Adam e RMSprop são amplamente usadas em Deep Learning por sua eficiência em datasets grandes e espaços de parâmetros de alta dimensão.
[Saiba mais sobre Gradient Descent](https://developers.google.com/machine-learning/crash-course/reducing-loss/gradient-descent)

### GPU (Graphics Processing Unit)
Processador originalmente projetado para renderização gráfica, mas que se tornou indispensável em Deep Learning por sua capacidade de executar milhares de operações matemáticas em paralelo. Enquanto uma CPU possui dezenas de núcleos otimizados para tarefas sequenciais, uma GPU moderna possui milhares de núcleos menores ideais para multiplicações de matrizes — operação central no treinamento de redes neurais. Plataformas como NVIDIA CUDA e frameworks como TensorFlow e PyTorch foram desenvolvidos para aproveitar ao máximo esse poder de processamento paralelo.
[Saiba mais sobre GPUs em Deep Learning](https://developer.nvidia.com/deep-learning)

---

## H

### Hiperparâmetro
Parâmetro de configuração definido pelo cientista de dados antes do início do treinamento, que controla o processo de aprendizado mas não é aprendido diretamente a partir dos dados. Exemplos incluem: taxa de aprendizado, número de camadas e neurônios, taxa de dropout, tamanho do batch e número de épocas. Diferem dos parâmetros do modelo (como pesos de uma rede neural), que são ajustados automaticamente durante o treinamento. A busca pelo conjunto ótimo de hiperparâmetros é chamada de tuning e pode ser feita com Grid Search, Random Search ou otimização bayesiana.
[Saiba mais sobre Hiperparâmetros](https://www.ibm.com/br-pt/topics/hyperparameter-tuning)

### Holdout
Método simples de avaliação de modelos que consiste em dividir o dataset original em dois subconjuntos disjuntos: conjunto de treino (geralmente 70-80% dos dados) e conjunto de teste (20-30%). O modelo é treinado exclusivamente no conjunto de treino e avaliado no conjunto de teste, que simula dados não vistos. Uma variante mais completa usa três conjuntos: treino, validação (para ajuste de hiperparâmetros) e teste (para avaliação final). É mais rápido que Cross-Validation, mas pode ser instável com datasets pequenos.
[Saiba mais sobre Holdout](https://machinelearningmastery.com/train-test-split-for-evaluating-machine-learning-algorithms/)

---

## I

### Inteligência Artificial (IA)
Campo amplo da ciência da computação dedicado a criar sistemas e algoritmos capazes de realizar tarefas que normalmente requerem inteligência humana, como raciocínio, aprendizado, percepção, linguagem e tomada de decisão. A IA engloba subáreas como Machine Learning, Deep Learning, Processamento de Linguagem Natural, Visão Computacional e Sistemas Especialistas. Nos últimos anos, avanços em Deep Learning e LLMs levaram a IA a patamares sem precedentes, impactando setores como saúde, finanças, educação e entretenimento.
[Saiba mais sobre Inteligência Artificial](https://www.ibm.com/br-pt/topics/artificial-intelligence)

### Inferência
Processo de utilizar um modelo já treinado para gerar previsões ou saídas a partir de novos dados não vistos durante o treinamento. Distingue-se da fase de treinamento pois os parâmetros do modelo permanecem fixos — apenas o forward pass (propagação dos dados pelas camadas) é executado. Em produção, a eficiência da inferência (latência e throughput) é crítica. Técnicas como quantização, pruning e destilação de modelos são usadas para reduzir o custo computacional da inferência em ambientes de recursos limitados.
[Saiba mais sobre Inferência em ML](https://www.intel.com/content/www/us/en/learn/what-is-ai-inference.html)

---

## L

### Label (Rótulo)
Valor de saída conhecido associado a uma amostra de treinamento no aprendizado supervisionado, representando a "resposta certa" que o modelo deve aprender a prever. Em classificação, o rótulo é uma categoria (ex.: "gato" ou "cachorro"); em regressão, é um valor numérico (ex.: preço de uma casa). A qualidade dos rótulos é crucial: rótulos incorretos ou ambíguos (label noise) degradam diretamente o desempenho do modelo. O processo de criação de rótulos por humanos é chamado de anotação de dados, e pode ser caro e demorado.
[Saiba mais sobre Labels em ML](https://developers.google.com/machine-learning/glossary#label)

### Learning Rate (Taxa de Aprendizado)
Hiperparâmetro fundamental que controla o tamanho dos passos dados pelo algoritmo de otimização (ex.: Gradient Descent) ao atualizar os parâmetros do modelo. Uma taxa muito alta pode fazer o treinamento divergir ou oscilar; uma taxa muito baixa torna o treinamento lento e pode prender o modelo em mínimos locais. Técnicas como learning rate scheduling (reduzir a taxa ao longo do tempo) e warm restarts são usadas para equilibrar velocidade de convergência e estabilidade. É um dos hiperparâmetros mais sensíveis e impactantes em Deep Learning.
[Saiba mais sobre Learning Rate](https://developers.google.com/machine-learning/crash-course/reducing-loss/learning-rate)

### LLM (Large Language Model)
Modelo de linguagem de grande escala baseado na arquitetura Transformer, treinado em corpora massivos de texto (bilhões de palavras) com o objetivo de compreender e gerar linguagem natural. LLMs como GPT-4, Llama e Gemini demonstram capacidades emergentes notáveis, como raciocínio, tradução, geração de código e resposta a perguntas. São treinados com autosupervisionamento (previsão do próximo token) e posteriormente alinhados às preferências humanas via RLHF (Reinforcement Learning from Human Feedback).
[Saiba mais sobre LLMs](https://www.ibm.com/br-pt/topics/large-language-models)

### Loss Function (Função de Perda)
Função matemática que quantifica a discrepância entre as previsões do modelo e os valores reais, fornecendo um sinal de erro que guia a otimização durante o treinamento. A escolha da função de perda depende da tarefa: Cross-Entropy é padrão para classificação, Mean Squared Error (MSE) para regressão. O objetivo do treinamento é minimizar essa função ao longo do tempo. Uma função de perda bem escolhida alinha os incentivos do modelo com o objetivo real do problema.
[Saiba mais sobre Loss Functions](https://machinelearningmastery.com/loss-and-loss-functions-for-training-deep-learning-neural-networks/)

### LSTM (Long Short-Term Memory)
Variante de Rede Neural Recorrente (RNN) projetada para superar o problema do desaparecimento do gradiente, que dificulta o aprendizado de dependências de longo prazo em sequências. LSTMs utilizam células de memória e três tipos de "gates" (portas): esquecimento, entrada e saída, que controlam seletivamente quais informações são mantidas, atualizadas ou descartadas ao longo da sequência. Foram amplamente usadas em tarefas como tradução automática, reconhecimento de fala e previsão de séries temporais antes da popularização dos Transformers.
[Saiba mais sobre LSTM](https://colah.github.io/posts/2015-08-Understanding-LSTMs/)

---

## M

### Matriz de Confusão
Tabela que apresenta o desempenho de um modelo de classificação, cruzando os valores reais com as previsões do modelo. As linhas representam as classes reais e as colunas as classes previstas. Os elementos da diagonal principal são as previsões corretas (Verdadeiros Positivos e Verdadeiros Negativos), enquanto os elementos fora da diagonal são os erros (Falsos Positivos e Falsos Negativos). A partir da matriz de confusão, derivam-se métricas como Acurácia, Precisão, Recall e F1-Score, cada uma capturando diferentes aspectos do desempenho do classificador.
[Saiba mais sobre Matriz de Confusão](https://scikit-learn.org/stable/modules/model_evaluation.html#confusion-matrix)

### MLOps
Conjunto de práticas, ferramentas e cultura que integra Machine Learning com DevOps e Engenharia de Dados para operacionalizar modelos de ML em produção de forma confiável, escalável e reprodutível. Abrange todo o ciclo de vida do modelo: desenvolvimento, versionamento, implantação, monitoramento e retreinamento. Ferramentas como MLflow, DVC, Kubeflow e Weights & Biases são pilares do ecossistema MLOps. Sem boas práticas de MLOps, modelos de alto desempenho em pesquisa frequentemente falham ao serem implementados em sistemas reais.
[Saiba mais sobre MLOps](https://ml-ops.org/)

### Modelo
Representação matemática ou computacional aprendida a partir de dados, capaz de capturar padrões e relações para fazer previsões ou tomar decisões em novos exemplos. Um modelo é definido por sua arquitetura (estrutura) e pelos parâmetros aprendidos durante o treinamento. Pode ser simples, como uma regressão linear com dois parâmetros, ou extremamente complexo, como um LLM com bilhões de parâmetros. Em ML, o processo de treinamento é a busca pelos parâmetros que minimizam o erro do modelo no conjunto de dados de treino.
[Saiba mais sobre Modelos de ML](https://developers.google.com/machine-learning/glossary#model)

---

## N

### NLP (Natural Language Processing)
Subcampo da Inteligência Artificial dedicado a capacitar computadores a compreender, interpretar e gerar linguagem humana de forma natural. NLP combina linguística, estatística e Deep Learning para resolver tarefas como análise de sentimento, tradução automática, sumarização de texto, extração de informações e criação de chatbots. A chegada dos Transformers e dos LLMs revolucionou o campo, tornando possível sistemas como o ChatGPT que interagem fluentemente em linguagem natural em múltiplos idiomas.
[Saiba mais sobre NLP](https://www.ibm.com/br-pt/topics/natural-language-processing)

### Normalização
Técnica de pré-processamento que reescala os valores de features para um intervalo específico, tipicamente [0, 1] ou [-1, 1]. É obtida aplicando a fórmula `x_norm = (x - x_min) / (x_max - x_min)`. Modelos baseados em distância (como KNN e SVM) e redes neurais são sensíveis à escala das features — sem normalização, features com valores numericamente grandes dominam o aprendizado. Diferencia-se da Padronização (Standardização), que transforma os dados para ter média zero e desvio padrão um.
[Saiba mais sobre Normalização](https://scikit-learn.org/stable/modules/preprocessing.html#scaling-features-to-a-range)

### Neurônio
Unidade computacional fundamental de uma rede neural artificial, inspirada no neurônio biológico. Cada neurônio recebe múltiplas entradas, aplica uma soma ponderada (cada entrada multiplicada por seu peso), adiciona um bias e passa o resultado por uma função de ativação (como ReLU ou Sigmoid) para produzir uma saída. Redes neurais são compostas por camadas de neurônios interconectados: camada de entrada, camadas ocultas e camada de saída. O poder de representação da rede cresce com o número e a organização de seus neurônios.
[Saiba mais sobre Neurônios Artificiais](https://pt.wikipedia.org/wiki/Neur%C3%B4nio_artificial)

---

## O

### One-Hot Encoding
Técnica de codificação que transforma variáveis categóricas em vetores binários esparsos, criando uma coluna binária para cada categoria possível: a coluna da categoria presente recebe valor 1 e todas as demais recebem 0. Por exemplo, a feature "cor" com valores {vermelho, verde, azul} se torna três colunas binárias. Isso é necessário porque algoritmos de ML geralmente requerem entradas numéricas. Para categorias de alta cardinalidade (muitas categorias únicas), alternativas como Target Encoding ou Embeddings são mais eficientes.
[Saiba mais sobre One-Hot Encoding](https://scikit-learn.org/stable/modules/generated/sklearn.preprocessing.OneHotEncoder.html)

### Overfitting (Sobreajuste)
Fenômeno onde um modelo aprende os dados de treinamento com detalhe excessivo — incluindo o ruído e as peculiaridades específicas daquele conjunto —, perdendo a capacidade de generalizar para novos dados. Um modelo com overfitting apresenta baixo erro no treino, mas alto erro em dados não vistos. Ocorre tipicamente quando o modelo é muito complexo em relação ao volume de dados disponível. Técnicas para combater overfitting incluem regularização (L1/L2), Dropout, aumento de dados, redução da complexidade do modelo e early stopping.
[Saiba mais sobre Overfitting](https://developers.google.com/machine-learning/crash-course/overfitting/overfitting)

---

## P

### Pipeline
Sequência encadeada de transformações e operações aplicadas aos dados e ao modelo, de forma automatizada e reprodutível. Em ML, um pipeline típico conecta etapas como pré-processamento, extração de features, treinamento do modelo e avaliação. Ferramentas como `sklearn.pipeline.Pipeline` permitem encadear essas etapas de forma elegante, evitando vazamento de dados (data leakage) entre treino e teste. Pipelines bem projetados facilitam a experimentação, o versionamento e a implantação de modelos em produção.
[Saiba mais sobre Pipelines em ML](https://scikit-learn.org/stable/modules/compose.html)

### Precisão (Precision)
Métrica de avaliação para classificadores que mede a proporção de previsões positivas que são de fato corretas: `Precisão = Verdadeiros Positivos / (Verdadeiros Positivos + Falsos Positivos)`. Alta precisão significa que quando o modelo prevê positivo, raramente erra. É especialmente importante em cenários onde o custo de um Falso Positivo é alto — por exemplo, em detecção de spam (não queremos bloquear e-mails legítimos). Existe um trade-off clássico entre Precisão e Recall que deve ser equilibrado conforme o contexto do problema.
[Saiba mais sobre Precisão](https://developers.google.com/machine-learning/crash-course/classification/precision-and-recall)

### Pré-processamento
Conjunto de etapas de limpeza e transformação aplicadas aos dados brutos antes de alimentar um modelo de ML. Inclui tratamento de valores ausentes (imputação ou remoção), remoção de outliers, codificação de variáveis categóricas, normalização/padronização de features numéricas e seleção de features relevantes. A qualidade do pré-processamento tem impacto direto no desempenho final do modelo — dados mal preparados levam a modelos que aprendem padrões espúrios. É comum que o pré-processamento consuma 60-80% do tempo em projetos reais de Ciência de Dados.
[Saiba mais sobre Pré-processamento](https://scikit-learn.org/stable/modules/preprocessing.html)

---

## R

### Recall (Revocação)
Métrica de avaliação que mede a proporção de casos positivos reais que foram corretamente identificados pelo modelo: `Recall = Verdadeiros Positivos / (Verdadeiros Positivos + Falsos Negativos)`. Alto Recall significa que o modelo encontra a maioria dos positivos reais, mesmo que ao custo de alguns Falsos Positivos. É especialmente importante quando o custo de um Falso Negativo é alto — por exemplo, em diagnóstico de doenças graves (não queremos deixar de detectar casos reais). Está em trade-off com a Precisão.
[Saiba mais sobre Recall](https://developers.google.com/machine-learning/crash-course/classification/precision-and-recall)

### Regressão
Classe de tarefas de Machine Learning supervisionado que visa prever um valor numérico contínuo como saída, em vez de uma categoria discreta. Exemplos incluem previsão do preço de imóveis, temperatura amanhã ou vendas mensais. A regressão linear é o algoritmo mais simples, modelando a relação entre features e saída como uma função linear. Variantes mais complexas incluem regressão polinomial, Ridge, Lasso e redes neurais para regressão. O desempenho é avaliado por métricas como MSE, RMSE e R².
[Saiba mais sobre Regressão](https://developers.google.com/machine-learning/intro-to-ml/supervised#regression)

### Regularização
Conjunto de técnicas para prevenir overfitting, adicionando restrições ou penalidades ao processo de treinamento que limitam a complexidade do modelo. As formas mais comuns são L1 (Lasso), que penaliza a soma dos valores absolutos dos pesos e promove esparsidade, e L2 (Ridge), que penaliza a soma dos quadrados dos pesos e mantém pesos pequenos. Em redes neurais, Dropout é uma forma de regularização implícita. A regularização introduz um viés deliberado para reduzir a variância do modelo, melhorando sua capacidade de generalização.
[Saiba mais sobre Regularização](https://developers.google.com/machine-learning/crash-course/overfitting/regularization)

### RNN (Recurrent Neural Network)
Arquitetura de rede neural projetada para processar dados sequenciais (texto, áudio, séries temporais), onde a ordem dos elementos importa. Diferente das redes feedforward, as RNNs possuem conexões recorrentes que passam informações de um passo temporal para o próximo, mantendo um "estado oculto" que funciona como memória da sequência. O principal desafio das RNNs simples é o desaparecimento do gradiente em sequências longas, o que motivou o desenvolvimento de variantes como LSTM e GRU. Foram amplamente substituídas pelos Transformers em muitas tarefas de NLP.
[Saiba mais sobre RNNs](https://pt.wikipedia.org/wiki/Rede_neural_recorrente)

---

## S

### Scikit-learn
Biblioteca Python de código aberto amplamente utilizada para Machine Learning, construída sobre NumPy, SciPy e Matplotlib. Oferece implementações eficientes e consistentes de dezenas de algoritmos de classificação, regressão, clustering, redução de dimensionalidade, pré-processamento e validação de modelos. A API unificada (fit/transform/predict) facilita a criação de pipelines e a troca de algoritmos. É a escolha padrão para ML clássico em produção e pesquisa, e integra-se perfeitamente com o ecossistema científico Python.
[Saiba mais sobre Scikit-learn](https://scikit-learn.org/stable/)

### Split
Divisão do dataset disponível em subconjuntos distintos para garantir uma avaliação justa do modelo. O esquema mais completo usa três conjuntos: treino (para ajustar os parâmetros do modelo), validação (para ajustar hiperparâmetros e decisões de modelagem) e teste (para a avaliação final imparcial, nunca usado durante o desenvolvimento). A proporção típica é 70/15/15 ou 80/10/10. Usar dados de teste para qualquer decisão de modelagem contamina a avaliação, criando uma estimativa otimista do desempenho real.
[Saiba mais sobre Train-Test Split](https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.train_test_split.html)

### Standardização
Técnica de pré-processamento que transforma cada feature para ter média zero e desvio padrão um, aplicando a fórmula `x_std = (x - μ) / σ`. Ao contrário da normalização por min-max, a standardização não limita os valores a um intervalo fixo, sendo mais robusta a outliers. É o método de escalonamento preferido para algoritmos que assumem distribuição normal dos dados, como SVM, Regressão Logística e PCA, e para qualquer modelo sensível à escala das features, incluindo redes neurais.
[Saiba mais sobre Standardização](https://scikit-learn.org/stable/modules/generated/sklearn.preprocessing.StandardScaler.html)

---

## T

### TensorFlow
Framework de código aberto desenvolvido pelo Google Brain para computação numérica e Machine Learning em larga escala. Utiliza grafos computacionais para representar operações matemáticas, permitindo diferenciação automática e execução eficiente em CPUs, GPUs e TPUs. Com a API Keras integrada, TensorFlow oferece uma interface de alto nível para construção e treinamento de redes neurais. É amplamente usado em pesquisa e produção, com suporte a deploy em múltiplas plataformas, incluindo dispositivos móveis (TensorFlow Lite) e navegadores (TensorFlow.js).
[Saiba mais sobre TensorFlow](https://www.tensorflow.org/)

### Transformer
Arquitetura de rede neural introduzida no artigo "Attention is All You Need" (2017) que revolucionou o processamento de sequências ao substituir recorrência por mecanismos de atenção (self-attention). O self-attention permite ao modelo relacionar qualquer par de posições da sequência diretamente, independente da distância, capturando dependências de longo alcance de forma eficiente e paralelizável. Os Transformers são a base de virtualmente todos os LLMs modernos (GPT, BERT, T5, Llama) e também dominam tarefas de visão computacional (Vision Transformers).
[Saiba mais sobre Transformers](https://huggingface.co/learn/nlp-course/chapter1/4)

### Transfer Learning
Técnica que reutiliza o conhecimento adquirido por um modelo durante o treinamento em uma tarefa-fonte para melhorar o aprendizado em uma tarefa-alvo diferente, mas relacionada. Em vez de treinar do zero, parte-se de um modelo pré-treinado (ex.: ResNet treinada no ImageNet, ou BERT treinado em grandes corpora de texto) e adapta-se ao novo problema com muito menos dados e tempo de treinamento. É especialmente valioso quando dados rotulados para a tarefa-alvo são escassos. Transfer Learning é hoje a abordagem padrão em visão computacional e NLP.
[Saiba mais sobre Transfer Learning](https://www.ibm.com/br-pt/topics/transfer-learning)

### Treino (Training)
Processo iterativo de ajuste dos parâmetros (pesos) de um modelo a partir dos dados de treinamento, de forma que o modelo aprenda a fazer previsões cada vez mais precisas. A cada iteração, o modelo faz previsões, calcula o erro pela função de perda e atualiza os parâmetros na direção que reduz esse erro (via backpropagation e Gradient Descent). O treinamento termina quando o modelo converge (o erro estabiliza) ou após um número pré-definido de épocas. Monitorar curvas de treino e validação é essencial para diagnosticar overfitting e underfitting.
[Saiba mais sobre Treinamento de Modelos](https://developers.google.com/machine-learning/crash-course/training-and-loss/training-and-loss)

---

## U

### Underfitting (Subajuste)
Fenômeno oposto ao overfitting: ocorre quando o modelo é excessivamente simples para capturar os padrões e relações presentes nos dados, resultando em alto erro tanto no conjunto de treinamento quanto nos dados não vistos. Um modelo com underfitting não aprendeu adequadamente — equivale a tentar ajustar uma linha reta a dados que seguem um padrão claramente não-linear. Soluções incluem aumentar a complexidade do modelo (mais camadas, mais parâmetros), treinar por mais épocas, reduzir a regularização ou criar features mais informativas.
[Saiba mais sobre Underfitting](https://developers.google.com/machine-learning/crash-course/overfitting/underfitting)

---

## V

### Validação
Processo de avaliação do desempenho de um modelo em dados que não foram usados durante o treinamento, com o objetivo de estimar sua capacidade de generalização e guiar decisões de modelagem (como ajuste de hiperparâmetros). O conjunto de validação é separado dos dados de treino e de teste: enquanto o teste fornece a avaliação final imparcial, a validação é usada ao longo do desenvolvimento. Técnicas como Cross-Validation permitem uma estimativa mais robusta da performance com uso eficiente de todos os dados disponíveis.
[Saiba mais sobre Validação em ML](https://scikit-learn.org/stable/modules/cross_validation.html)

### Variância
No contexto de Machine Learning, descreve a sensibilidade do modelo a pequenas variações nos dados de treinamento. Um modelo com alta variância aprende os dados de treino com tanta especificidade que qualquer mudança no conjunto de treino resulta em previsões muito diferentes — sinal de overfitting. A variância está em trade-off direto com o bias: modelos simples têm alto bias e baixa variância; modelos complexos têm baixo bias mas alta variância. Encontrar o equilíbrio certo entre os dois é o objetivo central da seleção e regularização de modelos.
[Saiba mais sobre o trade-off Bias-Variância](https://towardsdatascience.com/understanding-the-bias-variance-tradeoff-165e6942b229)

### Vetor
Representação matemática unidimensional de dados, composto por uma sequência de números (coordenadas). Em IA, vetores transformam informações do mundo real (palavras, imagens, características) em formato numérico que computadores conseguem processar e comparar. Exemplo: uma pessoa pode ser representada pelo vetor [altura, peso, idade]. Vetores são fundamentais para operações de similaridade, transformações e aprendizado em modelos de Machine Learning.
[Saiba mais sobre Vetores em álgebra linear](https://pt.wikipedia.org/wiki/Vetor_(matem%C3%A1tica))

---

## X

### XGBoost
Implementação otimizada e altamente eficiente do algoritmo Gradient Boosting, desenvolvida por Tianqi Chen. Constrói um ensemble de árvores de decisão de forma sequencial, onde cada nova árvore corrige os erros residuais das anteriores. Destaca-se por sua velocidade (paralelização do treinamento), regularização integrada (L1 e L2) para evitar overfitting e capacidade de lidar com valores ausentes. É um dos algoritmos mais premiados em competições do Kaggle e amplamente usado em produção para dados tabulares, frequentemente superando Deep Learning nesse domínio.
[Saiba mais sobre XGBoost](https://xgboost.readthedocs.io/en/stable/)

---

*Este glossário será atualizado continuamente. Contribuições são bem-vindas!*
