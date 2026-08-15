
# Requirements

## 1. Problema

* **Qual problema o sistema precisa resolver?**
Os clientes de uma concessionária não têm onde registrar suas avaliações, e principalmente usuários novos não têm acesso a avaliações que poderão ser determinantes na compra do seu carro. E como não tem onde postar as avaliações, causa desconfiança por parte dos usuários.
* **Quem possui esse problema?**
Concessionária OmniDrive e os seus prospects.
* **Qual resultado o sistema precisa proporcionar?**
Exibir avaliações reais na tela do usuário visitante, permitindo que o usuário se cadastre, filtre até a sua concessionária e consiga colocar sua avaliação.

---

## 2. Usuários

* **Quem utilizará o sistema?**
Usuários Visitantes, Usuários Cadastrados e Admins do site.
* **Quais tipos de usuários existem?**
1. Usuário Visitante
2. Usuário Cadastrado
3. Usuário Administrador


* **O que cada tipo de usuário precisa conseguir fazer?**
* **Usuário Visitante:** Pode ler avaliações do site, entrar em contato conosco, ver informações sobre nós (página Fale Conosco e Sobre Nós), filtrar a lista de filiais por estado e ver as avaliações daquelas filiais.
* **Usuário Cadastrado:** Pode ler e criar novas avaliações sobre o produto e serviço da filial onde fez negócios.
* **Usuário Administrador:** Pode colocar novos produtos e seus atributos (adicionar informações do veículo), e ver as avaliações da sua filial para tomar decisões de negócios.


* **Existem ações que apenas determinados usuários podem executar?**
* **Usuários Visitantes:** NÃO podem avaliar, só ler.
* **Usuários Cadastrados:** Podem criar avaliações (se tiverem fechado compra/negócio), mas NÃO podem adicionar marca, modelo ou qualquer outro atributo da concessionária e filiais.
* **Usuário Administrador:** É o único com poder de adicionar novos veículos bem como seus atributos, mas por questões de transparência e ética NÃO pode cadastrar avaliações.



---

## 3. Funcionalidades

### Consultar informações institucionais

* **Quem precisa dessa funcionalidade?** Visitantes e Clientes.
* **Qual necessidade ela atende?** Visitantes e Clientes desejam saber mais sobre a rede de concessionárias.
* **O que o usuário precisa fazer?** Clicar na página Fale Conosco e página Sobre Nós.
* **Qual informação ele precisa fornecer?** Clique.
* **O que o sistema deve fazer?** Navegador carrega as informações.
* **Qual resultado o usuário deve receber?** Página exibida com as informações.
* **Como eu saberia que a funcionalidade está funcionando?** Quando a página mostrar para ele as informações.

### Consultar concessionária

* **Quem precisa dessa funcionalidade?** Visitantes e Clientes.
* **Qual necessidade ela atende?** Visitantes e Clientes desejam encontrar a concessionária mais próxima, seus produtos e avaliações.
* **O que o usuário precisa fazer?** Fazer o filtro por estado.
* **Qual informação ele precisa fornecer?** Filtrar a Cidade/Estado da Filial a ser filtrado.
* **O que o sistema deve fazer?** Servidor filtra o estado e retorna as concessionárias daquele estado.
* **Qual resultado o usuário deve receber?** As concessionárias daquele estado (ou de todos se não houver preenchido o campo estado), com nome, endereço e informações daquela concessionária.
* **Como eu saberia que a funcionalidade está funcionando?** As concessionárias serem exibidas e uma mensagem de sucesso com o número de concessionárias encontradas.

### Consultar Avaliações

* **Quem precisa dessa funcionalidade?** Visitantes e Clientes.
* **Qual necessidade ela atende?** Visitantes e Clientes desejam verificar as avaliações de um modelo ou concessionária específica para decidir se vão fazer negócio.
* **O que o usuário precisa fazer?** Selecionar uma concessionária para ver as avaliações.
* **Qual informação ele precisa fornecer?** Selecionar a concessionária desejada.
* **O que o sistema deve fazer?** Buscar e carregar as avaliações da concessionária selecionada.
* **Qual resultado o usuário deve receber?** Avaliações reais da concessionária selecionada exibidas na tela.
* **Como eu saberia que a funcionalidade está funcionando?** Quando o usuário conseguir ver as avaliações daquela filial.

### Autenticar (Login e Cadastro)

* **Quem precisa dessa funcionalidade?** Clientes e Admins.
* **Qual necessidade ela atende?** Fator determinante para que um usuário consiga se cadastrar (se tiver feito negócio com a concessionária) e para um usuário admin conseguir gerenciar o site e adicionar novos produtos.
* **O que o usuário precisa fazer?** Acessar a página de login/cadastro e preencher os campos.
* **Qual informação ele precisa fornecer?** Dados para cadastro e/ou login (dados administrativos com usuário e senha predefinida para admins; ou dados de negócio/cliente para cadastro).
* **O que o sistema deve fazer?** Servidor verifica se está cadastrado (como cliente ou admin) ou se é cliente para poder se cadastrar.
* **Qual resultado o usuário deve receber?** Para o cadastro/login, a página de perfil com suas avaliações (clientes) ou páginas administrativas (adm).
* **Como eu saberia que a funcionalidade está funcionando?** O usuário conseguir acessar a área correspondente ao seu perfil.

### Publicar avaliações

* **Quem precisa dessa funcionalidade?** Clientes cadastrados.
* **Qual necessidade ela atende?** Clientes desejam demonstrar suas opiniões quanto ao produto e serviço de um modelo e uma concessionária com a qual fizeram negócios.
* **O que o usuário precisa fazer?** Clicar no botão de avaliar ao lado da concessionária que ele negociou.
* **Qual informação ele precisa fornecer?** Concessionária, modelo para avaliar, seu comentário e estrelas.
* **O que o sistema deve fazer?** Registrar a avaliação e associá-la à página de avaliações daquela concessionária.
* **Qual resultado o usuário deve receber?** A avaliação dele aparece na página de avaliações daquela concessionária e uma mensagem de sucesso.
* **Como eu saberia que a funcionalidade está funcionando?** Quando ele conseguir ver a avaliação publicada na página e receber a mensagem de sucesso.

### Cadastrar novos veículos

* **Quem precisa dessa funcionalidade?** Usuários Administradores.
* **Qual necessidade ela atende?** Usuários admins desejam cadastrar veículos e consórcios para tornar mais atrativo novos clientes.
* **O que o usuário precisa fazer?** Clicar no botão de adicionar modelo.
* **Qual informação ele precisa fornecer?** Dados do veículo e seus atributos.
* **O que o sistema deve fazer?** Processar e registrar o novo veículo no catálogo do sistema.
* **Qual resultado o usuário deve receber?** Página do veículo cadastrado exibida na página da concessionária.
* **Como eu saberia que a funcionalidade está funcionando?** O novo veículo e seus atributos aparecerem listados corretamente.

---

## 4. Regras

* **Regra de Cadastro de Cliente:** O usuário só pode se cadastrar se tiver feito negócios com a concessionária, pois não faz sentido avaliar algo com que nunca teve contato.
* **Regra de Permissão de Avaliação:** Apenas usuários cadastrados (clientes que fecharam negócio) podem criar avaliações. Visitantes só podem ler.
* **Regra de Restrição de Administrador:** O usuário administrador é o único com poder de adicionar novos veículos e atributos, mas por questões de transparência e ética NÃO pode cadastrar avaliações.
* **Regra contra Spam e Fraude:**
* Se qualquer usuário novo pudesse criar avaliações, haveria muito spam e baixaria a credibilidade do site.
* Se qualquer usuário cadastrado ou visitante pudesse criar novos veículos, poderia fornecer informações falsas e usar de má-fé, baixando a transparência da empresa.


* **Tratamento de Exceções e Condições Não Atendidas:**
* **Filtro sem resultado:** Se não existir uma concessionária no filtro, deve exibir uma página dizendo que não houve resultado.
* **Tentativa de avaliação sem compra:** Se o usuário tentar avaliar uma concessionária com a qual não fez negócios, deve mostrar uma página ou alerta falando que ele só pode avaliar a concessionária que negociou.
* **Tentativa de avaliação por Admin:** Se o administrador tentar avaliar, o sistema deve emitir uma página de erro lembrando que ele é admin e não pode avaliar.



---

## 5. Critérios de aceitação

* **Consultar Institucional:** O usuário clica na página Fale Conosco ou Sobre Nós e o sistema exibe corretamente a página com as informações.
* **Filtrar Concessionárias:** O usuário seleciona o estado no filtro e o sistema exibe as concessionárias daquele estado acompanhadas de mensagem de sucesso com o número de concessionárias encontradas. Se não houver, exibe página sem resultados.
* **Visualizar Avaliações:** O visitante ou cliente clica na concessionária e visualiza as avaliações reais cadastradas na tela.
* **Autenticação:** O cliente/admin fornece seus dados, o sistema valida e redireciona o cliente para seu perfil/avaliações e o admin para a área administrativa.
* **Publicar Avaliação:** O cliente cadastrado clica no botão de avaliar ao lado da concessionária que negociou, preenche o comentário/estrelas e, ao enviar, recebe mensagem de sucesso e vê a avaliação publicada na página.
* **Cadastrar Veículos:** O admin fornece os dados do veículo, clica em adicionar modelo e o novo produto passa a ser exibido na página da concessionária.

---

## 6. Dúvidas

* *Como o sistema vai validar se o usuário realmente fechou negócio com a concessionária antes de permitir o cadastro/avaliação?*


* *Quais são exatamente os atributos obrigatórios que o Administrador precisa fornecer ao cadastrar um novo veículo?*