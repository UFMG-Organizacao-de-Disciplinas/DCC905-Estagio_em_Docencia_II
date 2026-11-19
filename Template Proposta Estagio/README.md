# Template de Proposta de Trabalho — Estágio em Docência (PPGCC/DCC/UFMG)
# Work Proposal Template — Teaching Internship (PPGCC/DCC/UFMG)

[Português (PT-BR)](#português-pt-br) | [English (EN-US)](#english-en-us)

---

## Português (PT-BR)

Template LaTeX baseado na estrutura exigida pelas *Diretrizes para as Atividades de Estágio em Docência* (Proposta de trabalho: 1. Identificação; 2. Sobre a Disciplina; 3. Atividades; 4. Cronograma). Não contém dados pessoais: todo conteúdo variável está entre colchetes `[ ... ]`.

### Conteúdo do Pacote

| Arquivo | Função |
|---|---|
| `main.tex` | Documento principal (identificação, sobre a disciplina, atividades, cronograma, considerações finais e assinaturas) |
| `README.md` | Este guia (PT-BR / EN-US) |
| `main.pdf` | Prévia do template compilado |

### Como Preencher

1. **Dados gerais:** edite os comandos `\newcommand` no início de `main.tex` (bloco *DADOS GERAIS*): estagiário, estágio (I ou II), disciplina, código, turma, horários, semestre e professor. Eles são reutilizados no título, na identificação, nas considerações finais e nas assinaturas.
2. **Seções:** cada seção possui uma caixa azul **INSTRUÇÃO** explicando o que escrever. Substitua os textos `[ ... ]`; adicione ou remova linhas das tabelas, listas e do cronograma conforme necessário.
3. **Ocultar instruções:** ao finalizar, troque `\mostrarinstrucoestrue` por `\mostrarinstrucoesfalse`.
4. **Alinhamento prévio:** a proposta deve ser acertada com o professor responsável antes da submissão.
5. **Entrega:** envie o PDF pelo Moodle (nome do arquivo: `NomeCompletoDoAluno.pdf`) e informe o coordenador da disciplina por e-mail, com o professor responsável em cópia.
6. **Coerência:** o Relatório Final deve prestar contas das atividades e do cronograma aqui propostos.

### Compilação

```bash
pdflatex main.tex
pdflatex main.tex   # segunda passada para ajustar a tabela longa (longtable)
```

Requer TeX Live (ou MiKTeX) com os pacotes `babel`, `tcolorbox`, `longtable`, `titling`, `enumitem`, `hyperref`.

---

## English (EN-US)

LaTeX template following the structure required by the *Teaching Internship Guidelines* (*Diretrizes para as Atividades de Estágio em Docência* — Work Proposal: 1. Identification; 2. About the Course; 3. Activities; 4. Schedule). It contains no personal data: all variable fields are enclosed in brackets `[ ... ]`.

### Package Contents

| File | Purpose |
|---|---|
| `main.tex` | Main document (identification, course overview, activities, schedule, final remarks, and signatures) |
| `README.md` | This guide (PT-BR / EN-US) |
| `main.pdf` | Compiled template preview |

### How to Fill In

1. **General data:** edit the `\newcommand` macros at the top of `main.tex` (*DADOS GERAIS* block): intern name, internship level (I or II), course name, course code, class code, schedule, semester, and supervising professor. These values are automatically reused in the title, identification section, final remarks, and signature blocks.
2. **Sections:** each section includes a blue **INSTRUÇÃO** box explaining what to write. Replace the `[ ... ]` placeholders and add or remove table rows, list items, and schedule entries as needed.
3. **Hide instructions:** once completed, change `\mostrarinstrucoestrue` to `\mostrarinstrucoesfalse` to remove all instruction boxes from the compiled PDF.
4. **Prior alignment:** the proposal must be agreed upon with the supervising professor before submission.
5. **Submission:** upload the compiled PDF to Moodle (named `StudentFullName.pdf`) and notify the course coordinator by email with the supervising professor copied.
6. **Consistency:** the Final Report must account for the activities and schedule proposed in this document.

### Compilation

```bash
pdflatex main.tex
pdflatex main.tex   # second pass required for longtable alignment
```

Requires TeX Live (or MiKTeX) with the packages `babel`, `tcolorbox`, `longtable`, `titling`, `enumitem`, `hyperref`.
