# Pacote PKG_DISCIPLINA

## Descrição
O pacote `PKG_DISCIPLINA` contém um conjunto de procedures e cursores que implementam operações relacionadas à entidade Disciplina. Este pacote permite o cadastro de disciplinas, a contagem de alunos por disciplina, o cálculo da média de idade dos alunos matriculados em uma disciplina e a listagem de alunos de uma disciplina específica.

## Procedures e Cursores

### Procedure de Cadastro de Disciplina
**Nome:** `CADASTRAR_DISCIPLINA`

**Descrição:** 
Cadastra uma nova disciplina na tabela de disciplinas.

**Parâmetros:**
- `P_NOME` (VARCHAR2): Nome da disciplina.
- `P_DESCRICAO` (VARCHAR2): Descrição da disciplina.
- `P_CARGA_HORARIA` (NUMBER): Carga horária da disciplina.

**Exemplo de Uso:**
```sql
BEGIN
  PKG_DISCIPLINA.CADASTRAR_DISCIPLINA('Matemática', 'Matemática Básica', 60);
END;
/
