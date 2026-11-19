# Template de Relatório Final — Estágio em Docência (PPGCC/DCC/UFMG)
# Final Report Template — Teaching Internship (PPGCC/DCC/UFMG)

[Português (PT-BR)](#português-pt-br) | [English (EN-US)](#english-en-us)

---

## Português (PT-BR)

Template LaTeX baseado na estrutura exigida pelas *Diretrizes para as Atividades de Estágio em Docência* (Relatório final: 1. Disciplina/turma apoiada; 2. Atividades conduzidas; 3. Resultados obtidos; 4. Autoavaliação; 5. Sugestões para futuras ofertas). Não contém dados pessoais: todo conteúdo variável está entre colchetes `[ ... ]`.

### Conteúdo do Pacote

| Arquivo | Função |
|---|---|
| `main.tex` | Documento principal (capa, resumo, seções 1–5, considerações finais e assinaturas) |
| `bibliografia.bib` | Referências BibTeX (substituir os exemplos) |
| `imgs/default/` | Logos institucionais (UFMG e DCC) usados na capa |
| `README.md` | Este guia (PT-BR / EN-US) |
| `main.pdf` | Prévia do template compilado |

### Como Preencher

1. **Capa:** edite os comandos `\newcommand` no início de `main.tex` (bloco *DADOS DA CAPA*): semestre, disciplina, código, turma, professor, estagiário, matrícula, e-mails, local/data. Eles são reutilizados automaticamente na capa e nas assinaturas.
2. **Seções:** cada seção possui uma caixa azul **INSTRUÇÃO** explicando o que escrever. Substitua os textos `[ ... ]` pelo seu conteúdo; adicione ou remova linhas de tabelas e itens conforme necessário.
3. **Ocultar instruções:** ao finalizar, troque `\mostrarinstrucoestrue` por `\mostrarinstrucoesfalse` (logo após a definição das caixas). Todas as caixas desaparecem do PDF.
4. **Referências:** cadastre as obras em `bibliografia.bib` e cite com `\cite{chave}`.
5. **Privacidade (LGPD):** em *Resultados*, use apenas dados agregados; não cite nomes nem matrículas de alunos.
6. **Conferência:** o relatório deve refletir a Proposta de Trabalho aprovada e é avaliado pelo professor supervisor (cumprimento dos objetivos, qualidade do apoio, disponibilidade e assiduidade, motivação e desenvoltura). Envie o PDF final pelo Moodle.

### Compilação

```bash
pdflatex main.tex
bibtex main
pdflatex main.tex
pdflatex main.tex
```

Requer TeX Live (ou MiKTeX) com os pacotes `babel`, `tikz`, `tcolorbox`, `longtable`, `enumitem`, `hyperref`.

---

## English (EN-US)

LaTeX template following the structure required by the *Teaching Internship Guidelines* (*Diretrizes para as Atividades de Estágio em Docência* — Final Report: 1. Supported course/class; 2. Conducted activities; 3. Achieved results; 4. Self-assessment; 5. Suggestions for future offerings). It contains no personal data: all variable fields are enclosed in brackets `[ ... ]`.

### Package Contents

| File | Purpose |
|---|---|
| `main.tex` | Main document (cover page, abstract, sections 1–5, final remarks, and signatures) |
| `bibliografia.bib` | BibTeX references (replace the placeholder entries) |
| `imgs/default/` | Institutional logos (UFMG and DCC) used on the cover page |
| `README.md` | This guide (PT-BR / EN-US) |
| `main.pdf` | Compiled template preview |

### How to Fill In

1. **Cover page:** edit the `\newcommand` macros at the top of `main.tex` (*DADOS DA CAPA* block): semester, course name, course code, class code, supervising professor, intern name, student ID, emails, and location/date. They are automatically reused on the cover page and signature blocks.
2. **Sections:** each section includes a blue **INSTRUÇÃO** box explaining what to write. Replace the `[ ... ]` placeholders with your content; add or remove table rows and list items as needed.
3. **Hide instructions:** once completed, switch `\mostrarinstrucoestrue` to `\mostrarinstrucoesfalse` (right after the box definition). All instruction boxes will disappear from the compiled PDF.
4. **References:** add your bibliography entries to `bibliografia.bib` and cite them using `\cite{key}`.
5. **Privacy (LGPD):** in the *Results* section, report only aggregated metrics; never include student names or ID numbers.
6. **Review & Submission:** the final report must reflect the approved Work Proposal and is evaluated by the supervising professor (fulfillment of objectives, quality of support, availability and attendance, motivation, and autonomy). Submit the final PDF via Moodle.

### Compilation

```bash
pdflatex main.tex
bibtex main
pdflatex main.tex
pdflatex main.tex
```

Requires TeX Live (or MiKTeX) with the packages `babel`, `tikz`, `tcolorbox`, `longtable`, `enumitem`, `hyperref`.
