# Pokémon NFT Battle Game (ERC-721)

## Introdução

Este projeto é um contrato inteligente desenvolvido em **Solidity** que utiliza o padrão ERC-721 para criar tokens não fungíveis (NFTs). Ele simula um jogo de batalhas entre Pokémons, onde cada Pokémon é representado por um NFT com atributos únicos, como nome, nível e imagem. Esse trabalho foi desenvolvido com o objetivo de aprofundar meu conhecimento sobre Blockchain, explorando tanto aspectos técnicos da programação quanto aplicações práticas da tecnologia.

O processo de desenvolvimento me proporcionou aprendizado sobre contratos inteligentes, segurança em Blockchain, uso de bibliotecas padrão da OpenZeppelin e os fundamentos da criação e gestão de NFTs.

---

## Estrutura do Contrato

O contrato, chamado `PokemonNft`, herda funcionalidades do padrão ERC-721 implementado pela biblioteca OpenZeppelin, garantindo compatibilidade com o ecossistema NFT. Ele é dividido em três principais áreas de funcionalidade:

### Representação dos Pokémons

Cada Pokémon é modelado como uma estrutura que inclui:
- **Nome**: Um identificador textual do Pokémon.
- **Nível**: Um atributo numérico que influencia a força do Pokémon.
- **Imagem**: Um link ou caminho para a representação visual do Pokémon.

Esses Pokémons são armazenados em um array público, permitindo que qualquer pessoa consulte suas informações diretamente na Blockchain.

### Propriedade e Controle

O contrato identifica o criador do contrato como o proprietário do jogo. Além disso, ele implementa mecanismos que garantem que somente o dono de um Pokémon pode realizar ações específicas, como batalhas, usando verificações baseadas no endereço do usuário.

### Criação e Batalhas

#### Criação de Pokémons

Os usuários podem adicionar novos Pokémons ao jogo, que são automaticamente vinculados às suas contas. Esses Pokémons são convertidos em NFTs, sendo emitidos como tokens únicos no padrão ERC-721.

#### Mecânica de Batalha

Uma funcionalidade central do jogo é a possibilidade de realizar batalhas entre Pokémons. Durante uma batalha, o nível de ambos os Pokémons é ajustado com base em seus atributos:
- Se o nível do atacante for maior ou igual ao do defensor, o atacante ganha mais experiência.
- Caso contrário, o defensor ganha mais experiência.

Essa dinâmica cria uma progressão contínua para os jogadores que participam do sistema.

---

## Aplicações e Aprendizado

Este projeto foi desenvolvido como uma experiência prática para aplicar e consolidar conhecimentos teóricos sobre Blockchain e contratos inteligentes. Abaixo estão algumas das lições aprendidas e áreas de aplicação:

### Contratos Inteligentes na Prática

Ao criar este contrato, foi possível compreender como contratos inteligentes garantem a execução descentralizada e imutável de regras previamente definidas. A programação de modificadores, como restrições baseadas no proprietário, também reforçou meu entendimento sobre segurança e boas práticas.

### NFTs e o Padrão ERC-721

Aprendi a implementar e personalizar o padrão ERC-721, explorando sua capacidade de representar ativos únicos e interoperáveis. Entendi como ferramentas padrão, como as bibliotecas da OpenZeppelin, simplificam o processo de desenvolvimento ao garantir compatibilidade e segurança.

### Gamificação e Blockchain

Combinar a lógica de um jogo com a tecnologia de Blockchain abriu novas perspectivas sobre como criar experiências descentralizadas. A transparência e a imutabilidade das regras do jogo são garantidas pela natureza do contrato inteligente, enquanto a propriedade dos NFTs dá aos usuários controle total sobre seus ativos digitais.

---

## Implantação e Execução

O contrato foi projetado para ser implantado em uma rede Ethereum (ou compatível), utilizando ferramentas como Ganache para simular redes locais e Hardhat ou Truffle para gerenciar a implantação. Esses frameworks simplificam a interação com o contrato, desde a criação de Pokémons até a realização de batalhas.

Após a implantação, as interações com o contrato podem ser realizadas por meio de scripts ou interfaces descentralizadas, como carteiras compatíveis com ERC-721.

---

## Conclusão

Este projeto demonstra como a tecnologia Blockchain pode ser aplicada para criar jogos descentralizados, utilizando NFTs como componentes centrais. A mecânica de batalhas e a personalização dos Pokémons são exemplos de como combinar elementos de gamificação com segurança e transparência da Blockchain.

Além disso, o trabalho reforça a importância dos contratos inteligentes no desenvolvimento de aplicações descentralizadas. Suas possibilidades de expansão incluem a implementação de um marketplace, novas dinâmicas de evolução para os Pokémons e até funcionalidades de interação multiplayer. 

Este projeto é um marco importante na minha jornada de aprendizado em Blockchain, evidenciando seu potencial transformador para o futuro da tecnologia.
