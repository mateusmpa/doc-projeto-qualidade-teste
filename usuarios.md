Epico Usuários

Funcionalidade: Cadastrar usuário
Eu como um usuário novo
Quero me cadastrar no site
Para criar uma conta personalizada
E salvar minhas informações de contato

Cenário: Cadastrar um novo usuário com tipo comprador
Dado que sou um visitante do site com interesse em comprar
Quando clico no botão "Cadastre-se"
Então devo ser redirecionado para a página de cadastro
E posso preencher o formulário com minhas informações pessoais
E posso marcar que "sou comprador"
E após preencher o formulário corretamente
Então devo ser registrado no site com uma conta personalizada

Cenário: Cadastrar um novo usuário do tipo vendedor
Dado que sou um visitante do site com interesse em vender
Quando clico no botão "Cadastre-se"
Então devo ser redirecionado para a página de cadastro
E posso preencher o formulário com minhas informações pessoais
E posso marcar que "sou vendedor"
E após preencher o formulário corretamente
E clicar no botão salvar
Então devo ser registrado no site com uma conta personalizada

Cenário: Cadastrar um novo usuário com dados inválidos
Dado que sou um visitante do site
Quando clico no botão "Cadastre-se"
Então devo ser redirecionado para a página de cadastro
E posso preencher o formulário com minhas informações pessoais
E após preencher o formulário com algum dado inválido
Então devo receber uma mensagem de "falha no cadastro"


Funcionalidade: Logar
Eu como um usuário cadastrado
Quero fazer login de forma segura
Para acessar minha conta

Cenário: Logar com dados de um usuário registrado
Dado que sou um usuário registrado
Quando acesso a página de login
E preencho meu nome de usuário e senha corretamente
Então devo ser redirecionado para a minha página de perfil
E devo estar logado na minha conta

Cenário: Logar com dados inexistentes
Dado que sou um usuário
Quando acesso a página de login
E preencho um nome de usuário e senha inexistentes
Então devo ser redirecionado para a página de login
E devo receber uma mensagem de falha na autenticação


Funcionalidade: Atualizar perfil
Eu como um usuário cadastrado
Quero poder atualizar meu perfil
Para manter meus dados pessoais atualizados

Cenário: Modificar cadastro
Dado que sou um usuário autenticado
Quando acesso minha página de perfil
E clico no botão editar
Então devo ser redirecionado para a página de edição de cadastro
E devo visualizar um formulário preenchido com minhas informações pessoais
E posso modificar minhas informações pessoais
E após preencher o formulário corretamente
E clicar no botão salvar
Então devo ser redirecionado para a minha página de perfil
E devo receber uma mensagem de sucesso na edição


Funcionalidade: Visualizar dados do vendedor
Eu como um usuário autenticado
Quero visualizar os dados de contato do vendedor
Para ter um meio de efetuar um contato

Cenário: Visualizar dados do vendedor quando autenticado
Dado que sou um usuário autenticado
Quando acesso a página de visualização de um veículo
Então devo visualizar os dados do vendedor

Cenário: Bloquear acesso aos dados do vendedor quando não autenticado
Dado que sou um usuário não autenticado
Quando acesso a página de visualização de um veículo
Então não devo visualizar os dados do vendedor


Funcionalidade: Recuperar senha
Eu como um usuário cadastrado
Quero poder recuperar minha senha
Para conseguir autenticar no site caso esqueça os dados de acesso

Cenário: Recuperar senha através de e-mail cadastrado
Dado que sou um usuário não autenticado
Quando acesso a tela de login
E clico no botão "Recuperar senha"
Então devo ser redirecionado para a tela de recuperar senha
E posso escolher a opção "e-mail cadastrado"
E posso inserir meu e-mail de cadastro
Então devo receber um e-mal contendo um link para definir uma nova senha


Funcionalidade: Deletar cadastro
Eu como um usuário cadastrado
Quero poder deletar meu cadastro
Para não ter meus dados salvos no site

Cenário: Confirmar a deleção de um cadastro com perfil de comprador
Dado que sou um usuário autenticado com perfil de comprador
Quando acesso minha página de perfil
E clico no botão "Deletar cadastro"
Então devo visualizar um popup perguntando se "quero confirmar a ação"
E posso escolher a opção "sim"
Então devo ser redirecionado para a tela inicial do site
E minha sessão deve ser deletada
E meu cadastro deve ser deletado

Cenário: Confirmar a deleção de um cadastro com perfil de vendedor
Dado que sou um usuário autenticado com perfil de vendedor
Quando acesso minha página de perfil
E clico no botão "Deletar cadastro"
Então devo visualizar um popup perguntando se "quero confirmar a ação"
E posso escolher a opção "sim"
Então devo ser redirecionado para a tela inicial do site
E minha sessão deve ser deletada
E meu cadastro deve ser deletado
E os veículos cadastros em meu nome devem ser deletados

Cenário: Iniciar deleção sem confirmar
Dado que sou um usuário autenticado
Quando acesso minha página de perfil
E clico no botão "Deletar cadastro"
Então devo visualizar um popup perguntando se "quero confirmar a ação"
E posso escolher a opção "não"
Então devo ser redirecionado para a minha página de perfil
