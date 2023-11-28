<h2><a href= "https://www.mackenzie.br">Universidade Presbiteriana Mackenzie</a></h2>
<h3><a href= "https://www.mackenzie.br/graduacao/sao-paulo-higienopolis/sistemas-de-informacao">Sistemas de Informação</a></h3>


<font size="+12"><center>
*&lt;Nome do Projeto&gt;*
</center></font>

>*Observação 1: A estrutura inicial deste documento é só um exemplo. O seu grupo deverá alterar esta estrutura de acordo com o que está sendo solicitado na disciplina.*

>*Observação 2: O índice abaixo não precisa ser editado se você utilizar o Visual Studio Code com a extensão **Markdown All in One**. Essa extensão atualiza o índice automaticamente quando o arquivo é salvo.*

**Conteúdo**

- [Autores](#nome-alunos)
- [Descrição do projeto](#introdução-do-projeto)
- [Análise de requisitos funcionais e não-fucionais](#descrição-dos-requisitos)
- [Diagrama de casos de uso](#diagrama-de-comportamento-atores)
- [Descrição dos casos de uso](#descrição-das-funcões)
- [Diagrama de senquencia](#diagrama-de-ordem-interações)
- [Diagrama de classes](#diagrama-orientado-objetos)
- [Diagrama de componentes](#diagrama-estrutura-componente)
- [Decisões de arquitetura](#decisões-de-arquitetura)
- [Diagrama de implantação](#diagrama-de-hardware-software)
- [Referências](#referências)


# Autores
Kauã Paixão - 32349351

Rodrigo Graziani - 32339143

Yuri Sanches - 32088541

# Descrição do projeto

A Pizza-Express é uma cadeia de 40 lojas de fast-food e entrega em casa.

Pizza-Express tem perdido recentemente 30% do rendimento de vendas devido a um problema em seu negócio da entrega. Atribuem este problema a seu concorrente principal que promoveu um programa que garante o serviço de entrega em 30 minutos, desde a entrada da ordem de serviço até a entrega na casa do cliente (delivery).

Pizza-Express anuncia a entrega em uma hora.

Pizza-Express usa atualmente computadores para armazenar as operações e as funções usuais do negócio, mas não auxiliam nas funções para processar a entrega dos pedidos dos seus clientes.

Elonn Muske, o gerente de sistemas de informação é o encarregado para desenvolver uma aplicação do software para identificar a localização de lojas de pizza Pizza-Express mais próxima do cliente e para criar o sistema de software necessário para operá-las.

O patrocinador deste projeto, a empresa Papa-Léguas Delivery, disse que o futuro da Pizza-Express depende deste projeto.

A equipe deverá investigar uma opção para entregar a pizza em menos de 30 minutos.

A sua idéia é montar lojas de pizza Pizza-Express que não teriam nenhum espaço de varejo, pois a sua função é somente receber ordens, preparar e entregar as pizzas.

A loja deverá ser localizada o mais próximo do cliente receberá a ordem através de uma central, processará, e entregará a ordem dentro de 10 ou 15 minutos da entrada do pedido.

Há dois projetos do desenvolvimento do software identificados aqui:

- O primeiro é um sistema de software para o atendimento do pedido e para encontrar localização da fábrica da pizza mais próxima do cliente para fazer a entrega;
- O segundo é um sistema de software para suportar operações da fábrica de pizzas.

# Análise de requisitos funcionais e não-funcionais
Projeto 1: Sistema de Software para Atendimento do Pedido e Localização da Fábrica da Pizza

Requisitos Funcionais:

1. Recebimento de Pedidos.
2. Identificação da Localização do Cliente.
3. Integração com GPS.
4. Estimativa de Tempo de Entrega.

Requisitos Não Funcionais:

1. Desempenho ágil.
2. Escalabilidade para atender a picos de demanda.
3. Disponibilidade 24/7.
4. Segurança dos dados do cliente.

Projeto 2: Sistema de Software para Suportar Operações da Fábrica de Pizzas

Requisitos Funcionais:

1. Gerenciamento de Pedidos.
2. Priorização de Pedidos.
3. Integração com o Sistema de Entrega.
4. Monitoramento de Tempo.

Requisitos Não Funcionais:

1. Eficiência operacional.
2. Confiabilidade e ausência de erros.
3. Integração suave com tecnologias existentes.
4. Facilidade de uso para os funcionários.
# Diagrama de casos de uso

[Diagrama de usos.pdf](https://github.com/profdscrodrigo/UML-Classroom-FCI/files/12836204/Diagrama.de.usos.pdf)

# Descrição dos casos de uso
Descrição Detalhada dos Casos de Uso:

1. Fazer Pedido:
   - Ator Principal: Cliente
   - Pré-condições:
     - O cliente deve estar logado no sistema.
     - O cliente deve ter acesso ao menu de opções.
   - Pós-condições:
     - O pedido é registrado no sistema.
   - Requisitos:
     - O sistema deve exibir um menu atualizado com opções de pizzas.
   - Fluxo Básico:
     1. O cliente acessa o menu de opções.
     2. O cliente escolhe uma pizza do menu.
     3. O cliente seleciona o tamanho desejado para a pizza.
     4. O cliente adiciona a pizza ao carrinho.
     5. O cliente confirma o pedido.

2. Personalizar Pedido:
   - Ator Principal: Cliente
   - Pré-condições:
     - O cliente deve ter selecionado uma pizza.
   - Pós-condições:
     - As personalizações são aplicadas ao pedido.
   - Requisitos:
     - O sistema deve permitir que o cliente escolha os ingredientes e as opções de personalização.
   - Fluxo Básico:
     1. O cliente escolhe a opção de personalizar a pizza.
     2. O cliente seleciona os ingredientes e opções desejados.
     3. O cliente confirma as personalizações.

3. Cancelar Pedido:
   - Ator Principal: Cliente
   - Pré-condições:
     - O cliente deve ter um pedido em processamento.
   - Pós-condições:
     - O pedido é cancelado e removido do sistema.
   - Requisitos:
     - O sistema deve permitir que o cliente cancele o pedido antes do início da preparação.
   - Fluxo Básico:
     1. O cliente acessa a seção de pedidos.
     2. O cliente seleciona o pedido que deseja cancelar.
     3. O cliente confirma o cancelamento do pedido.

4. Efetuar Pagamento:
   - Ator Principal: Cliente
   - Pré-condições:
     - O cliente deve ter um pedido pronto para pagamento.
   - Pós-condições:
     - O pagamento é efetuado e o pedido é confirmado.
   - Requisitos:
     - O sistema deve oferecer diferentes opções de pagamento.
   - Fluxo Básico:
     1. O cliente escolhe a opção de pagamento desejada.
     2. O cliente fornece as informações de pagamento necessárias.
     3. O sistema processa o pagamento.

5. Ativar Localização:
   - Ator Principal: Cliente
   - Pré-condições:
     - O cliente deve permitir o acesso à sua localização no dispositivo.
   - Pós-condições:
     - A localização do cliente está disponível para o sistema.
   - Requisitos:
     - O sistema deve solicitar permissão para acessar a localização do dispositivo.
   - Fluxo Básico:
     1. O cliente ativa a funcionalidade de localização em seu dispositivo.
     2. O sistema obtém a localização atual do cliente.

6. Identificar Localização do Cliente:
   - Ator Principal: Geolocalizador
   - Pré-condições: A localização do cliente deve estar disponível.
   - Pós-condições:
     - A localização do cliente é identificada e disponível para uso no sistema.
   - Requisitos:
     - O sistema deve utilizar APIs ou funcionalidades do dispositivo para obter a localização do cliente.
   - Fluxo Básico:
     1. O sistema obtém as informações de localização do dispositivo do cliente.

7. Encontrar Fábricas de Pizzas Mais Próximas:
   - Ator Principal: Geolocalizador
   - Pré-condições: A localização do cliente deve estar identificada.
   - Pós-condições:
     - As fábricas de pizzas mais próximas são identificadas para processamento do pedido.
   - Requisitos:
     - O sistema deve ter um banco de dados atualizado com as localizações das fábricas de pizzas.
   - Fluxo Básico:
     1. O sistema utiliza a localização do cliente para identificar as fábricas de pizzas mais próximas.

8. Receber Chamado:
   - Ator Principal: Funcionário Pizza-Express
   - Pré-condições:
     - O pedido do cliente deve ter sido validado e encaminhado para preparação.
   - Pós-condições:
     - O pedido é recebido pelo funcionário para preparação.
   - Requisitos:
     - O sistema deve notificar os funcionários sobre os novos pedidos recebidos.
   - Fluxo Básico:
     1. O sistema notifica os funcionários sobre um novo pedido recebido.

9. Validar Pedido:
   - Ator Principal: Funcionário Pizza-Express
   - Pré-condições:
     - O pedido deve ter sido recebido pelo funcionário.
   - Pós-condições:
     - O pedido é validado e pronto para preparação.
   - Requisitos:
     - O sistema deve apresentar todas as informações do pedido ao funcionário para validação.
   - Fluxo Básico:
     1. O funcionário revisa o pedido para garantir que todas as informações estejam corretas e completas.

10. Preparar Pedido:
    - Ator Principal: Funcionário Pizza-Express
    - Pré-condições:
      - O pedido deve ter sido validado pelo funcionário.
    - Pós-condições:
      - O pedido é preparado e pronto para entrega.
    - Requisitos:
      - O sistema deve apresentar as instruções de preparação para o pedido ao funcionário.
    - Fluxo Básico:
      1. O funcionário inicia a preparação da pizza de acordo com as instruções do pedido.

11. Finalizar Entrega:
    - Ator Principal: Entregador
    - Pré-condições:
     

 - O pedido deve estar preparado e pronto para entrega.
    - Pós-condições:
      - O pedido é entregue ao cliente.
    - Requisitos:
      - O sistema deve permitir que o funcionário de entrega atualize o status de entrega.
    - Fluxo Básico:
      1. O funcionário de entrega entrega a pizza ao cliente.
      2. O sistema atualiza o status do pedido para entregue.

12. Logar no Sistema:
    - Ator Principal: Funcionário Pizza-Express
    - Pré-condições:
      - O funcionário deve ter um login e senha válidos.
    - Pós-condições:
      - O funcionário está autenticado no sistema e pode acessar as funcionalidades.
    - Requisitos:
      - O sistema deve garantir a segurança e autenticidade das credenciais de login.
    - Fluxo Básico:
      1. O funcionário insere suas credenciais de login (usuário e senha).
      2. O sistema autentica as credenciais e permite o acesso.
# Diagrama de sequencia

[*&lt;Diagrama de ordem e interação dos objetos&gt;*](https://drive.google.com/file/d/1PcLaR8Faomr9_FZ7KYQ4GoL_Tw3Ooavh/view?pli=1)

# Diagrama de classes

![diagclasse](https://github.com/profdscrodrigo/UML-Classroom-FCI/assets/137851402/05bb0550-abf0-42a8-92cc-daba7f77db9c)

# Diagrama de Componentes

![diagcomp](https://github.com/profdscrodrigo/UML-Classroom-FCI/assets/137851402/d9dbdfda-a105-4432-bf95-8c63b2697881)

# Decisões de arquitetura

Decisão de Arquitetura para Pizza-Express:

1. Microsserviços:
   - Justificativa: Adote uma arquitetura de microsserviços para dividir a aplicação em componentes independentes, cada um responsável por uma função específica. Isso facilita a manutenção, escalabilidade e implementação de novos recursos de forma modular.

2. Serviço de Pedidos:
   - Descrição: Implemente um serviço de pedidos responsável pelo registro e gerenciamento de pedidos dos clientes.
   - Tecnologias: Node.js, Express, MongoDB.

3. Serviço de Localização:
   - Descrição: Desenvolva um serviço de localização que utilize a geolocalização para encontrar a fábrica de pizza mais próxima do cliente.
   - Tecnologias: Python, Flask, Redis.

4. Serviço de Entrega:
   - Descrição: Crie um serviço dedicado para gerenciar a entrega de pedidos, otimizando rotas e fornecendo atualizações em tempo real aos clientes.
   - Tecnologias: Java, Spring Boot, PostgreSQL.

5. Serviço de Fábrica de Pizzas:
   - Descrição: Implemente um serviço para operações internas da fábrica, como preparação de pizzas, gestão de estoque e rastreamento interno.
   - Tecnologias: Ruby on Rails, MySQL.

6. API Gateway:
   - Descrição: Introduza um API Gateway para gerenciar as solicitações entre os diferentes microsserviços, garantindo segurança e controle de acesso.
   - Tecnologias: Nginx, Kong.

7. Banco de Dados Distribuído:
   - Descrição: Utilize um banco de dados distribuído para garantir alta disponibilidade e escalabilidade.
   - Tecnologias: Cassandra, Amazon DynamoDB.

8. Contêineres e Orquestração:
   - Descrição: Empregue contêineres (Docker) e orquestração (Kubernetes) para facilitar o empacotamento, implantação e dimensionamento dos serviços.

9. Monitoramento e Logging:
   - Descrição: Implemente ferramentas de monitoramento e logging para acompanhar o desempenho, identificar problemas rapidamente e melhorar continuamente o sistema.
   - Tecnologias: Prometheus, Grafana, ELK Stack.

10. Comunicação Assíncrona:
    - Descrição: Use mensageria assíncrona (por exemplo, RabbitMQ) para desacoplar serviços e garantir uma comunicação eficiente.

Justificativas e Benefícios:

- Escalabilidade: A arquitetura distribuída permite escalar componentes individualmente, atendendo ao aumento da demanda.
  
- Resiliência: Microsserviços independentes aumentam a resiliência, já que falhas em um serviço não afetam diretamente os outros.

- Agilidade: A abordagem de microsserviços permite atualizações e implementações independentes, promovendo agilidade no desenvolvimento.

- Eficiência na Entrega: A separação de serviços especializados, como localização e entrega, otimiza as operações, facilitando o cumprimento do objetivo de entrega em menos de 30 minutos.

- Facilidade de Manutenção: A manutenção e expansão de funcionalidades são mais fáceis com microsserviços, pois cada serviço é gerenciado separadamente.

# Diagrama de implantação

![diagimp](https://github.com/profdscrodrigo/UML-Classroom-FCI/assets/137851402/3860a22e-954b-4c87-8b58-d32318012d48)

# Referências

Slides de Desenvolvimento de Sistemas I

Tecnologias de IA

StarUML
