## 1. Instale Python e Django

Antes de mergulhar no código, certifique-se de que você possui as seguintes ferramentas:

* Verifique a instalação do Python usando o seguinte comando no seu terminal:

```
python3 --version # ou python --version
```

* Se ele estiver instalado, você verá o número da versão. Caso contrário, faça o download em [https://www.python.org/downloads/](https://www.python.org/downloads/).

* Crie um diretório para o seu projeto. Neste artigo, usaremos o nome **chatbot-django-gemini**. Acesse-o e crie um ambiente virtual para isolar as dependências do projeto:

```
mkdir chatbot-django-gemini
cd chatbot-django-gemini
python3 -m venv venv
```

* Ative o ambiente virtual:

```
source venv/bin/activate
```

* Instale o Django usando pip:

```
pip install django
```

* Crie um arquivo `requirements.txt` para listar as dependências do seu projeto, incluindo o Django. O conteúdo do arquivo `requirements.txt` deve ser algo assim:

```
django>=4.0
```

* Depois, instale as dependências do arquivo `requirements.txt`:

```
pip install -r requirements.txt
```

Para aplicar as mudanças do modelo ao seu banco de dados, execute os seguintes comandos no terminal:

```
python3 manage.py makemigrations
python3 manage.py migrate
```


## 10. Execute o Servidor e Teste Seu Chatbot

* No seu terminal, navegue até o diretório do projeto e inicie o servidor de desenvolvimento do Django usando:

```
python3 manage.py runserver
```

* Isso normalmente iniciará o servidor na porta 8000 por padrão.

* Abra seu navegador e acesse a URL do chatbot definida na configuração de URLs do seu projeto (http://127.0.0.1:8000/chatbot). Isso deve exibir a interface do chatbot.

