# Projeto base de um Crud de Clientes usando Django com Bootstrap.
Este projeto tem objetivo de auxiliar o aluno na criação do seu primeiro projeto usando a linguagem de programação Python com Framework Django com DRF (Django Rest Framework).

Professor: [Alann Perini](https://github.com/AlannKPerini).

 Este tutorial assume que você já tem o Python instalado em seu computador. Se você ainda não tem o Python instalado, faça o download e siga as instruções de instalação em https://www.python.org/downloads/.

As orientações a seguir são destinadas ao Sistema Operacional **Windows**. Caso esteja utilizando um sistema operacional diferente e deseje obter informações detalhadas sobre a instalação, consulte a documentação do [PIP](https://pip.pypa.io/en/stable/installation/), que será o gerenciador utilizado neste projeto.

Para usuários de distribuições **Linux**, recomendamos consultar a documentação específica correspondente à sua distribuição para obter instruções detalhadas.

# Tecnologias envolvidas neste projeto de Desenvolvimento Web

**PIP:** Por padrão o pip já vem instalado no seu Python e ele é um gerenciador de pacotes no Python, então ele vai gerenciar as bibliotecas que você vai instalar, desinstalar e atualizar. Ele aumenta seu fluxo de trabalho de desenvolvimento em vários aspectos. 

**DJANGO:** O Django é um framework web Python de código aberto, que se destaca por oferecer um ambiente que simplifica a criação de soluções web escaláveis, ao mesmo tempo, em que promove o desenvolvimento rápido e um design limpo, proporcionando ferramentas robustas e eficientes para pessoas desenvolvedoras.

**BOOTSTRAP:** Bootstrap é um framework front-end que fornece estruturas de CSS para a criação de sites e aplicações responsivas de forma rápida e simples. Além disso, pode lidar com sites de desktop e páginas de dispositivos móveis da mesma forma.

**SQLite:** Banco de dados relacional, utilizado no ambiente de desenvolvimento.  Formado por uma biblioteca em linguagem C, o SQLite é um dos bancos de dados relacional mais conhecidos, por ser capaz de criar uma estrutura com um banco de dados embutido.

# Processo de Instalação e configuração Inicial do Ambiente de Desenvolvimento Django.

# Passo 1: Instalação do Django e do PIP

**Crie uma pasta para seu projeto com o nome projeto_django_bosch**

**Abra a pasta no Vscode e siga as instruções**

**Abra o terminal do VSCode e digite os comandos listados abaixo.**

# Instalação e configuração do PIP

**1.1 Instalação do PIP no Windows**

-   Abra um terminal, (No Terminal do `VS Code`):

    `Ctrl + Alt + T`

-   Verifique se tem o **PIP** está instalado na máquina e qual a versão:

```shell
pip -V
```
**Caso não encontre faça a instalação do PIP no Windows**

Execute o comando abaixo no **PowerShell** (No Terminal do `VS Code`):

```shell
 pip install
```
**Após executar os comandos acima, reinicie o terminal, e verifique se o PIP está instalado e se precisa fazer uma atualização, neste caso vc executa o seguinte comando**

```shell
 python.exe -m pip install --upgrade pip
```
**1.2 Crie um ambiente virtual para instalação e configuração do seu projeto através das depedências e bibliotecas espefíficas.**

O módulo usado para criar e gerenciar ambientes virtuais é chamado venv. O venv normalmente irá instalar a versão mais recente de Python que você tiver disponível.

```shell
  py -m venv venv
```

**Após a criação da máquina virtual vcocê deverá ativar para continuar a configuração do seu projeto. Utilize o seguinte comando:**

```shell
  venv\Scripts\activate
```
Deverá aparrecer **(venv)** em verde após e execução do código anterior.

# Instalação do Django

**1.2.3 Instale o Django usando o PIP (Python Package Installer). Execute o seguinte comando:**

``` shell
pip install Django
```
**1.2.4 Verifique se a instalação foi bem-sucedida digitando o seguinte comando para exibir a versão do Django instalada:**
``` shell
django-admin --version
```

# Criação de uma aplicação 

- Criação de uma aplicação do projeto Django chamada **empresa**

``` shell
django-admin  startproject empresa .
```
**Compreendendo uma aplicação**
Uma aplicação no Django é um conjunto de arquivos e pastas que contém o código de uma funcionalidade específica do seu site.

Uma aplicação pode ser criada dentro de um projeto ou importada de outro projeto.

Em nosso projeto, temos uma aplicação criada, chamada empresa, conforme a imagem abaixo:

 ![](/img/img1.PNG)

Após criar a aplicação clientes você verá que foi criada várias pastas, essas pastas e arquivos fazem parte do Django.

# Executando o Servidor

-  **Utilize o comando abaixo para executar o projeto de aplicação web, digite no terminal**

``` shell
python manage.py runserver
```
Se foi criado tudo certo até o momento, deverá ser executado indicando a seguinte mensagem no terminal.

**Django version ?.?.?, using settings 'clientes.settings'**

**Starting development server at http://127.0.0.1:8000/**   

Esse é o número do servidor web local(padrão) para abrir a aplicação web. Toda vez que precisar executar a aplicação preciso iniciar o servidor. 

-   Verifique se o projeto está rodando:

    -   Página inicial: http://localhost:8000
    -   `Admin`: http://localhost:8000/admin

-   Ao rodar o projeto pela primeira vez, o arquivo `db.sqlite3` é criado conforme a imagem abaixo. 

   ![](/img/banco.PNG)

-   Também aparecem mensagens de erro importantes.
-   Abra o arquivo `db.sqlite3` dentro do **VS Code**.
-   Verifique que ele ainda não possui nenhuma tabela.

Você deverá clicar e abrir em um navegador a aplicação Django. 

Para sair fechar a aplicação no servidor é só usar o seguinte atalho: 

`Ctrl + C`

# Instalação e sincronização de extensões do VS Code

Eu recomendo as seguintes:

-   [Django(Formatação de código)](https://marketplace.visualstudio.com/items?itemName=batisteo.vscode-django)
-   [SqLite Viewer (Visualização de bancos de dados SQLite)](https://marketplace.visualstudio.com/items?itemName=alexcvzz.vscode-sqlite)
-   [isort (Organização de imports)](https://marketplace.visualstudio.com/items?itemName=Tyriar.sort-lines)
-   [Black Formatter(Formatação de código)](https://marketplace.visualstudio.com/items?itemName=ms-python.vscode-pylance)
-   [Git Extension Pack(Trabalhando com GitHub)](https://marketplace.visualstudio.com/items?itemName=donjayamanne.git-extension-pack)
-   [ESLint (JavaScript)](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint)
-   [Intellicode (Desenvolvimento Inteligente)](https://marketplace.visualstudio.com/items?itemName=VisualStudioExptTeam.vscodeintellicode)
-   [Markdown All in One (Edição de arquivos Markdown)](https://marketplace.visualstudio.com/items?itemName=yzhang.markdown-all-in-one)
-   [Material Icon Theme (Temas de ícones)](https://marketplace.visualstudio.com/items?itemName=PKief.material-icon-theme)
-   [Peacock (Personalização de cores)](https://marketplace.visualstudio.com/items?itemName=johnpapa.vscode-peacock)
-   [Portuguese (Brazil) Language Pack for Visual Studio Code (Tradução para Português da interface do VS Code)](https://marketplace.visualstudio.com/items?itemName=MS-CEINTL.vscode-language-pack-pt-br)


# Arquivos de configuração da aplicação

O projeto vem com alguns arquivos de configuração pré-configurados, como:

- `settings.py:` Arquivo de configuração do Django.
- `manage.py`: é o arquivo que você usa para executar comandos do **Django**.
- `urls.py:` Arquivo de configuração das rotas do Django.
- `.gitignore:` Arquivo de configuração do Git, para ignorar arquivos e diretórios.
-  `db.sqlite3`: é o arquivo de banco de dados do projeto.
-  O arquivo `__init__.py` é um arquivo que indica que a pasta é um pacote Python. Ele vai aparecer em todas as pastas que contêm código Python. Muitas vezes, ele é um arquivo vazio.
  
Posteriormente, iremos modificar esses arquivos, bem como incluir alguns arquivos novos.

  Vamos abrir cada um desses arquivos e verificar para que eles servem.

Abra o arquivo **`settings.py:`** para alteração do idioma  e o horário padrão do Django. Faça a alteração conforme o exemplo abaixo:

```shell
LANGUAGE_CODE = 'pt-br'

TIME_ZONE = 'America/Sao_Paulo'

USE_I18N = True

USE_TZ = True
```
# Formatação de código com isort , black e pre-commit

As ferramentas de formatação de código `isort` e `black` são muito úteis para manter o código Python organizado e legível. Enquanto o `isort` organiza as importações, o `black` formata o código, seguindo as convenções do PEP8.

Além disso temos o `pre-commit` que é um framework que permite fazer várias verificações antes de commitar um código.

É possível adicionar diversos plugins ao seu pipeline de verificação do pre-commit. Quando um commit for dado, o pipeline roda todas as verificações e, se houver alguma falha, o commit não é feito, alertando o que está inconsistente.

-   Instale as ferramentas de desenvolvimento  `isort` , `black` e `pre-comit` :

```shell
pip install isort
```

```shell
pip install black
```

```shell
pip install pre-commit
```

-   Crie um arquivo `.isort.cfg` na raiz do projeto:

```shell
touch .isort.cfg
```

-   Abra o arquivo `.isort.cfg` e coloque o seguinte conteúdo:

```python
[isort]
default_section = THIRDPARTY
known_first_party = config  # change it for the name of your django project
known_django = django
sections = FUTURE,STDLIB,DJANGO,THIRDPARTY,FIRSTPARTY,LOCALFOLDER

[settings]
profile=black
skip=.git, __init__.py, __pypackages__/
```

**Usando o isort e o black**

Caso queira executar o isort e o black, basta colocar o nome do script que quer exucutar as funções e executar o código:

```shell
isort nome_do_script.py
black nome_do_script.py
```

Opcionalmente, você pode utilizador o formatador de código em um arquivo, selecionando o código (`Ctrl` + `A`) e pressionando `Ctrl + Shift + I`.

# Crie o arquivo **.gitignore**

Arquivo de configuração do Git, para ignorar arquivos e diretórios.
O arquivo .gitignore é um arquivo de texto que diz ao 
Git **quais arquivos ou pastas ele deve ignorar em um projeto.**
Um arquivo .gitignore local geralmente é colocado no diretório raiz de um projeto. 

Você também pode criar um arquivo .gitignore global e todas as entradas que estiverem naquele arquivo serão ignoradas em todos os seus repositórios do Git.

Você poderá usar o site (https://www.toptal.com/developers/gitignore) para criar o script dos seus arquivos.


# Passo 2: Criação de uma Aplicação Django , neste exemplo nossa aplicação terá o nome de Clientes

- Agora, crie um aplicativo dentro do projeto empresa. 

- Os aplicativos são componentes reutilizáveis do Django que podem conter modelos, visualizações, URLs e templates. 

- Neste exemplo, vamos criar uma aplicação chamada "clientes":

``` shell 
python manage.py startapp clientes
  ```
ou 
``` shell 
py manage.py startapp clientes
  ```

Após a criação da aplicação Clientes, foi criada uma pasta com todos os arquivos de configuração do Django para sua aplicação funcione.  

![](/img/img2.PNG)

Dentro da pasta core temos alguns arquivos e pastas, mas os mais importantes são:

- `migrations:` é a pasta de migrações de banco de dados da
aplicação.
- `models:` é a pasta onde ficam as models (tabelas) da aplicação.
- `views:` é a pasta onde ficam as views da aplicação.
- `admin.py:` é o arquivo de configuração do Admin, uma ferramenta que permite que você gerencie os dados do seu site.

O arquivo `__init__.py` é um arquivo que indica que a pasta é um pacote Python. Ele vai aparecer em todas as pastas que contêm código Python. Muitas vezes, ele é um arquivo vazio.

Abra o arquivo **settings.py** no diretório do projeto (empresa) e adicione o nome do aplicativo "clientes" à lista **INSTALLED_APPS:**

  ``` shell 
INSTALLED_APPS = [
    # ...
    'clientes',
    # ...
]
  ```

# Passo 3: Definir o Modelo de Cliente:

Nesta etapa iremos configurar nossa classe Cliente com os seguintes atributos: **Nome do Cliente , Endereço, Cpf, Data de Nascimento.**

Iremos seguir o tipo de variáveis conforme o tipo do atributo. Veja o exemplo a seguir: 

Abra o **arquivo clientes/models.py** e defina o modelo de Cliente:

  ``` shell
from django.db import models

class Cliente(models.Model):
    nome = models.CharField(max_length=100)
    endereco = models.TextField()
    cpf = models.CharField(max_length=14, unique=True)
    data_nascimento = models.DateField()

    def __str__(self):
        return self.nome
  ```


# Passo 4: Depois de definir o modelo, execute as migrações para criar a tabela no banco de dados:

O comando `makemigrations` analisa se foram feitas mudanças nos modelos e, em caso positivo, cria novas migrações `(Migrations)` para alterar a estrutura do seu banco de dados, refletindo as alterações feitas.

Portanto, toda vez que você alterar o seu modelo `(models.py)`, não se esqueça: execute `python manage.py makemigrations`.

- No terminal vc precisa digitar os seguintes comandos para executar as migrações.

``` shell
python manage.py makemigrations
  ```
- Agora na sequência execute o código abaixo para efetivar as novas migrações no sistema e banco.

``` shell
python manage.py migrate
  ```

# Passo 5: Criar um Formulário para Cliente:

Crie um arquivo `forms.py` para podermos gerar um formulário personalizado em **clientes/forms.py:**
Após criar o arquivo utilize os código abaixo com a estrutura definida para clientes. 

``` shell
from django import forms
from .models import Cliente

class ClienteForm(forms.ModelForm):
    class Meta:
        model = Cliente
        fields = ['nome', 'endereco', 'cpf', 'data_nascimento']
```

# Passo 6: Criar uma View para o CRUD Clientes:

- Em **clientes/views.py**, crie views para listar, criar, editar e excluir clientes:

- Estas são as rotinas básicas do `CRUD (Create,Read,Update,Delete)` aonde fazemos toda manipulação do sistema, neste caso, faremos na  classe Cliente.

``` shell
from django.shortcuts import render, redirect, get_object_or_404
from .models import Cliente
from .forms import ClienteForm

def lista_clientes(request):
    clientes = Cliente.objects.all()
    return render(request, 'clientes/lista_clientes.html', {'clientes': clientes})

def cria_cliente(request):
    if request.method == 'POST':
        form = ClienteForm(request.POST)
        if form.is_valid():
            form.save()
            return redirect('lista_clientes')
    else:
        form = ClienteForm()
    return render(request, 'clientes/cria_cliente.html', {'form': form})

def edita_cliente(request, pk):
    cliente = get_object_or_404(Cliente, pk=pk)
    if request.method == 'POST':
        form = ClienteForm(request.POST, instance=cliente)
        if form.is_valid():
            form.save()
            return redirect('lista_clientes')
    else:
        form = ClienteForm(instance=cliente)
    return render(request, 'clientes/edita_cliente.html', {'form': form})

def deleta_cliente(request, pk):
    cliente = get_object_or_404(Cliente, pk=pk)
    cliente.delete()
    return redirect('lista_clientes')
```

# Passo 7: Configurar URLs:

Em `**clientes/urls.py**`, defina as URLs para as views:

Crie um arquivo `urls.py` para podermos gerar as rotas personalizadas em `**clientes/urls.py:**`

As Urls são as rotas para que o sistema identifique aonde procruar as rotinas de sistema que acabamos de criar no passo 6.

A diante vamos criar os templates de Front-End para manipular todo nosso sistema, mas antes conseguios definir os nome dos formulários e páginas que terão em nosso sistemas.

``` shell
from django.urls import path
from . import views

urlpatterns = [
    path('', views.lista_clientes, name='lista_clientes'),
    path('clientes/', views.lista_clientes, name='lista_clientes'),  # URL para listar clientes
    path('novo/', views.cria_cliente, name='cria_cliente'),
    path('editar/<int:pk>/', views.edita_cliente, name='edita_cliente'),
    path('deletar/<int:pk>/', views.deleta_cliente, name='deleta_cliente'),
]

```

# Desenvolvendo o FRONT END do projeto
# Passo 8: Criação de Templates HTML:

Neste ponto nós temos uma **`Estrutura BackEnd`** pronta para ser usada mas precisamos do Tela para que o usuário possa fazer as interações com o Sistema que acabamos de criar.

Para isso a princípio vamos utilizar uma formatação básica de Html e Css para criação de páginas de Internet usando o **`Bootstrap.`**

- **Crie uma pasta chamada `templates` no diretório do aplicativo `"clientes"`. Dentro da pasta templates, `crie outra pasta chamada clientes`.**

- Crie templates HTML em **`clientes/templates/clientes`** para listar, criar, editar e excluir clientes. Você pode usar o **Bootstrap** ou outros estilos CSS para estilizar os templates, conforme necessário.

O link para acesso ao BootStrap é: 
https://getbootstrap.com/docs/5.3/getting-started/introduction/

ou https://www.w3schools.com/bootstrap5/index.php

- Segue o modelo de estrutura de pastas que ficará após essas orientações. 

![](/img/telasweb.PNG)

Na pasta templates vamos criar um arquivo que servirá de base para todo nosso projeto. 

- **`base.html`** Template base para todo projeto. Essa estrutura será replicada para todo os outros arquivos htmls criado neste projeto.

Os demais arquivos HTMl segue as instruções abaixo. 

Usaremos os seguintes modelos para templates de Clientes, crie cada arquivo HTML conforme os nomes abaixo:

- **`lista_clientes.html`** Template para listar clientes.

- **`cria_cliente.html`** Template para criar um novo cliente.

 - **`edita_cliente.html`** Template para editar um cliente existente.

- **`exclui_cliente.html`** Template para confirmar a exclusão de um cliente.

Em cada template HTML, estenda o template "base.html" e defina o conteúdo específico para cada página. Por exemplo, em lista_clientes.html:


# Código do arquivo base.html:


``` shell
<!DOCTYPE html>
<html lang="pt">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>SISTEMA DE CLIENTES</title>
    <!-- Inclua links para os arquivos CSS do Bootstrap ou de outros estilos -->
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" 
    rel="stylesheet" integrity="sha384-QWTKZyjpPEjISv5WaRU9OFeRpok6YctnYmDr5pNlyT2bRjXh0JMhjY6hW+ALEwIH" 
    crossorigin="anonymous">   
</head>
<body>
    <header>
        <!-- Cabeçalho com o logotipo e menu -->
        <nav class="navbar navbar-expand-lg navbar-light bg-light">
        <!-- Título centralizado -->
            <h1 class="navbar-brand title">ROBERT BOSCH</h1>
            <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarNav">
                <ul class="navbar-nav">
                    <li class="nav-item">
                        <a class="nav-link" href="#">Início</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#">Clientes</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#">Funcionarios</a>
                    </li>
                    <!-- Adicione mais itens de menu conforme necessário -->
                </ul>
            </div>
        </nav>
    </header>
    <div class="container mt-4">
        <!-- Conteúdo da página -->
        {% block content %}{% endblock %}
    </div>

    <footer class="mt-4">
        <!-- Rodapé do site -->
        <div class="text-center">
            © 2024 PROJETO CRUD COM DJANGO - DTA BOSCH. Todos os direitos reservados.
        </div>
    </footer>
    <!-- Inclua links para os arquivos JavaScript do Bootstrap ou de outros scripts -->
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script>
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"></script>

</body>
</html>

```
Dentro da pasta `templates/clientes` coloque os códigos abaixo conforme cada arquivo.
# Código do arquivo cria_cliente.html:

``` shell
{% extends "base.html" %}
{% block content %}
<div class="container">
    <h1>Criar Novo Cliente</h1>
    <form method="post">
        {% csrf_token %}
        {{ form.as_p }}
        <button type="submit" class="btn btn-primary">Salvar</button>
        <a href="{% url 'lista_clientes' %}" class="btn btn-secondary">Cancelar</a>
    </form>
</div>
{% endblock %}
```

# Código do arquivo deleta_cliente.html:

``` shell
{% extends "base.html" %}
{% block content %}
<div class="container">
    <h1>Confirmação de Exclusão</h1>
    <p>Tem certeza de que deseja excluir o cliente "{{ cliente.nome }}"?</p>
    <form method="post">
        {% csrf_token %}
        <button type="submit" class="btn btn-danger">Sim, Excluir</button>
        <a href="{% url 'lista_clientes' %}" class="btn btn-secondary">Cancelar</a>
    </form>
</div>
{% endblock %}
```

# Código do arquivo edita_cliente.html:

``` shell
{% extends "base.html" %}
{% block content %}
<div class="container">
    <h1>Editar Cliente</h1>
    <form method="post">
        {% csrf_token %}
        {{ form.as_p }}
        <button type="submit" class="btn btn-primary">Salvar</button>
        <a href="{% url 'lista_clientes' %}" class="btn btn-secondary">Cancelar</a>
    </form>
</div>
{% endblock %}
```
# Código do arquivo lista_clientes.html:

``` shell
{% extends "base.html" %}
{% block content %}
<div class="container">
    <h1>Lista de Clientes</h1>
    <table class="table table-striped">
        <thead>
            <tr>
                <th>ID</th>
                <th>Nome</th>
                <th>Endereço</th>
                <th>CPF</th>
                <th>Data de Nascimento</th>
                <th>Ações</th>
            </tr>
        </thead>
        <tbody>
            {% for cliente in clientes %}
            <tr>
                <td>{{ cliente.id }}</td>
                <td>{{ cliente.nome }}</td>
                <td>{{ cliente.endereco }}</td>
                <td>{{ cliente.cpf }}</td>
                <td>{{ cliente.data_nascimento }}</td>
                <td>
                    <a href="{% url 'edita_cliente' cliente.id %}" class="btn btn-primary">Editar</a>
                    <a href="{% url 'deleta_cliente' cliente.id %}" class="btn btn-danger">Excluir</a>
                </td>
            </tr>
            {% endfor %}
        </tbody>
    </table>
    <a href="{% url 'cria_cliente' %}" class="btn btn-success">Novo Cliente</a>
</div>
{% endblock %}
```

# Passo 9: Conectar URLs do Aplicativo Principal:

Em `empresa/urls.py`, conecte as URLs do aplicativo `"clientes"`:

Lembrando que `EMPRESA` é o nome do projeto que criamos lá no início. 

``` shell
from django.contrib import admin
from django.urls import path, include
from django.urls import path
from django.shortcuts import redirect


urlpatterns = [
    path('admin/', admin.site.urls),
    path('clientes/', include('clientes.urls')),
    path('', lambda request: redirect('lista_clientes'), name='home'),
]
```

# Executar o Servidor Django:

Chegou o momento de testar a nossa aplicação.

Inicie o servidor Django com o seguinte comando:
``` shell
python manage.py runserver
```
Agora você deve ser capaz de acessar seu aplicativo **CRUD de Cliente** no navegador em
http://localhost:8000/clientes/.

Você também pode acessar outras URLs definidas, como criar, editar e excluir clientes.