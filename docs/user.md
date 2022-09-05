# Para o usuário

## Se você é aluno

### Como entrar no servidor de desafios
Os seus professores devem ter disponibilizado um link para vocês, no BlackBoard ou no email. Abra ele.
Seu usuário é o mesmo do Insper, e a senha é o mesmo nome de usuário (fique tranquilo, você poderá mudar depois).

### Enviando solução correta
Caso você acerte o código do exercício, o servidor irá te informar que está tudo correto. Parabéns!

### Enviando solução errada
Caso você erre, o servidor analisará quais testes passaram e quais não. Com isso, haverá um feedback para cada erro cometido. Use esses feedbacks para chegar até o código certo, não desista!

## Se você é professor

### Adicionando usuários
Para adicionar um usuário novo, adicione no arquivo *users.csv* um usuário novo (se o arquivo não existe ainda, pode criá-lo). Para adicionar um aluno com o usuario "pedrosilva", por exemplo, será preciso escrever o seguinte:

pedrosilva, student

Logo em seguida, execute o arquivo *adduser.py* escrevendo no terminal:
```
python3 adduser.py
```

Pronto! O usuário já conseguirá acessar o servidor!