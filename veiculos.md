Histórias de veículos

Funcionalidade: Adicionar veículo
Eu como um vendedor
Quero poder adicionar novos veículos
Para que os usuários do site possam visualizá-los

Cenário: Adicionar um novo veículo com sucesso
Dado que estou logado como um vendedor
Quando eu preencho o formulário de adição de veículo
E clico no botão "Adicionar"
Então devo ver uma mensagem de confirmação de sucesso
E o novo veículo deve ser exibido na lista de veículos

Cenário: Tentativa de adicionar veículo sem informações obrigatórias
Dado que estou logado como um vendedor
Quando eu preencho o formulário de adição de veículo sem informações obrigatórias
E clico no botão "Adicionar"
Então devo ver uma mensagem de erro informando que os campos obrigatórios estão em branco
E o novo veículo não deve ser adicionado à lista de veículos


Funcionalidade: Atualizar veículos
Eu como um vendedor
Quero poder atualizar os dados dos meus veículos
Para manter seus dados atualizados

Cenário: Atualizar dados de um veículo com sucesso
Dado que estou logado como um vendedor
E tenho um veículo cadastrado
Quando eu selecionar o veículo para atualização
E preencher o formulário de atualização
E clicar no botão "Atualizar"
Então devo ver uma mensagem de confirmação de sucesso
E os dados do veículo devem ser atualizados

Cenário: Tentativa de atualizar veículo com informações inválidas
Dado que estou logado como um vendedor
E tenho um veículo cadastrado
Quando eu selecionar o veículo para atualização
E preencher o formulário de atualização com informações inválidas
E clicar no botão "Atualizar"
Então devo ver uma mensagem de erro informando que as informações são inválidas
E os dados do veículo não devem ser atualizados


Funcionalidade: Visualizar veículo
Eu como um usuário anonimo ou cadastrado
Quero ver os detalhes de um veículo
Para auxiliar na compra de veículos
Ou auxiliar na precificação

Cenário: Visualizar detalhes de um veículo
Dado que estou na página de listagem de veículos
Quando eu selecionar um veículo da lista
Então devo ver os detalhes do veículo
E devo ver informações adicionais, como quilometragem, cor, etc.


Funcionalidade: Deletar veículo
Eu como um vendedor
Quero poder deletar meus veículo
Para não ter seus dados salvos no site

Cenário: Deletar veículo com sucesso
Dado que estou logado como um vendedor
E tenho um veículo cadastrado com
Quando eu selecionar o veículo para deleção
E confirmar a ação de deleção
Então devo ver uma mensagem de confirmação de que o veículo foi deletado com sucesso
E o veículo não deve mais estar listado no site

Cenário: Cancelar a deleção de um veículo
Dado que estou logado como um vendedor
E tenho um veículo cadastrado
Quando eu selecionar o veículo para deleção
E optar por cancelar a deleção
Então devo ver uma mensagem de confirmação de que o veículo não foi deletado
E o veículo ainda deve estar listado no site

Cenário: Tentativa de deletar veículo sem confirmação
Dado que estou logado como um vendedor
E tenho um veículo cadastrado
Quando eu selecionar o veículo para deleção
E não confirmar a deleção
Então devo permanecer na página do veículo
E o veículo ainda deve estar listado no site


Funcionalidade: Pesquisar veículo
Eu como um usuário anonimo ou cadastrado
Quero poder pesquisar veículos por marca, modelo, ano e faixa de preço
Para visualizar as melhores possibilidades de compra
Ou visualizar em qual posição estão os meus veículos

Cenário: Pesquisar veículos por marca
Dado que estou na página de pesquisa de veículos
Quando eu selecionar a opção de pesquisa por marca e inserir "Toyota"
E clicar no botão "Pesquisar"
Então devo ver uma lista de veículos da marca "Toyota" exibida
E cada veículo na lista deve ter a marca "Toyota"

Cenário: Pesquisar veículos cadastrados pelo vendedor
Dado que estou logado como um vendedor
E tenho veículos cadastrados no sistema
Quando eu acessar a página de pesquisa de veículos
E selecionar a opção "Meus Veículos"
Então devo ver uma lista dos veículos que cadastrei anteriormente
E cada veículo na lista deve pertencer ao meu perfil de usuário
