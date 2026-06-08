# Firmware original da Creality

A recicladora utiliza a placa principal e o firmware original de uma Ender 3 Pro.
Nao ha firmware customizado gravado na placa nesta versao do projeto.

O codigo-fonte do firmware da Creality nao e disponibilizado neste repositorio.
Este projeto documenta apenas a forma como a placa original foi reaproveitada e
controlada por arquivos G-code especificos.

## Estrategia de controle

Como o firmware permanece original, os parametros necessarios para a recicladora
funcionar sao definidos temporariamente no inicio de cada G-code, localizado em:

```text
codigo/gcode/
```

Isso inclui:

- temperatura do hotend;
- habilitacao dos motores;
- modo de extrusao relativa;
- steps/mm temporario do extrusor;
- limite de velocidade do extrusor;
- aceleracao;
- jerk;
- multiplicador de velocidade.

Essa abordagem permite reaproveitar a placa da Ender 3 Pro sem modificar o
firmware de fabrica. Ao mesmo tempo, mantem os testes mais simples, porque cada
arquivo G-code representa uma condicao de operacao especifica da recicladora.

## Observacao importante

Os comandos usados nos G-codes alteram o comportamento da maquina durante a
execucao, mas nao devem ser tratados como configuracoes permanentes, pois nao
sao salvos com `M500`.
