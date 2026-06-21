# Modelos 3D

Esta pasta reune os arquivos e referencias das pecas impressas em 3D usadas na
construcao da recicladora de PET.

As pecas foram modeladas no Tinkercad e impressas para compor a estrutura,
fixacao, tracao e bobinamento do equipamento.

## Imagens de referencia

![Visao geral das pecas no Tinkercad](imagens/visao-geral-pecas-tinkercad.png)

![Lista das pecas impressas em 3D](imagens/lista-pecas-impressas-3d.png)

## Lista de pecas impressas

Os arquivos STL ficam todos juntos em [`stl/`](stl/) para facilitar o download e
a impressao das pecas.

| Nº | Peca | Arquivo STL | Quantidade | Observacao |
| ---: | --- | --- | ---: | --- |
| 1 | Suporte do motor NEMA | [`stl/suporte-motor-nema17.stl`](stl/suporte-motor-nema17.stl) | 1x | Suporte estrutural para fixacao do motor NEMA. |
| 2 | Trava do filamento | [`stl/trava-filamento.stl`](stl/trava-filamento.stl) | 1x | Peca de apoio/travamento do caminho do material. |
| 3 | Engrenagem do motor NEMA 17 | [`stl/engrenagem-motor-nema17.stl`](stl/engrenagem-motor-nema17.stl) | 1x | Peca em cinza impressa com PET reciclado apos quebras nas primeiras versoes em PLA. |
| 4 | Arruelas adaptadoras | [`stl/arruela-adaptadora.stl`](stl/arruela-adaptadora.stl) | 2x | Arruelas para ajuste e adaptacao mecanica do conjunto. |
| 5 | Engrenagem do carretel | [`stl/engrenagem-carretel.stl`](stl/engrenagem-carretel.stl) | 1x | Engrenagem grande do sistema de movimentacao do carretel. |
| 6 | Espacador fino | [`stl/espacador-fino.stl`](stl/espacador-fino.stl) | 1x | Espacador para alinhamento do conjunto. |
| 7 | Suporte do carretel bobinador | [`stl/suporte-carretel-bobinador.stl`](stl/suporte-carretel-bobinador.stl) | 1x | Suporte estrutural do carretel que enrola o filamento produzido. |
| 8 | Suporte do carretel da fita PET | [`stl/suporte-carretel-fita-pet.stl`](stl/suporte-carretel-fita-pet.stl) | 1x | Suporte do carretel que armazena/alimenta a fita PET antes da extrusao. |
| 9 | Espacador largo | [`stl/espacador-largo.stl`](stl/espacador-largo.stl) | 1x | Espacador maior para alinhamento do conjunto. |

## Observacao sobre material

As pecas em cinza foram impressas com PET reciclado. As primeiras versoes em PLA
apresentaram quebras durante o funcionamento, entao o PET reciclado foi utilizado
nas pecas que exigiam maior resistencia mecanica para suportar o esforco da
maquina.

## Organizacao dos arquivos

- `stl/`: arquivos prontos para impressao, reunidos em uma unica pasta.
- `fatiamento/`: arquivos `.3mf`, perfis ou configuracoes de slicer.
- `imagens/`: capturas e pranchas explicativas das pecas.

## Observacao sobre arquivos editaveis

Os arquivos CAD/editaveis dos modelos nao serao disponibilizados neste repositorio.
Para reproducao do projeto, serao fornecidos apenas os arquivos STL das pecas
necessarias para impressao.

As imagens do Tinkercad ficam como referencia visual para identificar as pecas,
entender o conjunto e conferir quantidades.
