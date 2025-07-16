# Especificação de Requisitos

## Introdução

Este documento apresenta os requisitos do sistema **Finis**, uma aplicação de controle financeiro pessoal. O objetivo é descrever de forma clara e objetiva as funcionalidades esperadas, bem como os requisitos não funcionais que devem ser atendidos para garantir a usabilidade, desempenho e segurança do sistema.

Os requisitos aqui listados servirão como base para o desenvolvimento, testes e validação do sistema.

## Escopo

O sistema permitirá o gerenciamento de receitas, despesas, categorias financeiras, geração de relatórios e exportação de dados. Funcionalidades bancárias ou de integração direta com instituições financeiras não fazem parte do escopo desta versão.

<details>
<summary>  <h2>Requisitos funcionas do usuário </h2>  </summary>



  <table border="1">
  <thead>
    <tr>
      <th>ID</th>
      <th>Requisito</th>
      <th>Tipo</th>
      <th>Prioridade</th>
      <th>Status</th>
    </tr>
  </thead>
  <tbody>
    <tr><td>RF#01</td><td>O usuário deve ser capaz de efetuar login e logout com segurança usando suas credenciais.</td><td>Autenticação</td><td>Alta</td><td>Backlog</td></tr>
    <tr><td>RF#02</td><td>O usuário deve ser capaz de criar contas utilizando seu email.</td><td>Cadastro</td><td>Alta</td><td>Backlog</td></tr>
    <tr><td>RF#03</td><td>O usuário deve ser capaz de editar suas informações de perfil.</td><td>Perfil</td><td>Média</td><td>Backlog</td></tr>
    <tr><td>RF#04</td><td>O usuário deve ser capaz de recuperar sua senha via email.</td><td>Recuperação de Conta</td><td>Alta</td><td>Backlog</td></tr>
    <tr><td>RF#05</td><td>O usuário deve ser capaz de registrar sua renda.</td><td>Financeiro</td><td>Alta</td><td>Backlog</td></tr>
    <tr><td>RF#06</td><td>O usuário deve ser capaz de categorizar sua renda.</td><td>Financeiro</td><td>Média</td><td>Backlog</td></tr>
    <tr><td>RF#07</td><td>O usuário deve ser capaz de editar os dados de sua renda.</td><td>Financeiro</td><td>Média</td><td>Backlog</td></tr>
    <tr><td>RF#08</td><td>O usuário deve ser capaz de excluir os dados de sua renda.</td><td>Financeiro</td><td>Média</td><td>Backlog</td></tr>
    <tr><td>RF#09</td><td>O usuário deve ser capaz de registrar sua despesa.</td><td>Financeiro</td><td>Alta</td><td>Backlog</td></tr>
    <tr><td>RF#10</td><td>O usuário deve ser capaz de categorizar sua despesa.</td><td>Financeiro</td><td>Média</td><td>Backlog</td></tr>
    <tr><td>RF#11</td><td>O usuário deve ser capaz de editar os dados de sua despesa.</td><td>Financeiro</td><td>Média</td><td>Backlog</td></tr>
    <tr><td>RF#12</td><td>O usuário deve ser capaz de excluir os dados de sua despesa.</td><td>Financeiro</td><td>Média</td><td>Backlog</td></tr>
    <tr><td>RF#13</td><td>O usuário deve ser capaz de fazer upload de imagens de recibos. As imagens devem poder ser associadas a uma despesa ou a uma renda.</td><td>Upload</td><td>Média</td><td>Backlog</td></tr>
    <tr><td>RF#14</td><td>O usuário deve ser capaz de excluir a imagem de recibo.</td><td>Upload</td><td>Baixa</td><td>Backlog</td></tr>
    <tr><td>RF#15</td><td>O usuário deve ser capaz de editar a imagem de recibo.</td><td>Upload</td><td>Baixa</td><td>Backlog</td></tr>
    <tr><td>RF#16</td><td>O usuário deve ser capaz de baixar a imagem de recibo.</td><td>Upload</td><td>Baixa</td><td>Backlog</td></tr>
    <tr><td>RF#17</td><td>O usuário deve ser capaz de visualizar o resumo mensal com total de rendas, despesas e saldo atual.</td><td>Relatórios</td><td>Alta</td><td>Backlog</td></tr>
    <tr><td>RF#18</td><td>O usuário deve ser capaz de visualizar gráficos de renda e despesas por período ou categoria.</td><td>Relatórios</td><td>Média</td><td>Backlog</td></tr>
    <tr><td>RF#19</td><td>O usuário deve ser capaz de filtrar registros por data, categoria ou valor.</td><td>Visualização</td><td>Média</td><td>Backlog</td></tr>
    <tr><td>RF#20</td><td>O usuário deve ser capaz de buscar um registro específico de renda ou despesa por palavra-chave.</td><td>Pesquisa</td><td>Média</td><td>Backlog</td></tr>
    <tr><td>RF#21</td><td>O usuário deve ser capaz de cancelar uma despesa ou renda recorrente futura.</td><td>Recorrência</td><td>Baixa</td><td>Backlog</td></tr>
    <tr><td>RF#22</td><td>O usuário deve ser capaz de cadastrar uma renda ou despesa recorrente com periodicidade mensal, semanal, etc.</td><td>Recorrência</td><td>Média</td><td>Backlog</td></tr>
  </tbody>
</table>
</details>





## Requisitos  Funcionais do Sistema

 <table border="1" cellspacing="0" cellpadding="8">
  <thead>
    <tr>
      <th>ID</th>
      <th>Requisito</th>
      <th>Tipo</th>
      <th>Prioridade</th>
      <th>Status</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>RF#01</td>
      <td>O sistema deve exportar os registros financeiros do usuário nos formatos .csv e .pdf, incluindo rendas, despesas e saldo.</td>
      <td>Exportação / Dados</td>
      <td>Baixa</td>
      <td>Backlog</td>
    </tr>
    <tr>
      <td>RF#02</td>
      <td>O sistema deve validar os dados inseridos, como valores numéricos, formatos de data e categorias válidas.</td>
      <td>Validação</td>
      <td>Alta</td>
      <td>Backlog</td>
    </tr>
    <tr>
      <td>RF#03</td>
      <td>O sistema deve exibir uma mensagem de confirmação ao registrar uma despesa.</td>
      <td>UI / Validação</td>
      <td>Média</td>
      <td>Backlog</td>
    </tr>
    <tr>
      <td>RF#04</td>
      <td>O sistema deve fornecer filtros eficientes para busca e consulta de registros por data, categoria e valor.</td>
      <td>Filtro / Busca</td>
      <td>Alta</td>
      <td>Backlog</td>
    </tr>
    <tr>
      <td>RF#05</td>
      <td>O sistema deve mostrar o saldo disponível na tela inicial após o login.</td>
      <td>UI / Interface</td>
      <td>Alta</td>
      <td>Backlog</td>
    </tr>
    <tr>
      <td>RF#06</td>
      <td>O sistema deve apresentar um gráfico de pizza com a distribuição das despesas por categoria no mês atual.</td>
      <td>UI / Dados</td>
      <td>Média</td>
      <td>Backlog</td>
    </tr>
    <tr>
      <td>RF#07</td>
      <td>O sistema deve atualizar automaticamente a lista de transações ao adicionar uma nova renda.</td>
      <td>UI / Interface</td>
      <td>Alta</td>
      <td>Backlog</td>
    </tr>
    <tr>
      <td>RF#08</td>
      <td>O sistema deve ocultar os campos de recibo quando o tipo de transação for ‘transferência’.</td>
      <td>UI / Interface</td>
      <td>Média</td>
      <td>Backlog</td>
    </tr>
    <tr>
      <td>RF#09</td>
      <td>O sistema deve apresentar um botão fixo no canto inferior direito da tela para criação de novos registros.</td>
      <td>UI / Interface</td>
      <td>Média</td>
      <td>Backlog</td>
    </tr>
    <tr>
      <td>RF#10</td>
      <td>O sistema deve permitir navegação entre seções por meio de um menu lateral.</td>
      <td>UI / Navegação</td>
      <td>Média</td>
      <td>Backlog</td>
    </tr>
    <tr>
      <td>RF#11</td>
      <td>O sistema deve alertar o usuário visualmente quando seu saldo ficar negativo.</td>
      <td>UI / Alerta</td>
      <td>Média</td>
      <td>Backlog</td>
    </tr>
    <tr>
      <td>RF#12</td>
      <td>O sistema deve apresentar mensagens de validação ao usuário quando os campos estiverem incorretos.</td>
      <td>UI / Validação</td>
      <td>Média</td>
      <td>Backlog</td>
    </tr>
  </tbody>
</table>



## Requisitos Não Funcionais

<table border="1" cellspacing="0" cellpadding="8">
  <thead>
    <tr>
      <th>ID</th>
      <th>Requisito</th>
      <th>Tipo</th>
      <th>Prioridade</th>
      <th>Status</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>RNF#01</td>
      <td>O sistema deve armazenar senhas de forma criptografada utilizando algoritmo seguro (ex: bcrypt).</td>
      <td>Segurança</td>
      <td>Alta</td>
      <td>Backlog</td>
    </tr>
    <tr>
      <td>RNF#02</td>
      <td>O sistema deve utilizar HTTPS para comunicação entre cliente e servidor.</td>
      <td>Segurança</td>
      <td>Alta</td>
      <td>Backlog</td>
    </tr>
    <tr>
      <td>RNF#03</td>
      <td>O sistema deve validar token de autenticação em cada requisição protegida.</td>
      <td>Segurança</td>
      <td>Alta</td>
      <td>Backlog</td>
    </tr>
    <tr>
      <td>RNF#04</td>
      <td>O sistema deve proteger contra ataques como SQL Injection, XSS e CSRF.</td>
      <td>Segurança</td>
      <td>Alta</td>
      <td>Backlog</td>
    </tr>
    <tr>
      <td>RNF#05</td>
      <td>O sistema deve responder às requisições em até 2 segundos na média.</td>
      <td>Desempenho</td>
      <td>Média</td>
      <td>Backlog</td>
    </tr>
    <tr>
      <td>RNF#06</td>
      <td>A interface inicial deve carregar em no máximo 3 segundos em conexão padrão.</td>
      <td>Desempenho</td>
      <td>Média</td>
      <td>Backlog</td>
    </tr>
    <tr>
      <td>RNF#07</td>
      <td>O sistema deve suportar pelo menos 50 usuários simultâneos sem perda perceptível de desempenho.</td>
      <td>Desempenho</td>
      <td>Média</td>
      <td>Backlog</td>
    </tr>
    <tr>
      <td>RNF#08</td>
      <td>O código-fonte deve seguir convenções padronizadas e estar bem comentado.</td>
      <td>Manutenibilidade</td>
      <td>Média</td>
      <td>Backlog</td>
    </tr>
    <tr>
      <td>RNF#09</td>
      <td>Backend e frontend devem ser desacoplados em arquitetura em camadas.</td>
      <td>Manutenibilidade</td>
      <td>Média</td>
      <td>Backlog</td>
    </tr>
    <tr>
      <td>RNF#10</td>
      <td>O sistema deve apresentar interface intuitiva, acessível e responsiva.</td>
      <td>Usabilidade</td>
      <td>Alta</td>
      <td>Backlog</td>
    </tr>
    <tr>
      <td>RNF#11</td>
      <td>O sistema deve ser responsivo e adaptado para dispositivos móveis.</td>
      <td>Usabilidade</td>
      <td>Alta</td>
      <td>Backlog</td>
    </tr>
    <tr>
      <td>RNF#12</td>
      <td>Mensagens de erro devem ser claras e orientativas para o usuário.</td>
      <td>Usabilidade</td>
      <td>Média</td>
      <td>Backlog</td>
    </tr>
    <tr>
      <td>RNF#13</td>
      <td>O sistema deve estar estruturado para suportar expansão de funcionalidades sem perdas de desempenho.</td>
      <td>Escalabilidade</td>
      <td>Média</td>
      <td>Backlog</td>
    </tr>
    <tr>
      <td>RNF#14</td>
      <td>O banco de dados deve suportar crescimento contínuo dos registros financeiros.</td>
      <td>Escalabilidade</td>
      <td>Média</td>
      <td>Backlog</td>
    </tr>
    <tr>
      <td>RNF#15</td>
      <td>O sistema deve estar disponível 99% do tempo, com exceção de manutenções planejadas.</td>
      <td>Disponibilidade</td>
      <td>Alta</td>
      <td>Backlog</td>
    </tr>
    <tr>
      <td>RNF#16</td>
      <td>Em caso de erro, o sistema deve registrar logs e apresentar mensagem amigável ao usuário.</td>
      <td>Disponibilidade</td>
      <td>Média</td>
      <td>Backlog</td>
    </tr>
    <tr>
      <td>RNF#17</td>
      <td>O sistema deve possuir testes unitários com cobertura mínima de 80% no backend.</td>
      <td>Testabilidade</td>
      <td>Média</td>
      <td>Backlog</td>
    </tr>
    <tr>
      <td>RNF#18</td>
      <td>Os módulos devem ser testáveis de forma independente.</td>
      <td>Testabilidade</td>
      <td>Média</td>
      <td>Backlog</td>
    </tr>
  </tbody>
</table>





