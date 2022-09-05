# Para o desenvolvedor

## Preparando o ambiente de desenvolvimento

Primeiramente, será preciso instalar o Framework [Flask](https://flask.palletsprojects.com/en/2.2.x/). Os seguintes comandos precisarão ser rodados na linha de comando (caso você tenha o pip instalado).

```
pip install Flask
pip install flask_httpauth
```

Com isso, você terá todas bibliotecas do Flask instaladas e prontas para rodarem. A seguir, é preciso executar o comando ```flask --app softdes run```, é gerado um servidor no link **http://127.0.0.1:5000/**. Com isso, será possível fazer todas as modificações com o servidor rodado, e caso queira fazer uma mudança depois, é possível fazer o deploy. 

Além disso, para (quase) finalizar as instações necessárias, esse projeto utiliza o Sqlite3 também. Para instalalá-lo, basta apenas rodar no terminal
```
sudo apt install sqlite3
```

## Como rodar o software
Os comandos acima tornam possível rodar o projeto em questão, mas ele possui algumas necessidades extras para tornar possível acessar o servidor de desafios. Para começar, é preciso criar um arquivo em *csv*, e dentro dele informar dados dos usuários. Eles serão escritos da seguinte maneira:

usuario,tipo

Depois disso, é preciso rodar o arquivo *quiz.db*. A maneira mais eficaz de fazer isso é baixar mais uma instalação:
```
sudo apt install sqlitebrowser
```

Abra o [DB Browser for SQLite](https://sqlitebrowser.org/) e abra o arquivo *quiz.db*. Na aba "*Browse Data*", é possível ver os usuários adicionados e seus tipos, como mostra [essa foto](./img/dbbrowser.png).

Para logar, é preciso ter o usuário adicionado. A senha é o próprio nome do usuário, e é possível mudar ela dentro da página, conforme pode ser visto [aqui](./img/servidor.png).

## Estrutura do código em alto nível
Esse código utiliza uma base de dados SQL (para os usuários) e o framework Flask para a criação do servidor que será utilizado.