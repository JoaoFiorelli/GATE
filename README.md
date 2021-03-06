#### English version:

# GATE
Useful codes for simulating the acquisition of SPECT images in the GATE package.

## BrightView XCT

For the preparation of the virtual BrightView XCT it was necessary to search for physical parameters of the machine in order to elaborate a simulation as close to the possible reality. This information was obtained from the manufacturer's website (Medical Expo, 2019). With this in mind, it was possible to construct the geometry of the camera range for the simulation as described below.

First, a structure called SPECThead was created, which is the set that will be responsible for detecting the emitted photons. It has dimensions of 50 cm by 60 cm, and 10 cm in length. After that, our attention was turned to the crystal. It was made of NaI (sodium iodide) with dimensions of 40.6 cm by 53.9 cm, its thickness is 0.95 cm (3/8 inch). Right in front of you we put a collimator made of lead. Among the various options available to BrightView, we chose the low energy high resolution (LEHR), which is most used by the nuclear medicine sector of the Hospital das Clínicas in Ribeirão Preto in its routine, whose camera range is intended to be simulated. Its cavities are hexagonal with 1.22 mm sides, the thickness of this structure is 2.7 cm and the separation between each niche is 0.152 mm. The rest of SPECThead was called shielding. It was made with lead, is present on the side and back of the SPECThead and has the role of shielding scattered photons from other regions that could be detected and thus change the count. Figure 1 below shows the final geometry within the GATE environment.

## Jaszczak

For the construction of the Jaszczak simulator object, we performed the same process, looking for its dimensions through the manufacturer (SPECT, 2020). Among the four models available, the one reproduced here was the Deluxe. This is an acrylic cylinder with an external radius of 11.12 cm and an internal radius of 10.8 cm, its height is 20 cm and has walls with a thickness of 3.2 mm. Its internal structures are composed of spheres and small cylinders, both made of acrylic. The spheres are six of different diameters arranged in a circle. Their diameters are: 9.5 mm, 12.7 mm, 15.9 mm, 19.1 mm, 25.4 mm and 31.8 mm. The cylinders are arranged in groups of the same diameter in a triangular shape (figure 2). All have the same height of 8.8 cm and the diameter of the cylinders of each group are: 4.8 mm, 6.4 mm, 7.9 mm, 9.5 mm, 11.1 mm and 12.7 mm.

#### Versão em Português:

# GATE
Códigos úteis para a simulação da aquisição de imagens de SPECT no pacote GATE.

## BrightView XCT

Para a elaboração da BrightView XCT virtual foi necessário buscar parâmetros físicos da máquina a fim de elaborar uma simulação mais próximo da realidade possível. Essas informações foram obtidas no site da fabricante (Medical Expo, 2019). De posse disso, foi possível construir a geometria da gama câmara para a simulação como descrita abaixo.

Primeiramente foi criada a estrutura chamada SPECThead, que é o conjunto que será responsável pela detecção dos fótons emitidos. Ele possui dimensões de 50 cm por 60 cm, e 10 cm de comprimento. Após isso, nossa atenção foi voltada para o cristal. Ele foi feito de NaI (Iodeto de sódio) com dimensões de 40.6 cm por 53.9 cm, sua espessura é de 0.95 cm (3/8 de polegada). Logo a sua frente colocamos um colimador feito de chumbo. Dentre as várias opções disponíveis para a BrightView escolhemos a low energy high resolution (LEHR), que é mais utilizada pelo setor de medicina nuclear do Hospital das Clínicas de Ribeirão Preto em sua rotina, cuja gama câmara deseja-se simular. Suas cavidades são hexagonais de lado 1.22 mm, a espessura dessa estrutura é de 2.7 cm e a separação entre cada nicho é de 0.152 mm. O resto do SPECThead foi denominado de shielding. Ele foi feito com chumbo, está presente na parte lateral e posterior do SPECThead e tem o papel de blindar fótons espalhados e provenientes de outras regiões que por ventura poderiam ser detectados e assim alterar a contagem. A figura 1 abaixo mostra a geometria final dentro do ambiente do GATE.

## Jaszczak

Para a construção do objeto simulador Jaszczak, realizamos o mesmo processo, procurando suas dimensões através do fabricante (SPECT, 2020). Dentre os quatro modelos disponíveis o reproduzido aqui foi o Deluxe. Este é um cilindro de acrílico de raio externo de 11.12 cm e raio interno de 10.8 cm, sua altura é de 20 cm e tem paredes de espessura de 3.2 mm. Suas estruturas internas são compostas por esferas e pequenos cilíndros, ambos feitos de acrílico. As esferas são seis de diferentes diâmetros dispostas em círculo. Seus diâmetros são: 9.5 mm, 12.7 mm, 15.9 mm, 19.1 mm, 25.4 mm e 31.8 mm. Já os cilindros são dispostos em grupos de mesmo diâmetro em formato triangular (figura 2). Todos possuem a mesma altura de 8.8 cm e o diâmetro dos cilindros de cada grupo são: 4.8 mm, 6.4 mm, 7.9 mm, 9.5 mm, 11.1 mm e 12.7 mm. 

#### Figure 1- SPECThead BrightView XCT

![SPECThead BrightView XCT](https://github.com/JoaoFiorelli/GATE/blob/master/assets/SPECTheadFINAL.PNG)

#### Figure 2- Jaszczak

![Jaszczak](https://github.com/JoaoFiorelli/GATE/blob/master/assets/jaszczak.PNG)

## References/Referências

Medical Expo (2019). http://pdf.medicalexpo.com/pdf/philips-healthcare/brightview-x-xct/70721-170301-2.html; 15 de Julho de 2019:

SPECT (2020). http://www.spect.com/pub/Flanged_Jaszczak_Phantoms.pdf, 26 de Março de 2020.

## Author/Autor

LinkedIn: [João Pedro Fiorelli](https://www.linkedin.com/in/jo%C3%A3o-pedro-fiorelli-820942124/)
