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

*&lt;Diagrama de relacionamento entre classes para os seus atributos e operações&gt;*

# Diagrama de Componentes

*&lt;Diagrama para exibir a relação estrutural dos componentes de um sistema de software

# Decisões de arquitetura

*&lt;Descrever a infraestrutura escolhida para arquitetura do projeto&gt;*

# Diagrama de implantação

*&lt;Diagrama para exibir o relacionamento de hardware e software no projeto&gt;*

# Referências

*&lt;Lista de referências&gt;*
