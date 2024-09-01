##### Motivação para o uso de Redes
- **Aplicações comerciais**: 
	- Compartilhamento de recursos com o objetivo de tornar todos os programas, equipamentos e especialmente dados ao alcance de todas os usuários na rede, independente da localização física do recurso e do usuário.
	- Meio de comunicação. Ganho de agilidade na comunicação. 
	- Economia. Mainframes são caros.
- **Aplicações domésticas**: 
	1. Acesso a informações remotas.
	2. Comunicação entre pessoas.
	3. Entretenimento interativo.
	4. Comércio Eletrônico.

##### Protocolo de redes
- Protocolo define o formato e a ordem das mensagens trocadas entre duas ou mais entidades comunicantes, bem como as ações realizadas na transmissão e/ou no recebimento de uma mensagem ou outro evento.

##### Classificação de Redes
- **Redes Confinadas**: Redes são ditas confinadas quando as distâncias entre os módulos processadores são menores que alguns poucos metros.
- **Redes Locais**: Cobre uma ou várias construções localizadas em um mesmo campus. Permite a interconexão de equipamentos de comunicação de dados numa pequena região que são *distâncias* entre *100m e 25km*.
- **Redes Metropolitanas**: Cobrem uma cidade com *distâncias* abaixo de *200km*. Necessita a intervenção de operadoras públicas.
- **Redes de Longa Distância**: Necessita de intervenção de operadoras públicas. Face a várias considerações em relação ao custo. 

##### O que é a internet?
- **Hosts e sistemas finais**: *Estações de trabalho, servidores, celulares, microondas* rodando aplicações de rede.
- **Enlaces**: Canais de comunicação como *fibra, par trançado, rádio, satélite*.
- **Roteadores**: Encaminham *pacotes de dados* através da rede.
- **ISP**: Provedores de serviços de internet.

Protocolos controlam o envio e recepção de mensagens. 
Exemplo:

>TCP, IP, HTTP, FTP, PPP

**Internet**: rede de redes.
- Livremente hieráquica.
- Internet pública vs intranet privada.

**A infraestrutura de comunicação dá suporte às aplicações distribuídas**: 

> WWW, email, jogos, comércio eletrônico, compartilhamento de arquivos.

**Borda da rede**:
-  Aplicações e hospedeiros (*hosts*)
**Núcleo da rede**:
- Roteadores
- Rede de redes
**Rede de acesso**:
- Enlaces de comunicação

##### Borda da rede:
- **Sistemas finais (hosts)**: Rodam programas de aplicação como por exemplo: world wide web, email e etc.
- **Modelo Cliente / Servidor**: Host cliente faz pedidos que são atendidos pelos servidores:  Browser (host cliente) <-> Servidor 
- **Modelo Peer to Peer**

_Serviço orientado a conexões._

##### Borda da rede: Serviço orientado a conexões

**Objetivo**: Transferência de dados entre sistemas finais.

**Handshaking**: Inicialização para a transferência de dados.
- Alô -> Olá -  Protocolo humano de comunicação. 
- Inicializa o *estado* em dois hosts que desejam se comunicar.

**TCP - Transmission Control Protocol**: Serviço orientado a conexão da internet.
- Transferência de dados através de um fluxo de bytes ordenado e confiável.
	- Perda: reconhecimento e retransmissão.
- Controle de fluxo. Transmissão não inundará o receptor.
- Controle de congestionamento. Transmissor diminui a taxa de transmissão quando a rede está congestionada.

##### Borda da rede: Serviço sem conexões

**Objetivo**: Transferência de dados entre sistemas finais. 

**UDP - User Datagram Protocol**: Serviço sem conexão da internet. 
- Transferência de dados não confiável. 
- Não controla o fluxo nem o congestionamento. 

**Aplicações que usam TCP**: 
- HTTP (www), FTP (transferência de arquivo), Telnet (login remoto), SMTP (email).

**Aplicações que usam UDP**: 
- Streaming media, teleconferência, telefonia e internet.

