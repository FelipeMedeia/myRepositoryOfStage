# O presente repósitorio será o local onde terei a adição dos resumos feitos durante o estágio

## Neste segundo momento falaremos sobre:

- **Bitcoin e Blockchain**
- **Assinaturas Digitais**
- **Moeda Digital**
- **Proof of work**
- **Evitando Gasto Duplo**
- **Carteiras Digitais**
- **Anonimato**
---


# Bitcoin e Blockchain

O Blockchain foi apresentado como um sistemas que permite você adicionar dados e não pode alterar. Possui um mecânismo em que as duas partes envolvidas precisam estar em consenso. Isso foi apresentado em etapas, sua explicação podendo ser compreendida de uma criança a um especialista na área.

O Bitcoin é visto como uma unidade de troca, uma reserva de valor. Foi idealizada em 2008 em um artigo de Satoshe Nakamoto, um pseudônimo. Pontos importantes são: *Criptografia*, *Blockchain*, *Redes descentralizadas* e *Engenharia de Incentivo*. Em 2009 surgiu o primeiro bloco do Blockchain ( Genesis Block). Vamos analisar as caracteristicas entre o Bitcoin e os sistemas tradicionais ou os Bancos.

| Caracteristicas       | Sistema Tradicional      | Bitcoin  |
|---------              |--------------            |----------    |
| Contabilidade         | Centralizado             |Blockchain       |
| Armazenamento         | Fracionado               |100%     |
| Segurança             | Institucional            |Criptográfia |
| Emissão de moeda      | Politica economica       |Algoritmos |
| Transações            | Centralizado             |Distribuido, peer-to-peer |
| Autenticação          | Centralizado             |Blockchain      |
| Regulamentação        | Banco central, Normas    |Ainda indefinida |
| Processo de decisão   | Arbitrário               |Consenso     |
| Controle do dinheiro  | Banco                    |Você |
----   

O blockchain tem um mecânismo que auxilia em sua segurança com relação a tentativas de fraudes, esse sistema funciona como correntes, onde um bloco sempre aponta para outro, ou seja, se houver uma tentativa de alteração no bloco ele precisaria mudar também os dados dos blocos subsequentes aquele, o que é uma coisa bastante improvável, pois a capacidade de poder computacional para isso é enorme. Então com relação a seu funcionamento, existem as **Assinaturas Digitais**, em visão geral se trata de um mecânismo onde: Só você pode assinar( Quem possui a chave, falaremos a seguir); Qualquer um pode verificar a assinatura e Assinatura atrelada ao documento. Sobre seu funcionamento, esse sistema funciona com base no par de *Chave secreta*(Que deve permanecer em segredo, pois esse sistema de validação é com base nessa verificação de chave, assim quem possui essa chave secreta a priori é o dono dela) e a *Chave pública* que é atrelada ao documento, em resumo, ao assinar um documento você usará a chave secreta, ela então fará uma chave pública para aquele documento baseada no hash. Algumas propriedades da chave pública são:
- Impossivel de falsificar
- Fácil de verificar
- Atrelada ao documento

Então com isso foi apresentado como **Criar uma Moeda Digital**, de inicio vamos falar sobre *hash*, onde o hash do bloco é como se fose seu nome:
- Transforma um texto de entrada de qualquer tamanho em um texto de saída de tamanho fixo, por exemplo os codigos de barras.
Então as funções hash criptográficas são:
- Fácil de computar
- Livre de colisão: Impossivel* dois inputs com o mesmo output              *muito, muito improvável
- Unidirecional: Impossivel* descobrir o input dado seu output
- "Puzzle Friendly": Se modifica pouco na entrada muda muito na saída.

Ou seja, é inviável alterar os dados de um bloco, pois a hash é gerada pela entrada, alterando os dados, o hash muda, com isso toda a sequência que guardavam os dados da hash que foi alterada é quebrado, resultando em uma dependência de mudança em cadeia. Cada bloco armazena os dados relativos o seu hash e o hash do bloco anterior.

Foi então exemplificado os passos e caracteristicas das moedas e nesse exemplo havia uma unidade central que controlava o funcionamento, usada apenas para dar base para a compreensão, pois no **Bitcoin** essa unidade central é substituida por uma rede de computadores, sendo distribuida, sem hierarquia e baseada em protocolo de consenso, com isso qualquer computador conectado à rede blockchain é um nó desta rede, onde temos:
- Full Nodes:(Nós completos, mineradores)
   - Validam todas as transaçôes emeitidas pela rede
  - Mantêm a consistência da blockchain
- Lite Nodes:(Nós mais leves, podem ser carteiras)
  - Não armazenam toda a blockchain
  - Necessitam de informação de outros nós.

As transações possui os seguintes itens, assinatura, as moedas criadas para essa transação e a chave pública para quem está sendo enviada e as moedas que foram consumidas, para isso, as transações de bitcoin só são inseridas na blockchain quando são validadas pelos mineradores que também garante que todos os nós mantenham a mesma blockchain armazenada. Os mineradores então:
- Validam as transações recebidas e criam novos blocos
- Competem entre si pelo direito de adicionar o próximo bloco na blockchain
- Verificam blocos obtidos por outros mineradores e adicionam a blockchain quando válidos
- Sempre extendem o ramo mais longo da blockchain

Para a mineração usam o **Proof of work** que é o metodo de consenso, os blocos possuem em seu hash uma combinação e quando um minerador encontra a correta, eles entam em um conseso implicito para a adição desse bloco na blockchain, isso se dá quando começam a minerar sobre esse novo bloco buscando a combinação correta para o próximo, isso acontece em um intervalo de 10 minutos, existe também o conceito de *coinbase translaction*, onde o ganho por mineração cai pela metade a cada 4 anos. Com base em tudo apresentado, mineração em casa é práticamente impossível, dado o grande consumo de energia e processamento e mesmo assim não da garantia de éxito, existem as *Mining pools*, ela vai centralizar e dividir o ganho proporcionalmente a mineração de cada minerador, ela reduz os ricos e tem otimização. Graças ao PoW não existe o gasto duplo, que consiste básicamente em usar as mesmas moedas mais de uma vez, para que funcionasse um hacker precisaria de 51% de hash power, ele precisa minerar 5x mais que outros mineradores.

**Carteiras** apresentam 3 pilares: Disponibilidades, segurança e conveniência. Para formatos existem, a carteira de papel, que é litealmente um pedaço de papel e tem sua segurança tanto quanto um papel, um ponto positivo é não está na rede, sendo imune* a hackers. As carteira de hardware apresentam muitas váriedades são as mais seguras e permitem multiplos pares de CP/CS, que é sempre recomendado ter mais de uma chave pública. Existem as carteiras de software que funcionam em descktop e mobile e é tão segura quanto seu computador e as carteiras online as mais práticas, porém menos seguras, você não consegue saber seus pares de chave pública e privada.

As **Exchanges** surgem para apresentar formas de negociar criptomoedas, em resumo, elas centralizam as negociações onde pessoas tem cripto e querem vender e pessoas tem dinheiro e querem comprar criptos. Elas são básicamente um site. Em comparação com os Bancos, bancos são regulados, as exchanges( ainda não), em resumo você não tem nenhuma segurança com relação aos investimentos, por isso é sempre recomendado pesquisar bem antes de tomar qualquer decisão e saber que está correndo um riscode perder tudo que está colocando a jogo alí. Ficar sempre atento para não cair em esquemas de pirâmides...