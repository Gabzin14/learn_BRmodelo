# Modelo Conceitual

![Conceitual](https://user-images.githubusercontent.com/114401117/193117508-1032fbf1-765f-4fa9-bebb-882fd074f7aa.png)

# Modelo Lógico:
![logico_prova 2](https://user-images.githubusercontent.com/114401117/193117683-28c10d51-0876-466c-aa3f-a9345f3c4ab1.png)

# Descrição das tabelas do modelo
## Tabela professores_historico_alunos
Descreva dentro de um modelo relacional elaborado, onde e quais os atributos serão armazenados no historico, tanto como aluno e professor, dentro do nosso banco. Nela possuimos os atributos/colunas. 
* COD_PROF : chave primária.
* nome: permite diferenciar e identificar cada aluno e professor.
* endereço: permite mostrar onde cada um mora.
* cidade: região onde o aluno mora.
* fk_disciplina_cod_disc: chave estrangeira que faz referência a tabela disciplina.
* mat: chave primaria da matricula do aluno.
* cod_disc: chave primária do código disciplina.
* cod_turma: chave primária do codigo da turma.
* ano: ano que cursa ou série que estuda.
* frequência: numero da frequência de cada aluno.
* nota: nota atribuida ao desempenho dos alunos.

## Tabela turma
A tabela turma identifica a quantidade de alunos e seus devidos professores, incluindo horário e as notas de seus alunos. Nela possuímos atributos/colunas.
* cod_disc: número de identificação de cada disciplina.
* cod_prof: número de identificação de cada professor.
* cod_turma: chave primária da tabela.
* ano: série que estuda.
* horário: hora de estudo e funcionamento.
* fk_alunos_Mat : chave estrangeira q faz referência a tabela alunos.

## Tabela Disciplina
Essa tabela é usada principalmente para armazenar as disciplinas que cursa cada aluno.
Nela possuímos atributos/colunas.
* cod_disc: chave primária da tabela.
* nome_disc: nome dado a cada disciplina.
* carga_hor: quantidade total de horas de cada disciplina.

## Tabela pro_tur
É a relação entre professor e turma, onde será armazenado seus dados no banco de dados.
* fk_turma_cod_turma: chave estrangeira da tabela.
* fk_professores_históricos_alunos : chave estrangeira da tabela professores_historico_aluno.

## Tabela alu_pro
Essa tabela é a relação entre professor e aluno,  onde contém e será armazenados dados dos dois, onde se organizam no banco.
* fk_histórico_alunos_Mat: chave estrangeira da tabela alunos.
* fk_histórico_alunos_cod: chave estrangeira da tabela alunos.
* fk_professores_histórico: chave estrangeira da relação professor e histórico.

## Tabela alu_disc
Essa tabela é a relação entre aluno e disciplina, ela armazena os dados da disciplina e os dados do aluno para identificar qual disciplina estudar.Nela temos atributos/colunas.
* fk_alunos_mat: chave estrangeira da tabela alunos.
* fk_disciplinas_cod_disc: chave estrangeira da tabela disciplinas.
