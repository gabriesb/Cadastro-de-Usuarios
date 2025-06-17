#Cadastro de Usuários

##Este é um projeto simples em Django para cadastro de usuários com nome e idade. O sistema permite registrar e listar usuários utilizando um banco de dados SQLite.

Tecnologias Utilizadas

Python 3.10+

Django 4.x

HTML5 e Bootstrap 5

SQLite (padrão do Django)

##Como instalar e executar

##Clone este repositório:
git clone https://github.com/gabriesb/Cadastro-de-Usuarios.git
cd Cadastro-de-Usuarios

##Crie e ative um ambiente virtual:
python -m venv venv
No Windows: venv\Scripts\activate
No Linux/Mac: source venv/bin/activate

##Instale as dependências:
pip install -r project_cad_user/requirements.txt

##Execute as migrações do banco de dados:
python manage.py migrate

##Inicie o servidor:
python manage.py runserver

##Acesse em: http://127.0.0.1:8000

##Estrutura do Projeto (simplificada)

project_cad_user/

manage.py

requirements.txt

app_cad_user/

models.py

views.py

templates/

usuarios/

base.html

home.html

usuarios.html

##Funcionalidades

Cadastro de usuário com nome e idade

Listagem de usuários cadastrados

Validação simples no backend

##Testes Automatizados

O projeto usa GitHub Actions com flake8 e pytest para garantir qualidade de código.

##Contribuição

Sugestões e melhorias são bem-vindas! Sinta-se livre para abrir issues ou enviar pull requests.
