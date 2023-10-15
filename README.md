# trilha-testes-manuais-funcionais
Com esse desafio, foi realizada toda a documentação e preparação de testes para o desenvolvimento de uma loja virtual.
Para maiores informações, consultar documento **Testes Manuais Funcionais.pdf**

Para isso, foram realizadas as seguintes etapas:

* Criação de um ambiente colaborativo **JIRA**
  
![image](https://github.com/ViniciusBenevidesdaSilva/trilha-testes-manuais-funcionais/assets/105802950/9ccae97c-cf55-44c4-975b-d18c11f837ea)

* Definição dos tipos de Item que compõem o projeto:
  
![image](https://github.com/ViniciusBenevidesdaSilva/trilha-testes-manuais-funcionais/assets/105802950/9229ab28-da28-45f5-ad90-507403a3d2e4)

## Planos de Fluxo de Trabalho
* Fluxo de trabalho

![image](https://github.com/ViniciusBenevidesdaSilva/trilha-testes-manuais-funcionais/assets/105802950/3f648c0c-03be-4cf5-89d8-d91dc944ecef)

* Ciclo de vida do Bug

![image](https://github.com/ViniciusBenevidesdaSilva/trilha-testes-manuais-funcionais/assets/105802950/960c5873-3781-4c90-83f0-507ba9eb7f67)

## Criação de User stories
1. Como usuário, desejo acessar a página de login na loja virtual a fim de visualizar as opções de login, cadastro e redefinição de senha

![image](https://github.com/ViniciusBenevidesdaSilva/trilha-testes-manuais-funcionais/assets/105802950/55d88a16-2d97-41d6-8d8f-69cf45113805)
![image](https://github.com/ViniciusBenevidesdaSilva/trilha-testes-manuais-funcionais/assets/105802950/4a1dc45a-0a39-4e43-bbea-45c65fe1fd7e)

2. Como usuário, desejo preencher o formulário para criação de conta na loja virtual, a fim de criar o meu cadastro de acesso

![image](https://github.com/ViniciusBenevidesdaSilva/trilha-testes-manuais-funcionais/assets/105802950/f20822a6-6410-4dd1-8350-fe9218f6253c)
![image](https://github.com/ViniciusBenevidesdaSilva/trilha-testes-manuais-funcionais/assets/105802950/bacc95c5-0a8c-4f89-bc39-30ab6399d4b7)

3. Como usuário, desejo acessar a página de login na loja virtual a fim de efetuar meu login no sistema

![image](https://github.com/ViniciusBenevidesdaSilva/trilha-testes-manuais-funcionais/assets/105802950/7227d078-fff5-4778-a3c1-bce04fa836dc)
![image](https://github.com/ViniciusBenevidesdaSilva/trilha-testes-manuais-funcionais/assets/105802950/60d47f8a-c63b-48d9-a1c2-e6ec2e2be86b)


## Mind-Maps
![image](https://github.com/ViniciusBenevidesdaSilva/trilha-testes-manuais-funcionais/assets/105802950/c3d2a66d-16a4-43ae-8a5c-16da4fc6374e)
![image](https://github.com/ViniciusBenevidesdaSilva/trilha-testes-manuais-funcionais/assets/105802950/a68f9cc5-5f84-4ce2-8998-8d8f2870a424)
![image](https://github.com/ViniciusBenevidesdaSilva/trilha-testes-manuais-funcionais/assets/105802950/553487db-d8e3-4c92-ab13-ef0efbbf7813)

## Ciclo de Testes
![image](https://github.com/ViniciusBenevidesdaSilva/trilha-testes-manuais-funcionais/assets/105802950/a10c86f9-7c6d-4afe-b0f4-f77ad9cc682b)

### US_1 – Navegação Login
1.	Cliente navega por entre as telas de login e cadastro

**Given** que o cliente esteja na tela de login **And** não esteja cadastrado no sistema, **When** clicar em 'Sign Up', **Then** será redirecionado para uma tela de criação de nova conta

2.	Cliente navega por entre as telas de login e Forgot your password

**Given** que o cliente esteja na tela de login **And** não esteja cadastrado no sistema, **When** clicar em 'Forgot your password', **Then** será redirecionado para uma tela de recuperação de senha

###	US_2 - Cadastro de usuário
1.	Cliente deixa campos em branco no cadastro

**Given** que o cliente esteja na tela de cadastro, **And** tenha deixado algum campo em branco, **When** clicar em 'Sign Up', **Then** receberá um alerta sobre o campo pendente

2.	Cliente informa senha com menos de 3 caracteres

**Given** que o cliente esteja na tela de cadastro, **And** tenha informado uma senha com menos de 3 caracteres, **When** clicar em 'Sign Up', **Then** receberá um alerta sobre a quantidade de caracteres da senha

3.	Cliente informa um username ou e-mail já cadastrado

**Given** que o cliente esteja na tela de cadastro, **And** tenha inserido um username ou e-mail já cadastrado, **When** clicar em 'Sign Up', **Then** receberá um alerta

4.	Cliente informar data de nascimento inválida

**Given** que o cliente esteja na tela de cadastro, **And** tenha preenchido uma senha posterior a data atual, **When** clicar em 'Sign Up', **Then** receberá um alerta

5.	Cliente preenche os dados de cadastro corretamente

**Given** que o cliente esteja na tela de cadastro, **And** tenha preenchido corretamente o formulário, **When** clicar em 'Sign Up', **Then** seu usuário será criado **And** ele será redirecionado para uma tela de login


###	US_3 - Login usuário
1.	Cliente com cadastro valido realiza login

  1° Passo: Acessar url https://www.saucedemo.com/v1/index.html
Resultado: Usuário deve visualizar tela de login

  2° Passo: Usuário digita username no campo 'username'
Dados de Teste: User_Test
Resultado: Sistema aguarda próxima etapa

  3° Passo: Usuário digita password no campo 'password'
Dados de Teste: Password_Test
Resultado: Sistema aguarda próxima etapa

  4° Passo: Usuário clica no botão 'Login'
Resultado: Sistema emite um alerta informando que o usuário é inválido

2.	Cliente com senha inválida tenta fazer login

  1° Passo: Acessar url https://www.saucedemo.com/v1/index.html
Resultado: Usuário deve visualizar tela de login

  2° asso: Usuário digita username no campo 'username'
Dados de Teste: User_Test
Resultado: Sistema aguarda próxima etapa

  3° Passo: Usuário digita password no campo 'password'
Dados de Teste: Password_Test
Resultado: Sistema aguarda próxima etapa

  4° Passo: Usuário clica no botão 'Login'
Resultado: Sistema emite um alerta informando que a senha é inválida

3.	Cliente sem cadastro tenta fazer login

  1° Passo: Acessar url https://www.saucedemo.com/v1/index.html
Resultado: Usuário deve visualizar tela de login

  2° Passo: Usuário digita username no campo 'username'
Dados de Teste: User_Test
Resultado: Sistema aguarda próxima etapa

  3° Passo: Usuário digita password no campo 'password'
Dados de Teste: Password_Test
Resultado: Sistema aguarda próxima etapa

  4° Passo: Usuário clica no botão 'Login'
Resultado: Direcionar usuário para url https://www.saucedemo.com/v1/inventory.html
