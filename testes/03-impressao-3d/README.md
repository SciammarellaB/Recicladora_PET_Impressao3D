# Testes de impressão 3D com PET reciclado

Esta etapa documenta os testes realizados na impressora 3D usando o filamento de
PET produzido no projeto.

Depois da prova de conceito manual e da geração dos primeiros trechos de
filamento, o material foi testado na impressora para verificar se poderia ser
usado em uma impressão real. O objetivo inicial não era obter uma peça final
perfeita, mas entender o comportamento do material durante a alimentação,
extrusão e deposição.

## Primeiro teste de impressão

![Vídeo da primeira impressão com filamento PET](../../midia-readme/thumb-primeira-impressao-pet.png)

<a href="https://www.youtube.com/shorts/xxXg9N6lQYA" target="_blank" rel="noopener noreferrer">Assistir no YouTube</a>

Este vídeo registra a primeira vez em que o filamento PET foi usado em uma
impressão 3D. O teste serviu para observar:

- se a impressora conseguiria puxar o filamento;
- se o diâmetro produzido era compatível com o caminho do extrusor;
- se a temperatura de trabalho era suficiente para fundir o PET;
- se seria necessário ajustar fluxo, velocidade ou temperatura;
- quais problemas apareceriam durante a primeira tentativa de impressão.

Algumas peças foram impressas para observar o comportamento do material em
geometrias simples, curvas, engrenagens e peças funcionais.

![Gancho em formato de S impresso com PET reciclado](fotos/gancho-s-pet-reciclado.jpg)

![Engrenagens impressas com PET reciclado](fotos/engrenagens-pet-reciclado.jpg)

## Pontos avaliados

Durante os testes de impressão, os principais pontos de atenção foram:

- aderência inicial do material;
- continuidade da extrusão;
- fusão entre camadas;
- estabilidade do filamento no bico;
- necessidade de aumento do `Flow Ratio`;
- redução do `Max Volumetric Speed`;
- temperatura do hotend;
- temperatura da mesa.

## Teste com PET colorido

![Teste de impressão de Benchy com PET de garrafa colorida](../../midia-readme/thumb-benchy-pet-garrafa-colorida.png)

<a href="https://www.youtube.com/watch?v=Nncd09i17XM" target="_blank" rel="noopener noreferrer">Assistir no YouTube</a>

Este teste utilizou a impressão de um barquinho Benchy para avaliar o
comportamento de garrafas PET coloridas. O objetivo era observar se o material
manteria translucidez após a extrusão e impressão, além de verificar se a cor da
garrafa causaria alguma diferença perceptível no comportamento do filamento.

Durante esse tipo de teste, os pontos de comparação incluem acabamento visual,
transparência/translucidez, aderência entre camadas, estabilidade da extrusão e
regularidade do material depositado.

![Benchy impresso com PET de garrafa colorida](fotos/benchy-pet-garrafa-colorida.jpg)

![Cubo XYZ impresso com PET de garrafa colorida](fotos/cubo-xyz-pet-garrafa-colorida.jpg)

## Peças funcionais

Além das peças de teste, o filamento reciclado foi usado em peças funcionais do
proprio projeto, como suportes e componentes auxiliares da recicladora.

![Suporte do carretel da fita PET impresso com PET reciclado](fotos/suporte-carretel-fita-pet-impresso.jpg)

![Suporte do switch da fita PET montado](fotos/suporte-switch-fita-pet-montado.jpg)

## Relação com os parâmetros de impressão

Como o filamento produzido a partir de fita PET não é totalmente maciço, foi
necessário compensar a quantidade de material no fatiador. Nos testes do projeto,
isso levou ao aumento do fluxo e à redução da velocidade volumétrica máxima para
evitar falta ou excesso de material durante a impressão.

Os parâmetros detalhados estão registrados em:

[parametros](parametros/).
