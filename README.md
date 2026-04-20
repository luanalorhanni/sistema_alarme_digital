# Alarme Digital com Memória de Estado (Latch SR)

Projeto desenvolvido na disciplina **EECP 0002 – Circuitos Digitais (2026.1 – T01)** do curso de Engenharia da Computação da **Universidade Federal do Maranhão (UFMA)**.

O projeto consiste na construção de um alarme digital que utiliza um **Latch SR** (implementado com portas lógicas NOR do CI 74LS02) como elemento de memória de estado. O sistema é acionado por um sensor *reed switch* — que simula a abertura de uma porta ou janela — e, ao detectar o evento, mantém o estado de alarme ativo (buzzer + LED) mesmo após o sensor retornar à condição inicial, graças à característica de biestabilidade do latch. O alarme só é desarmado por meio de um *push-button* de reset manual.

## Visão Geral do Circuito

- **Entrada (SET):** Reed switch em configuração NA (Normalmente Aberto) com resistor de pull-down de 10kΩ.
- **Memória de Estado:** Latch SR construído com duas portas NOR do CI 74LS02 em realimentação cruzada.
- **Entrada (RESET):** Push-button com resistor de pull-down de 10kΩ.
- **Saídas:** Buzzer ativo (5V) e LEDs vermelhos com resistores limitadores de 330Ω.
- **Alimentação:** Fonte 5V com chave liga-desliga SPST e capacitor de filtro de 10µF, além de capacitores de desacoplamento de 100nF nos CIs.

## Objetivos

- Aplicar na prática os conceitos de **álgebra booleana** e **circuitos sequenciais** vistos em sala.
- Demonstrar o comportamento de **biestabilidade** e **memória de estado** do Latch SR.
- Projetar, simular e implementar fisicamente um circuito digital funcional.
- Documentar o processo completo seguindo boas práticas de gerenciamento de projeto (PMI/PMBOK®).

## Ferramentas Utilizadas

- **KiCad** — desenho dos esquemáticos elétricos.
- **Logisim Evolution** — simulação lógica do circuito.
- **Proteus** (opcional) — simulação avançada com modelos SPICE.
- **Protoboard + componentes discretos** — montagem do protótipo físico.

## Cronograma Resumido

| Fase | Período | Entrega |
|------|---------|---------|
| 1. Iniciação | 31/03 – 06/04/2026 | TAP aprovado |
| 2. Planejamento | 07/04 – 20/04/2026 | Especificação técnica |
| 3. Projeto dos Esquemáticos | 21/04 – 04/05/2026 | Esquemáticos KiCad |
| 4. Simulação | 05/05 – 18/05/2026 | Simulação validada |
| 5. Implementação Física | 19/05 – 08/06/2026 | Protótipo funcional |
| 6. Documentação | 09/06 – 22/06/2026 | Relatório técnico |
| 7. Encerramento | 23/06 – 30/06/2026 | Apresentação final |

## Estrutura do Repositório

```
.
├── docs/              # TAP, especificação técnica, relatório final
├── schematics/        # Arquivos KiCad e exportações em PDF
├── simulation/        # Arquivos Logisim e Proteus
├── tests/             # Planilhas de testes e resultados
├── media/             # Fotos do protótipo e capturas de simulação
└── README.md
```

## Equipe

- Edna Cristina Durans Santos
- Krislayne Rawane Silva Vieira
- Luana Lorhanni Pacheco Santos
- Lucas Salustriano dos Santos

**Orientador:** Prof. Luiz Henrique Neves Rodrigues

## Referências

- TOCCI, R. J.; WIDMER, N. S.; MOSS, G. L. *Sistemas Digitais: Princípios e Aplicações*.
- FLOYD, T. L. *Sistemas Digitais: Fundamentos e Aplicações*.
- IDOETA, I. V.; CAPUANO, F. G. *Elementos de Eletrônica Digital*.

---

*São Luís – MA · Abril de 2026*
