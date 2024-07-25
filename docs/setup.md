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
DEBUG=Bool
SECRET_KEY=String
EMAIL_HOST_USER=String
EMAIL_HOST_PASSWORD=String
```

> O arquivo de exemplo contém mais detalhes

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