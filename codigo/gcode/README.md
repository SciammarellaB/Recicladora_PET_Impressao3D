# G-codes da recicladora

Esta pasta deve conter os arquivos G-code usados para operar a recicladora de PET.
Eles controlam o aquecimento do hotend, habilitam os motores e executam a extrusao
continua da fita de PET em blocos, evitando comandos muito longos de extrusao.

A recicladora utiliza a placa principal e o firmware original de uma Ender 3 Pro.
Por esse motivo, os ajustes necessarios para a operacao do equipamento nao sao
gravados como alteracoes permanentes de firmware. As sobrecargas de valores e
parametros sao aplicadas diretamente pelos arquivos G-code durante a execucao.

## Arquivos usados

| Arquivo | Temperatura do bico | Finalidade |
| --- | ---: | --- |
| `PET_230c_20m.gcode` | 230 C | Extrusao de aproximadamente 20 m de material em temperatura mais baixa. |
| `PET_235c_20m.gcode` | 235 C | Extrusao de aproximadamente 20 m de material em temperatura intermediaria. |
| `PET_240c_20m.gcode` | 240 C | Extrusao de aproximadamente 20 m de material em temperatura mais alta. |

## Logica geral dos arquivos

Os tres arquivos seguem a mesma estrutura. A diferenca principal entre eles e a
temperatura configurada para o hotend.

Comandos principais:

- `M104 S...`: define a temperatura do bico.
- `M109 S...`: aguarda o bico atingir a temperatura configurada.
- `M17`: habilita os motores.
- `M83`: configura extrusao relativa.
- `M92 E175`: define temporariamente os steps/mm do extrusor, sem salvar com `M500`.
- `M203 E5`: limita a velocidade maxima do extrusor.
- `M201 E500`: define aceleracao do extrusor.
- `M205 E2`: define jerk do extrusor.
- `M220 S100`: mantem o multiplicador de velocidade em 100%.
- `G1 E190 F125`: executa blocos de extrusao do material.

## Observacoes de uso

- Os arquivos foram criados para uso na recicladora construida a partir de
  componentes reaproveitados de uma Ender 3 Pro original.
- A placa e o firmware permanecem originais; os parametros sao sobrescritos
  temporariamente pelo proprio G-code.
- A selecao entre 230 C, 235 C e 240 C permite testar o comportamento do PET em
  diferentes condicoes de fusao e conformacao.
- Nos testes documentados na monografia, 230 C apresentou a condicao mais
  estavel, com melhor acabamento superficial, aspecto mais cristalino e formato
  dimensional mais uniforme.
- Os blocos repetidos de `G1 E190 F125` ajudam a evitar problemas de firmware
  relacionados a comandos de extrusao muito longos.
- Os ajustes de temperatura e velocidade devem ser acompanhados por medicoes do
  diametro do filamento e observacao visual do acabamento superficial.

## Pendencias para documentacao

Quando os arquivos estiverem no repositorio, registrar tambem:

1. Qual temperatura gerou o filamento mais estavel.
2. Qual temperatura apresentou melhor acabamento visual.
3. Qual temperatura resultou em melhor impressao 3D posteriormente.
4. Em quais condicoes cada arquivo deve ser escolhido.
5. Se houve diferenca perceptivel entre garrafas de marcas, cores ou espessuras
   diferentes.
