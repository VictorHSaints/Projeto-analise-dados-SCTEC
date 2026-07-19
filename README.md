# Projeto-analise-dados-SCTEC
Projeto final avaliativo do curso Analise e visualização de dados do modulo de modelagem de dados do SCTEC
Victor Hugo dos Santos, turma 2
### Objetivo
Objetivo foi explorar conhecimentos de SQL, analise exploratória de dados e criação de gráficos no python. A utilização do freeSQL para exportação das tabelas para analise, uso das bibliotecas pandas, matplotlib e seaborn usando as tabelas do esquema HR para buscar informações, organizar os dados e transformá-los em uma análise fácil de entender.

### Tabelas utilizadas
As tabelas usadas eram um esquema de dados de RH, a tabela fato registrando as contratações e as tabelas dimensão departamento, trabalho, cidade, região e pais exploravam detalhes das mesmas.

### Consultas
As consultas principais foram Salarios_dep_carg_query_1 e Salarios_localizacao_query_2, sendo feitas também duas auxiliares Media_salarios_localizacao e Media_salarios_dep_carg. As consultas tiveram como objetivo investigar como se comportavam os salarios com base em cargo, departamento e localização.

### Resultados
Durante as analises foi possivel perceber que as tabelas não eram homogeneas, contendo outliers, ao analisar os dados como um todo podemos ver que o salário do diretor era um ponto bem fora da curva, além disso podemos verificar que uma concentração de até 50% até aproximadamente 6000 e cerca de 75% até 9000, o histograma corrobora essa informação mostrando uma concentração de quase 50 pessoas ganhando menos de 5000.

Depois podemos ver no Boxplot os extremos, sendo o extremo superior bem afastado e o outlier ainda mais (diretor). O histograma também auxilia a visualizar isso ao verificarmos que a linha vai descrescendo rapidamente.

![Histograma e boxplot dos salários](.\Outputs\boxplot_histograma.png)


Analisando por região a europa tem dados mais homogeneos, já as américas tem mais outlier e dados muito concentrados. 
![Boxplot por região](.\Outputs\boxplot_regiao.png)


Assim foi feita uma analise por departamento, revelando que essa disparidade se recai sobre o departamento da diretoria, tendo sua média salarial quase 2x maior que o departamento de contabilidade que tem a segunda maioir média. 

![histograma sálarios por departamento](.\Outputs\media_salaria_departamentos.png)


Por fim foi realizada a analise de gastos nos salários, demonstrando que no acumulado que por mais que não sejam os com maiores salários o setor de vendas mais acumula investimento com pessoal.

Quando analisamos por pais e cidade os Estados Unidos e Reino Unido acumulam quase todos os gastos, dentro desses países o investimento se concentra nas cidades de Oxford, Seattle e South San Francisco.




![Analise soma salários](.\Outputs\analise_somatório_salarios.png)

### Execução
1º passo: execussão da primeira celula para instalação das bibliotecas Numpy, Pandas, Matplotlib, Seaborn se houver instalado.
2º passo: execussão das seguintes celular em ordem para execussão. 


### Sugestões de melhoria para futuras versões

Caso sejam informações pertinentes de acompanhamento, sugere-se uma forma de integração com plataformas de BI para acompanhamento.

É interessante fazer analises do salário ao longo do tempo, um profissional que entra agora ganha o mesmo que o que já está na empresa? se não qual a relação de tempo e disparidade salarial? Se for possivel a coleta de dados como de satisfação é possivel fazer analises de relação entre salário e satisfação dos funcionários.
