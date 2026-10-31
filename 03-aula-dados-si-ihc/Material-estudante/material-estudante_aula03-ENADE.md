# Aula 3 — Dados, Sistemas de Informação e IHC

**Preparatório ENADE 2026 | UDF**  
**Cursos:** Sistemas de Informação, Ciência da Computação e Análise e Desenvolvimento de Sistemas (ADS)  
**Docente:** Profª Kadidja Valéria  
**Duração:** 60 minutos | **Data:** 31/10/26

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

## 1. Conceitos essenciais

### 1.1 Dados, informação e indicadores

**Dado** é um registro; **informação** é o dado interpretado em contexto; **indicador** é uma medida definida para acompanhamento e comparação. Decisões exigem verificar fonte, período, população, unidade e possíveis limitações.

### 1.2 Banco de dados relacional

- **Entidade/tabela:** conjunto de registros do mesmo tipo.
- **Chave primária (PK):** identifica unicamente um registro.
- **Chave estrangeira (FK):** relaciona registros de tabelas diferentes.
- **Integridade referencial:** impede referências a registros inexistentes.
- **Unicidade:** impede duplicidades segundo a regra definida.
- **Completude e consistência:** asseguram dados obrigatórios e regras uniformes.

Exemplo de modelo:

```text
ESTUDANTE(id PK, nome)
TURMA(id PK, disciplina)
MATRICULA(id PK, estudante_id FK, turma_id FK, situacao)
```

### 1.3 SQL: filtrar, agrupar e contar

```sql
SELECT turma_id, COUNT(*) AS total
FROM matricula
WHERE situacao = 'ativa'
GROUP BY turma_id;
```

A consulta retorna a quantidade de registros de matrícula ativa para cada turma. `WHERE` filtra, `GROUP BY` agrupa e `COUNT(*)` conta registros.

### 1.4 Indicadores e análise crítica

**Taxa de conclusão = concluintes / ingressantes × 100** (definição didática simplificada; em contextos reais, verificar coortes e metodologia). Comparações exigem denominadores equivalentes. Correlação ou sequência temporal **não demonstram causalidade**.

### 1.5 IHC e usabilidade

- **Efetividade:** concluir a tarefa.
- **Eficiência:** recursos e esforço para realizá-la.
- **Satisfação:** percepção da experiência.
- **Feedback:** informar estado, sucesso e erro.
- **Consistência e prevenção de erros:** padrões previsíveis e validações adequadas.

## 2. Exemplo resolvido pelo C.A.L.M.A.

**Situação:** o sistema deve processar solicitações de matrícula pela ordem de chegada.

| Etapa | Aplicação |
|---|---|
| Comando | Identificar a estrutura apropriada. |
| Assunto | Estruturas de dados. |
| Leitura | “Ordem de chegada” é a evidência central. |
| Marcação | Eliminar estruturas que não garantem FIFO. |
| Avaliação | Escolher **fila**, justificando o princípio FIFO. |

## 3. Atividade prática

Resolva as questões propostas no arquivo `atividade-aula-3.md` e registre a justificativa de cada escolha.

## 4. Estudo autônomo

Revise os conceitos, explique uma consulta SQL em palavras e proponha uma melhoria de usabilidade para um sistema acadêmico.

## 5. Referências de apoio

- ELMASRI, R.; NAVATHE, S. B. *Sistemas de Banco de Dados*.
- SILBERSCHATZ, A.; KORTH, H. F.; SUDARSHAN, S. *Sistema de Banco de Dados*.
- PRESSMAN, R. S.; MAXIM, B. R. *Engenharia de Software*.
- ROGERS, Y.; SHARP, H.; PREECE, J. *Design de Interação*.
- ISO 9241-11 — Ergonomia da interação humano-sistema: usabilidade.
