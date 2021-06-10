# Sobre Git

Git é um sistema de controle de versão distribuído. Com essa ferramenta, é possível rastrear mudanças em arquivos e recuperar versões anteriores.

O Git trabalha com repositórios - diretórios com arquivos e uma pasta oculta chamada _.git_. Essa é responsável por armazenar todas as informações necessárias para o controle de versão.

Os arquivos de um repositório podem estar em três áreas:

- Na área _working_, os arquivos são uma cópia de uma versão do repositório e podem ser editados;
- Na área _staging_, os arquivos estão preparados para ter suas mudanças confirmadas no histórico de versão do repositório;
- Na área _repository_, os arquivos estão confirmados em uma versão do repositório.

A manipulação de repositórios é feita através de uma interface de linha de comando chamada _Bash_. No _Windows_, caso o Git tenha sido adicionado a variável de ambiente _PATH_, ele pode ser utilizado no _Powershell_.