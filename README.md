#  Desempregando

## Telas da Aplicação 
**TELA 1 -
  Esta é a tela de Inicio e ao clicar em  Login/cadastro poderá ir para a tela de cadastro**
<p align="center" ><img src="test/inicio.png" width="800"></a><//>
      
**TELA 2 -
  Ao clicar em login/cadastro aparecerá a tela de LOG IN , caso usuário já estiver cadastrado basta acessar com e-mail e senha , caso não tenha cadastro acesse o "Cadastrar" .**
<p align="center" ><img src="test/login.png" width="800"></a><//>

**TELA 3 - 
  Esta tela o usuário poderá se cadastrar**
<p align="center" ><img src="test/signup.png" width="800"></a><//>

**TELA 4 -
  Esta é a tela principal que o usuário terá acesso ao realizar o Login.**
<p align="center" ><img src="test/Telalogin.png" width="800"></a><//>

**TELA 5 -
  Clicando em _ver mais_ o usuário terá as opções de cadastrar-se  e compartilhar a vaga**
<p align="center" ><img src="test/Cadastrar.png" width="800"></a><//>

**TELA 6 -
  Clicando em _Minha empresa_ o usuário pode cadastrar  a empresa , com o nome site e logo da empresa**
<p align="center" ><img src="test/criarempresa.png" width="800"></a><//>

**TELA 7 -
  Clicando em _Publicar vaga_ o usuário poderá publicar as vagas oferecidas pela empresa**
<p align="center" ><img src="test/vaga.png" width="800"></a><//>

**TELA 8 -
  Clicando em _Minhas vagas_ o usuário poderá ter acesso as vagas publicadas**
<p align="center" ><img src="test/minhasvagas.png" width="800"></a><//>


## Link do repositório
Use esse link  (https://github.com/Queenlife822/copy_Desempregando_DPre)



## Executem os comando

### docker-compose run --no-deps app rails new . --force --database=postgresql --webpacker

#ERROR
Fetching gem metadata from https://rubygems.org/.
You have requested:
  listen ~> 3.2

The bundle currently has listen locked at 3.1.5.
Try running `bundle update listen`

If you are updating multiple gems in your Gemfile at once,
try passing them all to `bundle update`
ERROR: 7
➜  teste bundle update listen
Could not find gem 'listen'.
➜  teste bundle update       
Your Ruby version is 3.0.2, but your Gemfile specified 2.7.8

## Comando para correção do erro
docker-compose run app bundle update

## Proximos comandos

$ sudo chown -R $USER:$USER .

$ sudo docker-compose up --build

## Configura Database

config/database.yml

## Subir a máquina

docker-compose up -d

## Criar o banco de dados

$ docker-compose run app rails db:create

## Se necessário instalar o yarn
https://classic.yarnpkg.com/en/docs/install/#debian-stable

## Comando pra rodar após incluir as Gems caso de errado e solicite alguma depedência

sudo docker-compose run app bundle exec figaro install

## Atualização da Gem

docker-compose run app bundle install

## Instalando Simple_form
docker-compose run app rails generate simple_form:install --bootstrap

## Instalando Devise
docker-compose run app rails generate devise:install

## Instalando e convertendo erb to haml

### Executar primeiro
docker-compose run app gem install html2haml

docker-compose run app rails generate haml:application_layout convert

### Executar
docker-compose run app rails haml:erb2haml