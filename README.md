# Mackenzie - Objetos Inteligentes Conectados - Sensor de estoque 

- O objetivo do projeto é o desenvolvimento de um protótipo em um controlador cm a IDE Arduino 2.3.3, que deve automatizar o controle de estoque, assegurando que todos os itens estejam disponíveis.

- Quando um item está em falta, o sensor calcula a distância até o produto e devido a variável proposta para distância mínima até o produto, é possível reconhecer se o produto existe ou não, de forma que o controlador junto a conexão MQTT envia uma mensagem para o dispositivo móvel do individual, garantindo que a informação chegue rapidamente aos responsáveis pela reposição.
  
**Os materiais e métodos escolhidos:


•	Controlador: O modelo ESP32 é altamente recomendado, pois já possui 
conectividade Wi-Fi integrada.

•	Sensor: O sensor de distância será o HCSR04 para detectar padrões e movimentações de retirada de itens.

•	Broker MQTT: Um servidor MQTT para comunicação, que pode ser configurado localmente ou usar um serviço online. Nesse caso será utilizado o Broker EMQX.

•	Biblioteca PubSubClient: Para a comunicação via MQTT no controlador, Biblioteca Wifi para conexão com a rede, Biblioteca do ESP32.
Para o projeto, será utilizado o app MQTT Dashboard, que é uma ferramenta para testar e monitorar dispositivos IoT que utilizam do protocolo. Dessa forma, ele possibilita a visualização e publicação dos dados enviados e interage com o modelo do controlador escolhido (ESP32) diretamente do celular.
Para a programação, usaremos a IDE 2.3.3 do controlador juntamente com a linguagem de programação C++. Dessa forma, acessando o site oficial do mesmo, fazendo a
instalação e configurando a ESP32 na IDE 2.3.3, podemos iniciar o processo de programação do prototipo.

**Construção:

O sensor utilizado foi o HCSR04 que é conectado ao microcontrolador ESP32, que irá processar os dados do estoque. Os cabos de alimentação do sensor são conectados às entradas de 5V e GND do ESP32, enquanto o sinal de saída do sensor é conectado ao pino digital 14 e 25 (Trigger e Echo). Este sistema é alimentado por uma fonte de 5V, adequada para a operação dos componentes eletrônicos envolvidos. Também há a possibilidade de alimentar todo o circuito através de um cabo USB direto de um computador.

![WhatsApp Image 2024-11-18 at 7 42 08 PM](https://github.com/user-attachments/assets/b15e495c-731d-48e3-a4ca-2828edd62ab9)


a




