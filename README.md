Observações sobre o Código
Instalação de Pacotes:

A linha pip install transformers pandas é necessária para instalar as bibliotecas transformers e pandas antes de executar o código. Certifique-se de que isso esteja documentado no README do seu repositório.
Importação de Bibliotecas:

As bibliotecas transformers e pandas estão corretamente importadas. A biblioteca transformers é utilizada para carregar o modelo de análise de sentimentos, enquanto o pandas é usado para manipular e organizar os resultados.
Pipeline de Análise de Sentimentos:

A variável classifier é inicializada com o pipeline de análise de sentimentos. Isso é uma abordagem eficaz para utilizar modelos pré-treinados de forma simples e intuitiva.
Entrada de Dados:

Os dados são fornecidos como uma string longa, onde cada avaliação é separada por uma nova linha e as classificações reais estão após um ponto e vírgula.
O método strip() é usado para remover espaços em branco desnecessários, e rsplit(';', 1) é uma boa escolha para separar a avaliação do sentimento real.
Predição de Sentimentos:

O loop que itera sobre as avaliações e aplica o classificador a cada uma está bem estruturado.
O resultado da predição é armazenado em um dicionário, que é uma abordagem adequada para organizar os dados.
Criação do DataFrame:

A criação do DataFrame df_resultados para armazenar os resultados é uma boa prática, pois facilita a visualização e a análise posterior dos dados.
Saída dos Resultados:

O resultado final é impresso e também retornado como um DataFrame. Essa é uma maneira eficaz de visualizar os resultados diretamente no console.

Uso
Para executar a análise de sentimentos, execute o script:

python nome_do_script.py

Exemplo de Dados
As avaliações devem estar no formato:

Avaliação 1; sentimento
Avaliação 2; sentimento

As classificações podem ser "positivo" ou "negativo".

Resultados:
Os resultados da análise serão exibidos no console e salvos em um arquivo CSV chamado resultados_analisados.csv.

![image](https://github.com/user-attachments/assets/a02c7ed7-9da0-4993-aed1-6c2b9bb393e2)




