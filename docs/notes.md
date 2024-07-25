## Problemas encontrados

- requirements.txt fora da pasta backend
- erro no gitignore, não ignora a pasta venv corretamente
- readme não mostra qual a pagina inicial. index deveria redirectionar para dashboard
- não é explicado o uso das variáveis do .env para o backend
- falta tratamento de erro para email não encontrado
- falta documeexplicação sobre dotenv do front
- falta polimento no layout
- falta tratamento de erro
- ux ruim
- dados da carteira não atualizam em tempo real
- layout do filtro quebrando

## Problemas corrigidos

### `requirements.txt` movido para `/backend`

Os requisitos fazem parte das dependencias do Python, logo, faz mais sentido deixar ao lado de onde vive o diretório `/venv`

### Criado `.gitignore` para o backend

É possível, e recomendável, para monorepos, criar cada git ignore individualmente.

### Criado `setup.md`

O arquivo `README.md` contém uma descrição incompleta das configurações de ambiente, tanto para back quando frontend. É necessária uma lista mais detalhada que explica de fato como é feito todo processo de configuração.

### Adicionada descrições no `.env.exemplo`

As descrições das variáveis de ambiente ajudam a compreender o fluxo em caso seja necessário modificar o código posteriormente