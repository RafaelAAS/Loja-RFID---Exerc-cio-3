# Loja RFID-Exercício 3

# Loja Autônoma RFID — Backlog de User Stories

> Repositório criado para a [DISCIPLINA 4] - Gestão de projetos de RFID.  
> Contém as histórias de usuário e critérios de aceitação para os principais problemas de uma loja autônoma com tecnologia RFID.

---

## Sobre o Projeto

Este repositório documenta o backlog de um sistema de **checkout autônomo baseado em RFID** (Radio-Frequency Identification). O objetivo é identificar problemas críticos de leitura de etiquetas e propor soluções estruturadas no formato de **User Stories**, seguindo as boas práticas de Product Ownership ágil.

---

## Problemas Mapeados

| # | Problema | Causa Raiz |
|---|----------|------------|
| 1 | **Duplicidade** — sistema registra múltiplos itens iguais | Antena faz várias leituras/segundo da mesma etiqueta |
| 2 | **Interferência** — sistema não lê itens em sacolas metálicas | Metal e papel-alumínio bloqueiam ondas de rádio (RFID passivo) |
| 3 | **Leitura Indesejada** — sistema cobra itens ainda na prateleira | Ganho/potência da antena muito elevado |
| 4 | **Conflito de Tráfego** — sistema trava com muitos clientes simultâneos | Colisão de sinais de rádio (anticolisão) |

---

## User Stories (Issues)

As histórias de usuário estão cadastradas como **Issues** neste repositório com a label `feature`.

| Issue | Título | Persona | Story Points |
|-------|--------|---------|:------------:|
| [#1](../../issues/1) | Filtro de deduplicação de leituras RFID | Financeiro da loja | 3 pts |
| [#2](../../issues/2) | Alerta de exceção para bloqueio de leitura RFID | Gerente da loja | 8 pts |
| [#3](../../issues/3) | Calibração de limiar de potência RSSI da antena | Analista de Infraestrutura | 5 pts |
| [#4](../../issues/4) | Configuração de protocolo de anticolisão RFID | Analista de Infraestrutura | 13 pts |

---

## Estrutura do Backlog

```
Total: 29 Story Points

[===........] #1 Filtro de Deduplicação    — 3 pts  (~1,5 dias)
[========...] #2 Alerta de Exceção         — 8 pts  (~2,5 dias)
[=====......] #3 Calibração de RSSI        — 5 pts  (~2,0 dias)
[=============] #4 Algoritmo de Anticolisão — 13 pts (~4,0 dias)
```

---

## Formato das User Stories

Cada issue segue o padrão:

```
Como [persona],
quero [funcionalidade],
para que [benefício/resultado esperado].
```

Acompanhado de **Critérios de Aceitação** no formato de checklist, garantindo rastreabilidade e validação objetiva de cada entrega.

---

## Tecnologias Envolvidas

- **RFID Passivo** — leitura de etiquetas sem bateria via campo eletromagnético
- **Sensor Infravermelho** — detecção de presença no portal de saída
- **RSSI (Received Signal Strength Indicator)** — métrica de intensidade do sinal de rádio
- **Protocolo de Anticolisão** — algoritmo para leitura simultânea de múltiplas etiquetas

---

## Autor

Desenvolvido como atividade prática da [DISCIPLINA 4] - Gestão de projetos de RFID.  
Foco em práticas ágeis: escrita de User Stories, critérios de aceitação e gestão de backlog no GitHub.
