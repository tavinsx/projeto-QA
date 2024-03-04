_1 - Como usuário mobile, quero fazer login no aplicativo_

Critérios de aceitação

- O usuário deve ser capaz de inserir suas credenciais (e-mail e senha).
- O aplicativo deve verificar se as credenciais são válidas.
- Se as credenciais forem válidas, o usuário deve ser redirecionado para a tela principal do aplicativo.
- Se as credenciais forem inválidas, o usuário deve receber uma mensagem de erro.

_2 - Como usuário mobile, quero redefinir minha senha_

criterios de aceitação:

- na pagina de login deve haver a opção de redefinir senha.
- deve ocorrer a solicitação do gmail associado a conta do cliente.
- o envio do link de redefinição de senha.
- o link deve expirar após um periodo de tempo. 

_3 - Como usuário mobile, quero criar uma nova conta_

criterios de aceitação:

- deve haver a opção de fazer login com uma nova conta. 
- o usuario deve fornecer o novo nome, gmail e senha.
- o aplicativo deve verificar se os dados inseridos já estão associados a uma conta.
- se for válido, cria a nova conta, e redireciona para a pagina principal.
- caso seja inválido, aparecer mensagem de erro, "conta ja existente"

_Caso de Teste para Login:_

- O aplicativo está instalado e aberto.
- Insira um e-mail e senha válidos.
- Clique no botão “Login”.
- verificar se é válido.
- caso seja inválido, aparecer uma mensagem de erro.
- pedir para conferir as informações inseridas.


_Caso de Teste para Redefinir Senha:_
- Clique na opção “Esqueci minha senha”.
- Insira o e-mail associado à conta.
- Verifique se o e-mail recebido está associado a conta.
- enviar o link de redefinição.

_Caso de Teste para Criar Nova Conta:_
- Clique na opção “Criar nova conta”.
- Preencha os campos obrigatórios (nome, e-mail, senha).
- Clique no botão “Registrar”.
- verificar se já não tem uma conta com essas informações.
- se for válido, criar a nova conta.
- caso for inválido aparecer mensagem de erro, ""conta ja existente".

_Step 3 - Imagine que existe o seguinte bug:_ Um usuário pode criar uma conta para um e-mail associado a outro usuário.
Por favor, reporte este bug com detalhes e sugestões sobre como devemos corrigir o problema

Passos para Reproduzir:

- Abra o aplicativo.
- Clique na opção “Criar Nova Conta”.
- Insira um e-mail que já está associado a outra conta.
- Complete o processo de criação da conta.

Resultado Esperado:

- O sistema deve validar se o e-mail fornecido é único e não está associado a nenhuma outra conta.
- Se o e-mail já estiver em uso, o usuário deve receber uma mensagem de erro informando que o e-mail não pode ser duplicado.
- O sistema não deve permitir a criação da conta com um e-mail já existente.

Sugestões para Correção:

_Validação de E-mail Único:_
- Antes de permitir que um usuário crie uma nova conta, verifique se o e-mail fornecido não está associado a nenhuma outra conta existente.
- Se o e-mail já estiver em uso, exiba uma mensagem de erro informando ao usuário que o e-mail não pode usado, pois já esta registrado a uma conta.

_Notificação de Conta Existente:_

- Se um usuário tentar criar uma conta com um e-mail já existente, notifique-o de que a conta já está registrada.
- Forneça opções para redefinir a senha ou fazer login com a conta existente.


