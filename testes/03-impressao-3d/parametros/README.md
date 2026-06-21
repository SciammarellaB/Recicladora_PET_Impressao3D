# Parametros de impressao com PET reciclado

Esta pasta documenta os principais ajustes usados no Orca Slicer para imprimir
com o filamento produzido a partir de garrafas PET.

O filamento reciclado nao se comporta exatamente como um filamento comercial
macico. Por ser formado a partir de uma fita PET dobrada e conformada pelo calor,
o material pode apresentar interior oco, ovalizacao e variacoes dimensionais.
Por isso, os parametros de impressao precisam compensar a diferenca de fluxo,
fusao e estabilidade do material.

## Ajustes principais

| Parametro | Valor/ajuste usado | Motivo |
| --- | --- | --- |
| Temperatura do hotend | Pelo menos 280 °C | Melhorar a fusao entre camadas do PET reciclado. |
| Temperatura da mesa | 70 °C a 80 °C | Melhorar a aderencia inicial, variando conforme o tamanho da peca. |
| Flow Ratio | Aumento aproximado de 25% a 35% | Compensar o interior oco e a menor quantidade efetiva de material depositado. |
| Max Volumetric Speed | Reducao para cerca de 1/3 do valor original | Evitar que a demanda de material exceda a capacidade real de fusao e deposicao. |

## Pontos avaliados nos testes

- aderencia inicial na mesa;
- continuidade da extrusao;
- fusao entre camadas;
- estabilidade do filamento no bico;
- acabamento visual;
- coerencia dimensional das pecas;
- comportamento em modelos de teste como Cubo XYZ e Benchy.

## Observacao

Os valores acima foram obtidos de forma experimental e devem ser tratados como
ponto de partida. Novos lotes de filamento podem exigir ajustes adicionais,
principalmente por diferencas entre garrafas, largura da fita, umidade residual e
regularidade dimensional do filamento produzido.
