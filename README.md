# negocio-da-marcia
uma lição que ela pediu

name: Conferir a senhas e logins

on: 
  push:   # quando chegar um novo login armazenar ele para que salvo no sistema
    branches:
      - main

jobs:
  padaria:
    runs-on: windows-latest  # login em um site

    steps:
      - name: Conferir senha
        run: echo "senha verificada!"

      - name: caso a senha esteja certa
        run: echo "acesso concedido!"

      - name: caso esteja errado 
        run: echo "acesso negado!"
