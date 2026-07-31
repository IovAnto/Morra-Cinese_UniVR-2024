# Morra cinese — FSMD

Elaborato del corso di Architettura degli Elaboratori, Università di Verona, 2023/2024.

Il gioco della morra cinese realizzato come FSMD, prima descritto in SystemVerilog e poi
portato a livello di porte logiche in SiS. La relazione confronta la rete non ottimizzata
con quella ottimizzata dopo il mapping.

## Struttura

```
SRC/
├── verilog/     design.sv, testbench.sv e l'output della simulazione
└── sis/         FSMD.blif, script di test e output SiS
Relazione/       relazione LaTeX con schemi e confronto ottimizzato / non ottimizzato
SIS2024.pdf      traccia del progetto
```

## Simulazione

Verilog, con Icarus:

```bash
iverilog -o morra SRC/verilog/design.sv SRC/verilog/testbench.sv
vvp morra
```

SiS, dalla shell del tool:

```
source SRC/sis/testbench.script
```

## Autori

Antonio Iovine e Tommi Bimbato.

## Licenza

Il codice e la relazione restano di proprietà degli autori. L'uso, la modifica e la
distribuzione sono consentiti citando la fonte.
