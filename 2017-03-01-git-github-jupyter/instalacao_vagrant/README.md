# Instalação do ambiente de desenvolvimento

Este tutorial instala o ambiente de desenvolvimento do clube de computação aplicada do FABLAB Joinville.

## VirtualBox

Instale o VirtualBox para o seu sistema operacional

- [Windows] (http://download.virtualbox.org/virtualbox/5.1.14/VirtualBox-5.1.14-112924-Win.exe)
- [Mac] (http://download.virtualbox.org/virtualbox/5.1.14/VirtualBox-5.1.14-112924-OSX.dmg)
- [Linux] (https://www.virtualbox.org/wiki/Linux_Downloads)

A instalação é bem simples no modo next, next, finish.

## Vagrant

Instale o Vagrant para o seu sistema operacional

- [Windows](https://releases.hashicorp.com/vagrant/1.9.2/vagrant_1.9.2.msi?_ga=1.247276676.1620532176.1488463812)
- [Mac](https://releases.hashicorp.com/vagrant/1.9.2/vagrant_1.9.2.dmg?_ga=1.247276676.1620532176.1488463812)
- [Linux - Debian 64bits](https://releases.hashicorp.com/vagrant/1.9.2/vagrant_1.9.2_x86_64.deb?_ga=1.247276676.1620532176.1488463812)

## Configuração

Em algum diretório de sua escolha na sua máquina faça os seguintes procedimentos

1. Crie um diretório com o nome clube-computacao
2. [Faça download do arquivo Vagrantfile aqui](Vagrantfile) e salve-o dentro deste diretório com o nome Vagrantfile
3. Abra um prompt de comando:
    
    Windows: Aperte Win+R, digite cmd e aperte enter
    Mac: Command+Espaço, digite terminal e aperte enter
    Linux: Se está usando linux provavelmente você sabe :)

4. No prompt de comando navegue até a pasta que você criou com o nome clube-computacao como no exemplo abaixo:
    
    Windows: cd c:\Users\guilherme\clube-computacao
    Mac: cd /Users/guilherme/clube-computacao
    Linux: cd ~/clube-computacao
    
5. No diretório onde se encontra o arquivo Vagrantfile digite o comando:

    vagrant up

Este comando fará o download de todos os arquivos necessários para executar o ambiente. Dependendo da sua conexão esse procedimento pode demorar vários minutos na primeira execução.

Caso precise encerrar o ambiente execute o comando:

    vagrant halt

Se precisar apagar o ambiente digite o comando:

    vagrant destroy

6) Se o comando vagrant up executar com sucesso você verá uma linha com o seguinte conteúdo:

    ==> default: [I 17:29:15.231 NotebookApp] The Jupyter Notebook is running at: http://[all ip addresses on your system]:8888/

Quando esta linha aparece basta abrir uma janela do browser e entrar no endereço

    http://localhost:8888

7) Todos os arquivos criados na interface web estarão disponíveis no diretório clube-computacao.
