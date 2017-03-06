# Introdução ao git, GitHub e Jupyter Notebooks

## Ambiente de desenvolvimento com Vagrant

O Vagrant permite configurar uma máquina virtual com todas as aplicações e bibliotecas que serão utilizadas no clube.
[Clique aqui para ver o tutorial de instalação no Windows, Mac e Linux](instalacao_vagrant/).

## git

O git é uma ferramenta para armazenagem de código com o propósito de facilitar a colaboração e realizar o controle de versão de código.

Controle de versão é um sistema que registra alterações em um arquivo ou conjunto de arquivos ao longo do tempo para que você possa lembrar versões específicas mais tarde. Para os exemplos neste livro que você irá usar o código-fonte de software como os arquivos que estão sendo versão controlada, embora na realidade você pode fazer isso com quase qualquer tipo de arquivo em um computador.

Para criar uma cópia do repositório do git no seu computador local, use o comando `git clone`. É possível trabalhar neste repositório fazendo atualizações `commits`. A atualização entre o repositório local e o repositório do git se dará com os comandos `git push` e `git pull`. Todos os demais comandos do git são para gerenciar o repositório local.

Após implementar e testar as alterações no seus arquivos locais, é necessário atualizar o seu repositótio local, através da seguinte sequência sugerida:

* `git status` mostra as diferenças entre seus arquivos e o repositório local
* `git add <file>` informa o arquivo que deseja atualizar no repositório local
* `git commit -m "comentário"` adiciona os arquivos registrados pelo add no repositório local
* `git checkout <file>` descarta os arquivos modificados, atualiza com os arquivos do repositório local

Após o `git commit` o seu repositório local está em uma situação consistente. Neste momento podemos fazer um `git pull` para que o repositório local seja atualizado ao repositório do git. Entretanto, é aconselhável que antes do `git push`, faça um `git pull` para que o seu repositório local seja atualizado com as modificações que porventura tenham sido feitas no git.
Lembrando que apenas os comando `git pull` e `git push` interagem com o repositório remoto do git. Todos os outros comandos operam no repositório local.

Aprenda a usar o git na prática com a ferramenta [try.github.io](http://try.github.io/).

Para entender melhor como funciona o sistema de versionamento, leia a [documentação do git](https://git-scm.com/book/pt-br/v2).

## GitHub

GitHub é um Serviço de Compartilhamento de projetos que usam o controle de versionamento `git`. Para entender como o GitHub funcione leia o [guia do serviço](https://guides.github.com/activities/hello-world/). Procure entender como funcionam os *Pull Requests*, algo que vamos usar muito nos próximos encontros.

Lembre-se de criar uma conta no [GitHub](https://github.com/) e de solicite a adição no grupo Makers do Fab Lab Joinville abrindo uma [*Issue*](https://github.com/fablabjoinville/computacao-aplicada/issues) neste repositrio.

Para clonar repositórios do GitHub na sua máquina local, recomendamos que você configure o uso de ssh. Veja como na [documentação do GitHub](https://help.github.com/articles/connecting-to-github-with-ssh/). Adicione a chave gerada em [https://github.com/settings/keys](https://github.com/settings/keys).

Configure seu usuário local:

* `git config --global user.name "user_name"`
* `git config --global user.email "email_id"`

## Jupyter Notebooks

[Jupyter](http://jupyter.org/) é uma ferramenta que nos ajuda a testar nossos algoritmos e documentar o que for necessários. em um mesmo documento conseguimos adicionar código, texto, imagens e equações matemáticas.

Teste o [Jupyter Notebboks online aqui](https://try.jupyter.org/).

Para instalar na sua máquina local, recomendamos usar a distribuição [Python Anaconda](https://www.continuum.io/downloads).

Para outras formas de instalar o Jupyter Notebooks acesse a [documentação do projeto](http://jupyter.readthedocs.io/en/latest/install.html).

Com o ambiente instalado, execute no seu terminal:

```
jupyter notebook
```

Você também pode usar um [container Docker](https://hub.docker.com/r/alfakini/python-notebooks/).

## Referências

* [Documentação git](https://git-scm.com/book/pt-br/v2)
