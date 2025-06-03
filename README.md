# Como executar o projeto em outra máquina

(Necessário ter o Python 3.1+ instalado)

### 1. Clone o repositório

git clone https://github.com/gabriesb/Cadastro-de-Usuarios.git
cd Cadastro-de-Usuarios

###2. Crie e ative um ambiente virtual (recomendado)
No Windows (PowerShell):

python -m venv .venv
.\\.venv\\Scripts\\activate

No Linux/macOS:

python3 -m venv .venv
source .venv/bin/activate

###3. Instale as dependências

pip install -r requirements.txt

###4. Configure o banco de dados PostgreSQL (Supabase)
No arquivo settings.py do Django, configure a conexão com o banco PostgreSQL do Supabase:

DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.postgresql',
        'NAME': 'postgres',           # Nome do banco no Supabase
        'USER': 'postgres',           # Usuário do banco
        'PASSWORD': 'cadastrousuario', # Senha do banco
        'HOST': 'db.zdfglipykgchpvrpzspj.supabase.co',  # Host do banco
        'PORT': '5432',
    }
}

Substitua as informações acima pelas credenciais do seu banco Supabase.

###5. Rode as migrations para criar as tabelas no banco

python manage.py migrate

###6. Execute o servidor local do Django

python manage.py runserver

###7. Acesse a aplicação
   
Abra no navegador:
http://127.0.0.1:8000/usuarios/
