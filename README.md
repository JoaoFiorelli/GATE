# GATE
Códigos úteis para a simulação da aquisição de imagens de SPECT no pacote GATE.

## BrightView XCT

Para a elaboração da BrightView XCT virtual foi necessário buscar parâmetros físicos da máquina a fim de elaborar uma simulação mais próximo da realidade possível. Essas informações foram obtidas no site da fabricante (Medical Expo, 2019). De posse disso, foi possível construir a geometria da gama câmara para a simulação como descrita abaixo.

Primeiramente foi criada a estrutura chamada SPECThead, que é o conjunto que será responsável pela detecção dos fótons emitidos. Ele possui dimensões de 50 cm por 60 cm, e 10 cm de comprimento. Após isso, nossa atenção foi voltada para o cristal. Ele foi feito de NaI (Iodeto de sódio) com dimensões de 40.6 cm por 53.9 cm, sua espessura é de 0.95 cm (3/8 de polegada). Logo a sua frente colocamos um colimador feito de chumbo. Dentre as várias opções disponíveis para a BrightView escolhemos a low energy high resolution (LEHR), que é mais utilizada pelo setor de medicina nuclear do Hospital das Clínicas de Ribeirão Preto em sua rotina, cuja gama câmara deseja-se simular. Suas cavidades são hexagonais de lado 1.22 mm, a espessura dessa estrutura é de 2.7 cm e a separação entre cada nicho é de 0.152 mm. O resto do SPECThead foi denominado de shielding. Ele foi feito com chumbo, está presente na parte lateral e posterior do SPECThead e tem o papel de blindar fótons espalhados e provenientes de outras regiões que por ventura poderiam ser detectados e assim alterar a contagem. A figura 1 abaixo mostra a geometria final dentro do ambiente do GATE.

![SPECThead BrightView XCT](https://github.com/JoaoFiorelli/GATE/tree/master/assets)
