Este projeto faz parte da playlist 'Curso de Modelagem de Dados', disponibilizada pelo canal do Youtube 'Bóson Treinamentos'. 
Link da playlist: https://youtube.com/playlist?list=PLucm8g_ezqNoNHU8tjVeHmRGBFnjDIlxD&si=ADM9iZyLToLK6FBN

DESCRIÇÃO BÁSICA
Este projeto simula um banco de dados usado para o gerenciamento de uma faculdade.

OBJETIVOS DO BANCO DE DADOS
- Realizar controle centralizado de alunos, professores, cursos, disciplinas, histórico escolar e turmas.

FASES DO PROJETO
- Levantamento de Requisitos
- Identificação de Entidades e Relacionamentos
- Modelo Entidade-Relacionamento
- Diagrama Entidade-Relacionamento
- Dicionário de Dados
- Normalização
- Implementação
- Testes Básicos (Consultas)

REGRAS DO NEGÓCIO
- Um aluno só pode estar matriculado em um curso por vez;
- Alunos possuem um código de identificação (RA);
- Cursos são compostos por disciplinas;
- Cada disciplina terá mo máximo 30 alunos por turma;
- As disciplinas podem ser obrigatórias ou optativas, dependendo do curso;
- As disciplinas pertencem a departamentos específicos;
- Cada disciplina possui um código de identificação;
- Alunos podem trancar matrícula, não estando então matriculados em nenhuma disciplina no semestre;
- Em cada semestre, cada aluno pode se matricular em no máximo 9 disciplinas;
- O aluno só pode ser reprovado no máximo 3 vezes na mesma disciplina;
- A faculdade terá no máximo 3.000 alunos matriculados simultaneamente, em 10 cursos distintos;
- Entram 300 alunos novos por ano;
- Existem 90 disciplinas no total disponíveis;
- Um Histórico Escolar traz todas as disciplinas cursadas por um aluno, incluindo nota final, frequencia e período do curso realizado;
- Professores podem ser cadastrados mesmo sem lecionar disciplinas;
- Existem 40 professores trabalhando na escola;
- Cada professor é vinculado a um departamento;
- Professores são identificados por um código de professor.

IDENTIFICAÇÃO DE ENTIDADES
- Aluno
- Professor
- Disciplina
- Curso
- Departamento
- Turma

IDENTIFICANDO RELACIONAMENTOS
Nesse ponto verificou-se a partir das regras do negócio quais entidades relacionam-se com outras. Foram identificados os seguintes relacionamentos:
- Aluno está matriculado em curso;
- Aluno cursa discipina;
- Aluno realizou disciplina;
- Aluno integra turma;
- Professor vinculado a departamento;
- Professor ministra disciplina;
- Disciplina pertece a departamento;

Durante o processo de modelagem algumas informações podem surgir que estivessem presentes nas regras de negócio. No caso da faculdade, é possível levantar alguns relacionamentos que não seriam depreendidos a partir das regras de negócios iniciais. São eles:
- Departamento controla curso;
- Disciplina depende de disciplina.

IDENTIFICANDO ATRIBUTOS