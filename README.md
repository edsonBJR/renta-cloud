# Renta Cloud
Arquitetura para um sistema em nuvem para uma empresa de locação de veículos.

Precisamos propor uma arquitetura para um sistema em nuvem para uma empresa de locação de veículos. 
A empresa em questão aluga automóveis, camionetas de passageiros e camionetas de carga. 
Ele atende a dois mercados, o das pessoas físicas e o das pessoas jurídicas. 
Para acelerar o atendimento, é importante conhecer os dados de clientes que já tenham usado a locadora no passado. Para cada pessoa física necessário conhecer seu nome, sexo, data de nascimento, endereço e CIC (CPF). 
Já para as pessoas jurídicas é necessário conhecer o seu nome, CGC, inscrição estadual e endereço. 
Os clientes são identificados por um código interno a locadora.
A empresa tem uma grande rede de filiais, espalhadas pelo sul do país. 
Em um momento no tempo, um veículo encontra-se sob responsabilidade de uma filial. 
Entretanto, como veículos podem ser alugados para viagens em um sentido somente, eles podem mudar de filial. 
Um veículo é identificado pela sua placa. 
Além disso, é necessário conhecer o número dos chassis, o número do motor, o tipo de veículo e a cor de cada veículo.

O sistema em computador deverá registrar:

a) Os veículos disponíveis em determinada filial na data corrente,
b) As reservas para veículos em uma filial, com previsão de que veículos estarão disponíveis em uma data futura,
c) Os veículos presentemente alugados pela filial, o ponto de entrega (caso seja diferente do de locação) e data de entrega prevista.

Os veículos são classificados por uma tabela de tipos. 
Por exemplo, P3 corresponde a automóveis pequenos, de quatro portas e com ar-condicionado e G4 a grandes automóveis de luxo. 
As reservas não são feitas para uma marca ou modelo de veículo, mas para um tipo de veículo. 
Para tipos de automóveis, os clientes desejam saber o tamanho, classificado em pequeno, médio e grande, o número de passageiros, o número de portas, bem como se possui os seguintes acessórios:

ar-condicionado, 
rádio, 
toca-fitas, 
CD, 
direção hidráulica 
e câmbio automático. 

Para tipos de camionetas de passageiros, as informações são as mesmas que para automóveis. 
Já para tipos de camionetas de carga, as informações acima não são relevantes.
Neste caso, os clientes desejam saber a capacidade de carga da camioneta.
Para cada tipo de veículo, há um determinado número de horas necessário para limpeza e revisão de entrega, entre uma reserva e outra.
Além disso, o sistema deve programar as revisões dos veículos, impedindo que sejam reservados quando há revisões pendentes. 
Esta programação é feita com base em um conjunto de parâmetros que são a quilometragem atual do veículo, a quilometragem média diária de veículo do tipo, bem como em uma tabela de revisões do tipo de veículo.
A seguradora que segura os veículos, exige que, para cada veículo alugado, seja mantida a identificação do motorista, o número de sua habilitação e data de vencimento dela. 
A habilitação não pode vencer dentro do prazo da locação.
