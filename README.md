# DCC905 — Estágio em Docência / Teaching Internship

[Português (PT-BR)](#português-pt-br) | [English (EN-US)](#english-en-us)

---

## Português (PT-BR)

Repositório de apoio às disciplinas **Estágio em Docência I e II** do Programa de Pós-Graduação em Ciência da Computação (PPGCC/DCC/UFMG). Reúne as diretrizes oficiais e **templates LaTeX anonimizados** para a **Proposta de Trabalho** e para o **Relatório Final**, com instruções detalhadas de preenchimento.

### Estrutura do Repositório

```
.
├── 20190802 Disciplina Estagio em Docencia Diretrizes Gerais v2019_2.pdf   # Diretrizes oficiais
├── Template Proposta Estagio/      # Template da Proposta de Trabalho
│   ├── main.tex
│   ├── main.pdf                    # Prévia compilada
│   └── README.md
├── Template Relatorio Final/       # Template do Relatório Final
│   ├── main.tex
│   ├── bibliografia.bib
│   ├── imgs/default/               # Logos institucionais (UFMG e DCC)
│   ├── main.pdf                    # Prévia compilada
│   └── README.md
├── LICENSE                         # Licença MIT
└── README.md                       # Este arquivo
```

### Conteúdo

| Item | Descrição |
|---|---|
| **Diretrizes (PDF)** | Normas gerais do Estágio em Docência: objetivos, condução, proposta, relatório final e critérios de avaliação (proposta: 50 pts; relatório: 50 pts). |
| **Template Proposta Estagio** | Estrutura exigida: 1. Identificação; 2. Sobre a Disciplina (condução, ementa/programa, bibliografia, avaliação); 3. Atividades; 4. Cronograma. |
| **Template Relatorio Final** | Estrutura exigida: 1. Disciplina/turma apoiada; 2. Atividades conduzidas; 3. Resultados obtidos; 4. Autoavaliação; 5. Sugestões para futuras ofertas. |

Os templates **não contêm dados pessoais**: nomes, matrículas, e-mails, disciplina e resultados foram substituídos por campos entre colchetes `[ ... ]`.

### Como Usar os Templates

1. Copie a pasta do template desejado para o seu projeto.
2. No início do `main.tex`, preencha os comandos `\newcommand` (bloco de dados da capa/gerais). Eles são reutilizados automaticamente em todo o documento.
3. Siga as caixas azuis **INSTRUÇÃO** de cada seção e substitua os textos `[ ... ]` pelo seu conteúdo.
4. Ao finalizar, troque `\mostrarinstrucoestrue` por `\mostrarinstrucoesfalse` para ocultar todas as caixas de instrução.
5. Compile o PDF (ver abaixo) e envie pelo Moodle.

#### Compilação

Requer TeX Live ou MiKTeX com os pacotes `babel`, `tcolorbox`, `longtable`, `enumitem`, `hyperref` (e `tikz`/`titling`, conforme o template).

```bash
# Proposta de Trabalho
cd "Template Proposta Estagio"
pdflatex main.tex && pdflatex main.tex

# Relatório Final
cd "Template Relatorio Final"
pdflatex main.tex && bibtex main && pdflatex main.tex && pdflatex main.tex
```

### Fluxo Recomendado do Estágio

1. **Proposta de Trabalho:** acertar previamente com o professor responsável, enviar o PDF pelo Moodle (`NomeCompletoDoAluno.pdf`) e avisar o coordenador da disciplina por e-mail, com o professor em cópia.
2. **Execução:** cumprir as atividades e o cronograma propostos ao longo do semestre.
3. **Relatório Final:** entregar pelo Moodle ao final do semestre; é avaliado pelo professor responsável (cumprimento dos objetivos, qualidade do apoio, disponibilidade e assiduidade, motivação e desenvoltura).

### Boas Práticas

- Use **dados agregados** no relatório (médias, taxas de entrega); nunca cite nomes ou matrículas de alunos (LGPD).
- Mantenha o relatório coerente com a proposta aprovada, justificando eventuais desvios.
- Não versione arquivos temporários de compilação (`.aux`, `.log`, `.out`, `.toc`, `.bbl`, `.blg`).

### Contribuindo

Melhorias aos templates são bem-vindas via *pull request*: faça um fork, crie uma branch, adicione suas alterações e abra o PR descrevendo a mudança. Commits preferencialmente no formato *Conventional Commits* (`docs: ...`, `fix: ...`).

### Licença

Distribuído sob a licença **MIT**. Consulte o arquivo [`LICENSE`](LICENSE) para mais detalhes.

### Referências

- Colegiado do PPGCC/UFMG. *Diretrizes para as Atividades de Estágio em Docência*, 2019.

---

## English (EN-US)

Support repository for the **Teaching Internship I and II (Estágio em Docência I e II)** courses of the Graduate Program in Computer Science (PPGCC/DCC/UFMG). It provides the official guidelines and **anonymized LaTeX templates** for both the **Work Proposal** and the **Final Report**, complete with fill-in instructions.

### Repository Structure

```
.
├── 20190802 Disciplina Estagio em Docencia Diretrizes Gerais v2019_2.pdf   # Official guidelines (PT-BR)
├── Template Proposta Estagio/      # Work Proposal template
│   ├── main.tex
│   ├── main.pdf                    # Compiled preview
│   └── README.md
├── Template Relatorio Final/       # Final Report template
│   ├── main.tex
│   ├── bibliografia.bib
│   ├── imgs/default/               # Institutional logos (UFMG and DCC)
│   ├── main.pdf                    # Compiled preview
│   └── README.md
├── LICENSE                         # MIT License
└── README.md                       # This file
```

### Contents

| Item | Description |
|---|---|
| **Guidelines (PDF)** | General rules for the Teaching Internship: objectives, procedures, work proposal, final report, and grading criteria (proposal: 50 pts; final report: 50 pts). |
| **Template Proposta Estagio** | Required sections: 1. Identification; 2. About the Course (teaching approach, syllabus/program, bibliography, grading); 3. Activities; 4. Schedule. |
| **Template Relatorio Final** | Required sections: 1. Supported course/class; 2. Conducted activities; 3. Achieved results; 4. Self-assessment; 5. Suggestions for future offerings. |

The templates **contain no personal data**: names, student IDs, emails, course details, and results have been replaced with bracketed placeholders `[ ... ]`.

### How to Use the Templates

1. Copy the desired template folder into your working directory.
2. At the top of `main.tex`, fill in the `\newcommand` macros (cover/general data block). They are automatically reused throughout the document.
3. Follow the blue **INSTRUÇÃO** boxes in each section and replace the `[ ... ]` placeholders with your content.
4. When finished, switch `\mostrarinstrucoestrue` to `\mostrarinstrucoesfalse` to hide all instruction boxes.
5. Compile the PDF (see below) and submit it via Moodle.

#### Compilation

Requires TeX Live or MiKTeX with the packages `babel`, `tcolorbox`, `longtable`, `enumitem`, `hyperref` (plus `tikz`/`titling`, depending on the template).

```bash
# Work Proposal
cd "Template Proposta Estagio"
pdflatex main.tex && pdflatex main.tex

# Final Report
cd "Template Relatorio Final"
pdflatex main.tex && bibtex main && pdflatex main.tex && pdflatex main.tex
```

### Recommended Internship Workflow

1. **Work Proposal:** align beforehand with the supervising professor, upload the PDF to Moodle (`StudentFullName.pdf`), and notify the course coordinator by email with the supervising professor copied.
2. **Execution:** carry out the proposed activities and schedule throughout the semester.
3. **Final Report:** submit via Moodle at the end of the semester; it is evaluated by the supervising professor (fulfillment of objectives, quality of support, availability and attendance, motivation, and autonomy).

### Best Practices

- Report only **aggregated data** in the final report (averages, submission rates); never include student names or ID numbers (LGPD privacy compliance).
- Keep the final report consistent with the approved proposal, justifying any deviations.
- Do not commit temporary LaTeX build artifacts (`.aux`, `.log`, `.out`, `.toc`, `.bbl`, `.blg`).

### Contributing

Improvements to the templates are welcome via *pull request*: fork the repository, create a branch, commit your changes, and open a PR describing the update. Prefer *Conventional Commits* (`docs: ...`, `fix: ...`).

### License

Distributed under the **MIT License**. See [`LICENSE`](LICENSE) for details.

### References

- PPGCC/UFMG Graduate Board. *Diretrizes para as Atividades de Estágio em Docência* (Teaching Internship Guidelines), 2019.
