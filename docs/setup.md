### Configuração do Backend

Entre na pasta `/backend`
```sh
cd DesafioVendaMais/backend
```

Crie um ambiente virtual:
```sh
# windows
python -m venv venv
.\.venv\Scripts\Activate


# unix
python3 -m venv venv
. venv/bin/activate
```

Instale as dependencias
```sh
pip install -r requirements.txt
```

Crie um arquivo `.env` com suas configurações. Basta seguir o exemplo fornecido no arquivo `.env.example`.

```txt
SECRET_KEY=String
```

Crie um super usuário para fazer o login
```sh
python manage.py createsuperuser
```

Rode as migrações
```sh
python manage.py makemigrations accounts
python manage.py makemigrations mybank
python manage.py migrate
```

Inicie o servidor
```
python manage.py runserver
```

### Configuração do Frontend

Entre na pasta `frontend`
```sh
cd DesafioVendaMais/frontend
```

Instale as dependencias utilizando o `npm`

```sh
npm i
```

> O projeto foi desenvolvido em torno do npm, caso queira utilizar outros gerenciadores de pacotes recomenda-se adicionar os "locks" ao gitignore

Inicie o servidor

```sh
npm run dev
```