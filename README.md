# Modelagem e banco de dados em MySQL

Trabalho acadêmico cujo a proposta é desenvolver um banco de dados para uma escola.
Durante o projeto foi desenvolvido um modelo conceitual, lógico e o próprio banco no MySQL utilizando o <a href="https://dev.mysql.com/doc/">MySQL Workbench</a>.

sobre o banco de dados:
- Existem outras entidades além dessas três (curso, turma, aluno)?               
  As entidades do modelo proposto são: 
  - curso
  - turma
  - disciplina
  - aluno
  - professor
  
</br>
<img alt="modelo conceitual" width="100%" src="https://github.com/marcelo-souto/modelagem-dados-mysql/blob/main/modelo_conceitual.jpg?raw=true" />

- Quais são os principais campos e tipos?                     
  os principais campos que distinguem as entidades são as chaves primárias representadas pelas colunas com o prefixo cod:
  - cod_curso 
  - cod_turma
  - cod_disciplina
  - cod_aluno
  - cod_professor

  estas chaves são códigos únicos utilizadas também para um possível referenciamento em outra tabela, assumindo o papel de chave estrangeira. No modelo lógico é possível ver as tabelas, suas respectivas chaves e o tipo de dado a ser recebido.

</br>
<img alt="modelo conceitual" width="100%" src="https://github.com/marcelo-souto/modelagem-dados-mysql/blob/main/modelo_logico.jpg?raw=true" />

- Como essas entidades estão relacionadas?        
  *curso* tem *turma*,              
  *turma* possui *disciplina*,            
  *disciplina* possui *professor* que comanda a *turma*,                  
  *aluno* pertence a *turma*.
