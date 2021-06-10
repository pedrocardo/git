# Comando _config_

O comando _config_ pode modificar ou acessar variáveis locais e globais.

Variáveis globais ficam no arquivo _.gitconfig_. No _Windows_, esse arquivo fica dentro do diretório do usuário.

Comando _config_ com _--global_ _user.name_ modifica a variável global que armazena o nome do usuário.

```
git config --global user.name [nome do usuário]
```

Comando _config_ com _--global_ _user.email_ modifica a variável global que armazena o e-mail do usuário.

```
git config --global user.email [e-mail do usuário]
```

Comando _config_ com _--list_ exibe uma lista de variáveis configuradas.

```
git config --list
```
