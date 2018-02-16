# Simples Hello World em Django

O projeto inclui um virtualenv na pasta djangohellovenv, que já inclui o Django versão 2.0.2. A execução do web app retorna uma página simples com o texto Hello World no navegador.

## Instalação
Clone este repositório em qualquer pasta de sua preferência

`git clone https://github.com/mateusmb/hellodjango.git`

## Utilização
Entre no repositório

`cd hellodjango`

Inicie o virtualenv

`source djangohellovenv/bin/activate`

Entre no diretório do projeto

`cd hellodjango`

Inicie o server do django

`python3 manage.py runserver`

Ou inicie o seu servidor http conforme as especificações do mantenedor

Acesse o seu browser, entrando no endereço http://127.0.0.1:8000 ou no endereço fornecido pelo seu serviço de hospedagem. Certifique-se de ver a mensagem Hello World!

## Estrutura
A raiz deste projeto tem duas pastas: djangohellovenv e hellodjango.

**djangohellovenv** - Arquivos e executáveis do virtualenv. Contém os executáveis do python e django.

**hellodjango** - Contém o projeto web com os arquivos de configuração e web apps. A página que exibe Hello World! é servida pelo app **hello** no diretório de mesmo nome.
Os arquivos editados neste projeto são:

**hellodjango/hellodjango/settings.py** - Incluído o app 'hello' na linha 40.

**hellodjango/hellodjango/urls.py** - Path do admin substituído pelo path para hello.urls na linha 20.

**hellodjango/hello/urls.py** -  Mapeada a view index.

**hellodjango/hello/views.py** - Uma view index criada que retorna uma página html simples.

**hellodjango/hello/templates/hello/index.html** - Diretório criado para conter os templates das páginas, o qual possui uma página simples que exibe Hello World!
