<b>
CONFIGURANDO UM AMBIENTE QUE SUPORTE CLOJURE
</b>

Todos os passos desse tutorial/exemplo/material de estudo são baseados nas seguintes referências: Clojure.org: https://clojure.org/guides/getting_started

Sobre o ambiente no qual esse material está sendo produzido:
luciano@leonard-kleinrock:~$ uname -a
Linux leonard-kleinrock 5.0.0-37-generic #40~18.04.1-Ubuntu SMP Thu Nov 14 12:06:39 UTC 2019 x86_64 x86_64 x86_64 GNU/Linux

--------------------------------------------------------------------------------------------
1) Garanta que você possui estas ferramentas instaladas: bash, curl, rlwrap, and Java1.1) Antes de tudo atualize as referências do gerenciador de pacotes: sudo apt update1.2) Para instalar o bash: sudo apt install bash1.3) Para instalar o curl: sudo apt install curl1.4) Para instalar o rlwrap: sudo apt install rlwrap1.5) Para instalar o java: sudo apt install default-jre

2) Crie um diretório para organizar o material de estudo.Sugestão: mkdir -p /home/luciano/estudo/clojure

3) Baixe o script de instalação do Clojure.Execute: curl -O https://download.clojure.org/install/linux-install-1.10.1.507.sh

4) Altere a permissão de execução do arquivo que acabou de baixar.Execute: sudo chmod u=rwx linux-install-1.10.1.507.sh

5) Execute o script de instalação.sudo ./linux-install-1.10.1.507.sh

Se tudo deu certo até aqui você vai executar "clj -help" e a primeira linha retornada será a versão do Clojure:
Version: 1.10.1.507Usage: clojure [dep-opt*] [--] [init-opt*] [main-opt] [arg*] clj [dep-opt*] [--] [init-opt*] [main-opt] [arg*]

<b>
EXECUTANDO O PRIMEIRO EXEMPLO
</b>

1) Execute o comando "clj" apontando para o arquivo hello.clj.luciano@leonard-kleinrock:~/estudo/clojure$ clj projeto-hello-world/hello.clj Hello world!