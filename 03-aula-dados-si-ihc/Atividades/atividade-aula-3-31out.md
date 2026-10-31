# Aula 3 — Dados, Sistemas de Informação e IHC

**Preparatório ENADE 2026 | UDF**  
**Cursos:** Sistemas de Informação, Ciência da Computação e Análise e Desenvolvimento de Sistemas (ADS)  
**Docente:** Profª Kadidja Valéria  
**Duração:** 60 minutos | **Data:** 31/10/2026

> **Nota:** questões autorais de treinamento, inspiradas em competências da área, não reproduções de itens oficiais do ENADE.

## Objetivos de aprendizagem

1. Interpretar modelos relacionais, consultas e regras de integridade.
2. Relacionar dados, informação, indicadores e decisões organizacionais.
3. Ler tabelas e gráficos criticamente, distinguindo associação e causalidade.
4. Reconhecer princípios de usabilidade e interação humano-computador.
5. Resolver problemas integrando tecnologia, usuário e negócio.

## Método C.A.L.M.A.

| Etapa | Pergunta norteadora |
|---|---|
| **C — Comando** | O que a questão solicita? |
| **A — Assunto** | Qual conhecimento é mobilizado? |
| **L — Leitura** | Quais evidências importam? |
| **M — Marcação** | Quais alternativas podem ser eliminadas? |
| **A — Avaliação** | Minha escolha atende exatamente ao comando? |

## Orientações

**Modalidade:** individual, seguida de discussão coletiva. **Tempo sugerido:** 20 minutos para as questões, mais discussão. **Pontuação:** a definir pela docente.

Em cada item: marque a alternativa e registre a evidência do enunciado que sustenta sua escolha. Use as etapas do C.A.L.M.A.

### Questão 1 — Modelo relacional

Na tabela MATRICULA(id, estudante_id, turma_id, situacao), qual atributo permite relacionar cada matrícula a um estudante?

- A) situacao
- B) estudante_id
- C) id da disciplina
- D) nome do estudante

**Resposta:** ______  **Justificativa:** ________________________________________

### Questão 2 — Integridade

Um estudante já possui matrícula ativa na turma X no período corrente e solicita nova matrícula ativa para a mesma turma. Qual solução atende melhor à regra de negócio?

- A) Aceitar ambas
- B) Excluir a anterior silenciosamente
- C) Bloquear a duplicidade com mensagem clara
- D) Esconder a duplicidade no relatório

**Resposta:** ______  **Justificativa:** ________________________________________

### Questão 3 — Consulta SQL

Considere SELECT turma_id, COUNT(*) FROM matricula WHERE situacao='ativa' GROUP BY turma_id. Qual resultado é produzido?

- A) Nomes de estudantes
- B) Total de matrículas ativas por turma
- C) Média de notas
- D) Matrículas canceladas

**Resposta:** ______  **Justificativa:** ________________________________________

### Questão 4 — Indicador

Uma turma possui 50 ingressantes e 40 concluintes. Qual a taxa de conclusão calculada como concluintes/ingressantes × 100?

- A) 20%
- B) 50%
- C) 80%
- D) 125%

**Resposta:** ______  **Justificativa:** ________________________________________

### Questão 5 — Leitura crítica

Após a implantação de um painel, a média das notas aumentou. Qual afirmação é sustentada apenas por essa observação?

- A) O painel causou o aumento
- B) Houve aumento após a implantação, mas causalidade não foi demonstrada
- C) O painel foi inútil
- D) Todos os estudantes melhoraram

**Resposta:** ______  **Justificativa:** ________________________________________

### Questão 6 — Usabilidade

Ao digitar CPF inválido, o sistema informa o erro junto ao campo e orienta como corrigir. Qual princípio é evidenciado?

- A) Feedback claro
- B) Ocultação do estado
- C) Aumento da complexidade
- D) Ausência de validação

**Resposta:** ______  **Justificativa:** ________________________________________

### Questão 7 — Qualidade de dados

Uma tabela contém vários registros sem data de matrícula, campo obrigatório para o relatório. Qual dimensão da qualidade está comprometida?

- A) Completude
- B) Portabilidade
- C) Estética
- D) Escalabilidade

**Resposta:** ______  **Justificativa:** ________________________________________

### Questão 8 — IHC e decisão

Um painel exibe somente totais, sem período nem definição dos indicadores. Qual melhoria é prioritária?

- A) Trocar apenas as cores
- B) Remover legendas
- C) Informar período, população e definição de cada indicador
- D) Reduzir o contraste

**Resposta:** ______  **Justificativa:** ________________________________________

## Desafio integrador — Painel de matrículas

Uma instituição precisa acompanhar solicitações e matrículas ativas por turma. O sistema não pode registrar duas matrículas ativas do mesmo estudante na mesma turma e período.

**Entregas:**
1. Esboce duas entidades e o relacionamento entre elas.
2. Escreva uma regra de integridade para evitar duplicidade.
3. Defina um indicador, seu numerador, denominador e período.
4. Proponha uma mensagem de erro clara e acessível.
5. Descreva um caso de teste válido e um inválido.

## Registro C.A.L.M.A.

| Questão | Comando | Assunto | Evidência | Alternativas eliminadas | Avaliação final |
|---|---|---|---|---|---|
| 1 | | | | | |
| 2 | | | | | |
| 3 | | | | | |
| 4 | | | | | |
| 5 | | | | | |
| 6 | | | | | |
| 7 | | | | | |
| 8 | | | | | |

## Autoavaliação

- **Verde:** consigo explicar e aplicar.
- **Amarelo:** preciso revisar.
- **Vermelho:** preciso retomar o conteúdo desde o início.

**Meu principal ponto de revisão:** __________________________
