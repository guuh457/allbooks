# AllBooks

Boas vindas a API do Allbooks!

O AllBooks é uma loja virtual que vende livros da Casa do Código. 
É um MVP que tá só começando e ainda tem muitas funcionalidades novas para serem desenvolvidas.

# JSONServer + JWT Auth

Essa é ma API Rest mockada, utilizando json-server e JWT.

## 🛠️ Instalação

```bash
$ npm install
$ npm run start-auth
```
## 🛠️ Como se registrar?

Você pode fazer isso efetuando uma requisição post para:

```
POST http://localhost:8000/public/registrar
```

Com os seguintes dados:


```
{
    "nome": "vinicios neves",
    "email": "vinicios@alura.com.br",
    "senha": "123456",
    "endereco": "Rua Vergueiro, 3185",
    "complemento": "Vila Mariana",
    "cep": "04101-300"
}
```

Repare que o e-mail é um campo único e usuários com e-mails duplicados não serão persistidos.

## 🛠️ Como fazer login?

Você pode fazer isso efetuando uma requisição post para:

```
POST http://localhost:8000/public/login
```

Com os seguintes dados:


```
{
  "email": "vinicios@alura.com.br",
  "senha":"123456"
}
```

Você vai receber um token no seguinte formato:

```
{
   "access_token": "<ACCESS_TOKEN>",
   "user": { ... dados do usuário ... }
}
```

## Autenticar próximas requests?

E então, adicionar este mesmo token ao header das próximas requisições:

```
Authorization: Bearer <ACCESS_TOKEN>
```
[33mcommit b384945c775a24c49e3c327546897b96cd540aab[m[33m ([m[1;36mHEAD[m[33m -> [m[1;32mmain[m[33m)[m
Author: guuh457 <gustavosilva.s457@gmail.com>
Date:   Wed May 22 16:00:04 2024 -0300

    Iniciando novo projeto

[33mcommit c84bf60546c9c779190acdd8172d2e572395cec8[m[33m ([m[1;31morigin/main[m[33m)[m
Author: guuh457 <167882993+guuh457@users.noreply.github.com>
Date:   Wed May 22 15:28:33 2024 -0300

    Update README.md

[33mcommit 81821d969690167f6bcc7daec38d8ad7d25b48ba[m
Author: guuh457 <gustavosilva.s457@gmail.com>
Date:   Tue May 21 10:03:28 2024 -0300

    Adiciona projeto inicial
