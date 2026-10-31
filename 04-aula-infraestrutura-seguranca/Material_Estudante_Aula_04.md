# Aula 04 — Arquitetura, Sistemas Operacionais, Redes e Segurança

**Preparatório ENADE 2026 — UDF**  
**Cursos:** Sistemas de Informação | Ciência da Computação | ADS  
**Professora:** Kadidja Valéria  
**Data:** 07/11/2026 | **Horário:** 11h às 12h | **Duração:** 60 minutos

**Observação:** as questões são **autorais para treinamento**; não são itens oficiais do ENADE.

## Objetivos de aprendizagem

- Relacionar componentes computacionais a sintomas de desempenho.
- Explicar processos, threads, escalonamento e memória virtual.
- Identificar funções de DNS, IP, TCP e HTTPS.
- Aplicar confidencialidade, integridade e disponibilidade a incidentes.
- Selecionar controles e justificar decisões técnicas em questões contextualizadas.

## 1. Arquitetura de computadores

**CPU** executa instruções; **RAM** armazena temporariamente dados e instruções em uso; **armazenamento** mantém dados persistentes; **rede** viabiliza comunicação. Um sistema lento pode ter diferentes causas: CPU saturada, pressão de memória, entrada/saída de disco, gargalo de rede ou problemas na aplicação.

**Exemplo:** CPU próxima de 100% com memória e rede estáveis sugere investigar a carga de processamento, mas não prova a causa definitiva. É necessário medir processos e comportamento da aplicação.

## 2. Sistemas operacionais

- **Processo:** instância de programa em execução, com contexto e recursos.
- **Thread:** fluxo de execução de um processo, compartilhando recursos do processo.
- **Escalonamento:** política que distribui tempo de CPU entre tarefas.
- **Memória virtual:** mecanismo de gerenciamento e isolamento de espaços de endereçamento.
- **Concorrência:** tarefas progridem em períodos sobrepostos; paralelismo exige execução simultânea.

**Armadilha de prova:** processo e thread não são sinônimos; escalonamento não é função do DNS.

## 3. Redes de computadores

| Elemento | Função principal | Exemplo de investigação |
|---|---|---|
| DNS | Resolver nomes para endereços | Funciona por IP, mas falha por nome |
| IP | Endereçamento e encaminhamento | Verificar conectividade e rotas |
| TCP | Transporte confiável e ordenado | Verificar conexão e retransmissões |
| HTTPS/TLS | Proteger comunicação HTTP em trânsito | Verificar certificado e configuração |

**Importante:** HTTPS protege a comunicação em trânsito, mas não garante, sozinho, que o sistema seja seguro contra todas as ameaças.

## 4. Segurança da informação

A **tríade CIA** reúne:
- **Confidencialidade:** apenas pessoas autorizadas acessam os dados.
- **Integridade:** dados não são alterados de modo indevido.
- **Disponibilidade:** sistemas e dados estão acessíveis quando necessários.

**Controles:** autenticação multifator (MFA), privilégio mínimo, atualizações, monitoramento, backups com testes de restauração e procedimentos de resposta a incidentes.

**Exemplos:** vazamento de dados afeta confidencialidade; alteração indevida de notas afeta integridade; queda do portal afeta disponibilidade. Um incidente pode comprometer mais de uma propriedade.

## 5. Como analisar uma questão contextualizada

1. Leia o comando antes de procurar a alternativa.
2. Destaque evidências observáveis do cenário.
3. Associe cada evidência à camada correta: hardware, SO, rede, aplicação ou segurança.
4. Elimine alternativas incompatíveis.
5. Confirme que a resposta resolve o problema apresentado, sem extrapolar dados.

## Método C.A.L.M.A.

| Etapa | Pergunta |
|---|---|
| **C — Comando** | O que a questão pede? |
| **A — Assunto** | Qual conceito devo usar? |
| **L — Leitura** | Quais dados do enunciado são relevantes? |
| **M — Marcação** | Que alternativas posso eliminar? |
| **A — Avaliação** | Minha resposta atende exatamente ao comando? |

## 6. Atividade e estudo autônomo

Resolva as questões do arquivo de atividade e registre justificativas. No desafio integrador, elabore um plano de diagnóstico e proteção do portal acadêmico.

### Checklist de revisão

- [ ] Diferencio CPU, RAM, armazenamento e rede.
- [ ] Explico processos, threads e escalonamento.
- [ ] Identifico DNS, IP, TCP e HTTPS.
- [ ] Distingo confidencialidade, integridade e disponibilidade.
- [ ] Sei justificar MFA, privilégio mínimo e backup testado.
- [ ] Aplico as cinco etapas do C.A.L.M.A.

## Referências bibliográficas de apoio

- STALLINGS, William. *Arquitetura e Organização de Computadores*.
- TANENBAUM, Andrew S.; BOS, Herbert. *Sistemas Operacionais Modernos*.
- KUROSE, James F.; ROSS, Keith W. *Redes de Computadores e a Internet*.
- STALLINGS, William; BROWN, Lawrie. *Segurança de Computadores: Princípios e Práticas*.
- ISO/IEC 27001 — Sistemas de gestão da segurança da informação.
