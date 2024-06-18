# Student Scores Clustering

(EN)

This assignment was a part of the 2024.1 Data Mining coursework at the Federal University of ABC (UFABC). Special thanks to professor Debora Medeiros :)

## Assignment
Conduct a clustering analysis in a database of your choice by following these steps:

1. Select a database to work with.

2. Conduct a preliminary examination of the database.

3. Conduct the Clustering Analysis (including preprocessing methods):
   - Determine the number of clusters.
   - Apply clustering algorithms.

4. Select and interpret the results:
   - For k-means, explore the centroids.
   - Use the pandas `groupby` function with the resulting clusters to observe their numerical attributes, such as means.
   - Fit a decision tree using the resulting groups as classes.

**Note**: if rescaling is used in item 4, the original attributes must be restored, for example:

- By using the original database and adding the resulting group labels.
- By using the **inverse_transform** method of the scaler.

The selected dataset is the [Student Scores](https://www.kaggle.com/datasets/mexwell/student-scores?rvi=1) dataset, available on Kaggle.

**Metadada retrieved from the dataset description:**

id: Unique identifier assigned to each student (we need this because it is possible that two or more students have the same name).

first_name: The first name of a student.

last_name: The last name of a student.

email: The email address of a student.

gender: The gender of a student.

math_score: The score obtained by a student in the subject of mathematics (0 – 100).

history_score: History score (0 – 100).

physics_score: Physics score (0 – 100).

chemistry_score: Chemistry score (0 – 100).

biology_score: Biology score (0 – 100).

english_score: English score (0 – 100).

geography_score: Geography score (0 – 100).

part_time_job: This indicates whether a student is engaged in a part-time job. Taking a part-time job can have an effect on grades.

absence_days: The total count of days the student was not present in class due to various reasons.

extracurricular_activities: This captures whether a student participates in extracurricular activities. It could include clubs, sports, arts, or other activities outside of regular academic coursework.

weekly_self_study_hours: This represents the number of hours a student spends on self-study each week. It indicates the amount of time the student dedicates to independent learning and studying outside of class.

career_aspiration: This column records the student's career aspirations or goals for the future. It provides insight into the profession or field the student aims to pursue after completing their education.

<br>

The purpose of this activity is to find clusters of students that share similar profiles according to the features presented in the dataset.

<br>

(PT)

Este projeto foi desenvolvido durante a disciplina de Mineração de Dados na Universidade Federal do ABC (UFABC), no primeiro quadrimestre de 2024. Agradecimento especial à professora Debora Medeiros :)

## Atividade
Realizar uma análise de presença de grupos em uma base de dados de seu interesse:
1. Escolha uma base de dados
2. Realize uma análise inicial
3. Realize a análise de agrupamento (investigando formas de pré-processamento)
 * Análise de número de grupos
 * Aplicação de algoritmos de agrupamento
4. Selecionar um dos resultados e realizar uma interpretação dos grupos utilizando, por exemplo:
 * No caso do k-means, interpretar os centróides
 * Função groupby do pandas com os grupos resultantes para observar suas características numéricas, como médias.
 * Ajustar uma árvore de decisão utilizando como classes os grupos resultantes.

No item 4 da atividade, no caso de utilização de reescala, os atributos originais devem ser restaurados, por exemplo:
* utilizando a base de dados original e adicionando os rótulos de grupo resultantes
* utilizando o método **inverse_transform** do *scaler*

Para este estudo, será utilizado o dataset [Student Scores](https://www.kaggle.com/datasets/mexwell/student-scores?rvi=1), disponível no Kaggle.

**Metadados retirados da documentação:**

id: Identificador único atribuído a cada estudante (necessário porque é possível que dois ou mais estudantes tenham o mesmo nome).

first_name: O primeiro nome do estudante.

last_name: O sobrenome do estudante.

email: O endereço de e-mail do estudante.

gender: O gênero do estudante.

math_score: A nota obtida pelo estudante na disciplina de matemática (0 - 100).

history_score: Nota em história (0 - 100).

physics_score: Nota em física (0 - 100).

chemistry_score: Nota em química (0 - 100).

biology_score: Nota em biologia (0 - 100).

english_score: Nota em inglês (0 - 100).

geography_score: Nota em geografia (0 - 100).

part_time_job: Indica se o estudante trabalha em um emprego de meio período. Ter um emprego de meio período pode afetar as notas.

absence_days: O total de dias em que o estudante faltou à aula por vários motivos.

extracurricular_activities: Indica se o estudante participa de atividades extracurriculares. Isso pode incluir clubes, esportes, artes ou outras atividades fora do currículo acadêmico regular.

weekly_self_study_hours: Representa o número de horas na semana que o estudante dedica ao estudo individual. Indica a quantidade de tempo que o estudante dedica à aprendizagem e aos estudos fora da sala de aula.

career_aspiration: Esta coluna registra as aspirações profissionais ou metas futuras do estudante. Fornece insights sobre a profissão ou área que o estudante pretende seguir após concluir sua formação.

<br>

O objetivo dessa atividade é encontrar grupos de estudantes que compartilham um perfil semelhante de acordo com as características presentes no dataset.
