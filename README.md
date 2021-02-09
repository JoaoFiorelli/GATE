# GATE
Códigos úteis para a simulação da aquisição de imagens de SPECT no pacote GATE.

## BrightView XCT

Para a elaboração da BrightView XCT virtual foi necessário buscar parâmetros físicos da máquina a fim de elaborar uma simulação mais próximo da realidade possível. Essas informações foram obtidas no site da fabricante (Medical Expo, 2019). De posse disso, foi possível construir a geometria da gama câmara para a simulação como descrita abaixo.

Primeiramente foi criada a estrutura chamada SPECThead, que é o conjunto que será responsável pela detecção dos fótons emitidos. Ele possui dimensões de 50 cm por 60 cm, e 10 cm de comprimento. Após isso, nossa atenção foi voltada para o cristal. Ele foi feito de NaI (Iodeto de sódio) com dimensões de 40.6 cm por 53.9 cm, sua espessura é de 0.95 cm (3/8 de polegada). Logo a sua frente colocamos um colimador feito de chumbo. Dentre as várias opções disponíveis para a BrightView escolhemos a low energy high resolution (LEHR), que é mais utilizada pelo setor de medicina nuclear do Hospital das Clínicas de Ribeirão Preto em sua rotina, cuja gama câmara deseja-se simular. Suas cavidades são hexagonais de lado 1.22 mm, a espessura dessa estrutura é de 2.7 cm e a separação entre cada nicho é de 0.152 mm. O resto do SPECThead foi denominado de shielding. Ele foi feito com chumbo, está presente na parte lateral e posterior do SPECThead e tem o papel de blindar fótons espalhados e provenientes de outras regiões que por ventura poderiam ser detectados e assim alterar a contagem. A figura 1 abaixo mostra a geometria final dentro do ambiente do GATE.

### Figure 1- SPECThead BrightView XCT

![SPECThead BrightView XCT](https://github.com/JoaoFiorelli/GATE/blob/master/assets/SPECTheadFINAL.PNG)

## Jaszczak

Para a construção do objeto simulador Jaszczak, realizamos o mesmo processo, procurando suas dimensões através do fabricante (SPECT, 2020). Dentre os quatro modelos disponíveis o reproduzido aqui foi o Deluxe. Este é um cilindro de acrílico de raio externo de 11.12 cm e raio interno de 10.8 cm, sua altura é de 20 cm e tem paredes de espessura de 3.2 mm. Suas estruturas internas são compostas por esferas e pequenos cilíndros, ambos feitos de acrílico. As esferas são seis de diferentes diâmetros dispostas em círculo. Seus diâmetros são: 9.5 mm, 12.7 mm, 15.9 mm, 19.1 mm, 25.4 mm e 31.8 mm. Já os cilindros são dispostos em grupos de mesmo diâmetro em formato triangular (figura 2). Todos possuem a mesma altura de 8.8 cm e o diâmetro dos cilindros de cada grupo são: 4.8 mm, 6.4 mm, 7.9 mm, 9.5 mm, 11.1 mm e 12.7 mm. 

### Figure 2- Jaszczak

![Jaszczak](https://github.com/JoaoFiorelli/GATE/blob/master/assets/jaszczak.PNG)

## Referências

##Autor

LinkedIn: https://www.linkedin.com/in/jo%C3%A3o-pedro-fiorelli-820942124/
