# Descrição das tabelas do modelo
<h2> Tabela professores_historico_alunos </h2>
Descreva dentrode um modelo relacional elaborado, onde e quais os atributos serão armazenados no historico, tanto como aluno e professor, dentro do nosso banco. Nela possuimos os atributos/colunas. 
<ul><li>
    COD_PROF : chave primária.</li>
    <li>nome: permite diferenciar e identificar cada aluno e professor.</li>
    <li>endereço: permite mostrar onde cada um mora.</li>
    <li>cidade: região onde o aluno mora.</li>
    <li>fk_disciplina_cod_disc: chave estrangeira que faz referência a tabela disciplina.</li>
    <li>mat: chave primaria da matricula do aluno.</li>
    <li>cod_disc: chave primária do código disciplina.</li>
    <li>cod_turma: chave primária do codigo da turma.</li>
    <li>ano: ano que cursa ou série que estuda.</li>
    <li>frequência: numero da frequência de cada aluno.</li>
    <li>nota: nota atribuida ao desempenho dos alunos.
    </li></ul>

<h2>Tabela turma</h2>
<p>A tabela turma identifica a quantidade de alunos e seus devidos professores,incluindo horário e as notas de seus alunos .Nela possuímos atributos/colunas.</p> 
<ul>
    <li>cod_disc: número de identificação de cada disciplina.</li>
    <li>cod_prof: número de identificação de cada professor.</li>
    <li>cod_turma: chave primária da tabela.</li>
    <li>ano: série que estuda.</li>
    <li>horário: hora de estudo e funcionamento. </li>
    <li>fk_alunos_Mat : chave estrangeira q faz referência a tabela alunos.</li>
</ul>

<h2>Tabela Disciplina</h2>
<p>Essa tabela é usada principalmente para armazenar as disciplinas que cursa cada aluno.
Nela possuímos atributos/colunas.</p>
<ul>
    <li>cod_disc: chave primária da tabela. </li>
    <li>nome_disc: nome dado a cada disciplina.</li>
    <li>carga_hor: quantidade total de horas de cada disciplina.</li>
</ul>

<h2>Tabela pro_tur</h2>
<p>É a relação entre professor e turma, onde será armazenado seus dados no banco de dados.</p>
<ul>
    <li>fk_turma_cod_turma: chave estrangeira da tabela.</li>
    <li>fk_professores_históricos_alunos : chave estrangeira da tabela professores_historico_aluno.</li>
</ul>

<h2>Tabela alu_pro</h2>
<p>Essa tabela é a relação entre professor e aluno,  onde contém e será armazenados dados dos dois, onde se organizam no banco.</p>
<ul>
    <li>fk_histórico_alunos_Mat: chave estrangeira da tabela alunos.</li>
    <li>fk_histórico_alunos_cod: chave estrangeira da tabela alunos.</li>
    <li>fk_professores_histórico: chave estrangeira da relação professor e histórico.</li>
</ul>
