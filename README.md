<h1>Atividade Avaliativa - Banco de Dados</h1>
<p> Repositório com o diagrama lógico e conceitual.</p>

<h3>○ Diagrama Lógico</h3>
<div align="center">
 <img src="https://github.com/Lettxys/Atividade.Avaliativa/blob/main/DiagramaLogico.png?raw=true"/>
</div>

<h1>Descrição das tabelas do modelo</h1>
<h2>Tabela <i>Professores</i></h2>
A tabela <i>Professores</i> indica as informações básicas sobre os professores.
Nela possuímos os atributos/colunas:
<ul>
  <li>cod_prof: chave primária da tabela</li>
  <li>nome_prof: nome do professor</li>
  <li>endereco_prof: endereço do professor</li>
  <li>cidade_prof: cidade de que o professor vem</li>
</ul>

<h2>Tabela <i>Disciplinas</i></h2>
A tabela <i>Disciplinas</i> apresenta as informações de cada disciplina da universidade.
Nela possuímos os atributos/colunas:
<ul>
 <li>cod_disc: chave primária da tabela</li>
 <li>nome: nome da disciplina</li>
 <li>carga_hr: carga horária da disciplina</li>
</ul>

<h2>Tabela <i>Possuem</i></h2>
Tabela <i>possuem</i> tabela de ligação entre as tabelas </i>professores</i> e <i>disciplinas</i>.
Nela possuímos os atributos/colunas:
<ul>
  <li>fk_disciplinas_cod_disc: chave estrangeira que faz referência a tabela <i>disciplinas</i></li>
  <li>fk_professores_cod_prof: chave estrangeira que faz referência a tabela <i>professores</i> </li>
</ul>

<h2>Tabela <i>Turma</i></h2>
Tabela <i>turma</i> aqui teremos as informações sobre as turmas da universidade, relacionando-se com as tabelas </i>professores</i> e <i>disciplinas</i>.
Nela possuímos os atributos/colunas:
<ul>
 <li>cod_turma: chave primária da tabela</li>
 <li>cod_prof: código do professor na turma, faz referência a tabela </i>professores</i></li>
 <li>ano: ano da turma e segunda chave primária</li>
 <li>horário: horários da turma</li>
 </ul>
 
 <h2>Tabela <i>Tem</i></h2>
Tabela <i>tem</i> tabela de ligação entre as tabelas </i>turma</i> e <i>disciplinas</i>.
Nela possuímos os atributos/colunas:
<ul>
  <li>fk_disciplinas_cod_disc: chave estrangeira que faz referência a tabela <i>disciplinas</i></li>
  <li>fk_turma_cod_turma: chave estrangeira que faz referência a tabela <i>turma</i> </li>
  <li>fk_turma_ano:chave estrangeira que faz referência a tabela <i>turma</i></li>
</ul>

<h2>Tabela <i>historico</i></h2>
Tabela <i>historico</i> nesta tabela há o histórico da turma e dos alunos.
Nela possuímos os atributos/colunas:
<ul>
 <li>cod_disc: código de registro da disciplina;</li>
 <li>cod_prof: código de registro do professor;</li>
 <li>frequência: frequência da turma;</li>
 <li>nota: nota dos alunos.</li>
 <li>fk_alunos_mat: chave estrangeira que faz referência a tabela <i>aluno</i></li>
 <li>fk_turma_cod_turma: chave estrangeira que faz referência a tabela <i>turma</i></li>
 <li>fk_turma_ano: chave estrangeira que faz referência a tabela <i>turma</i></li>
</ul>

<h2>Tabela <i>alunos</i></h2>
Tabela <i>historico</i> nesta tabela há as informações dos alunos.
Nela possuímos os atributos/colunas:
<ul>
<li>mat: chave primária da tabela</li>
<li>nome: nome do aluno</li>
<li>endereço: endereço do aluno</li>
<li>cidade: cidade onde reside o aluno</li>
</ul>

