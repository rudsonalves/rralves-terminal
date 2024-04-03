# Plugin WordPress - RRAlves Terminal

O plugin “RRAlves Terminal” é uma ferramenta simples para o WordPress que simula uma emulação de terminal ao redor do seu texto, proporcionando a aparência de um terminal do iOS ou Linux. Essa funcionalidade é particularmente interessante para bloggers, desenvolvedores e educadores que desejam apresentar comandos, códigos ou instruções de maneira estilizada e interativa em seus posts.

Seu código é bem simples e está disponível para dowload no meu GitHub: rralves-terminal. Sinta-se a vontade para baixar, usar e alterar a seu gosto.
Funcionamento do Plugin

O coração deste plugin é o shortcode,

que permite aos usuários encapsular texto ou comandos específicos que devem ser exibidos dentro de um ambiente que imita um terminal. O plugin oferece atributos personalizáveis, como user, computer, e cwd (diretório de trabalho atual), para que os autores possam customizar a prompt de comando exibida antes dos comandos no terminal. Por exemplo, usar

personaliza a prompt para refletir esses valores específicos.

Bash


root@suzail:~$ ls -la

Observe que o usuário “root” será impresso em vermelho, enquanto que outros, são impressos em verde.

Bash


alves@arabel:~$ tree .
.
├── index.php
├── license.txt
├── readme.html
├── wp-activate.php
├── wp-admin
│   ├── about.php
│   ├── admin-ajax.php
│   ├── admin-footer.php
│   ├── admin-functions.php
│   ├── admin-header.php

Características Principais

    Personalização de Prompt: Os usuários podem definir o usuário, o nome do computador e o diretório de trabalho atual para personalizar a prompt de comando do terminal.
    Estilos de Terminal: Suporte para diferentes estilos de terminal, como iOS e Linux, permitindo aos usuários escolher a aparência que melhor se adapta ao conteúdo ou preferência pessoal.
    Shortcode Versátil: Através do uso do shortcode terminal, os autores podem facilmente adicionar saídas de terminal estilizadas dentro de seus posts, melhorando a forma como o conteúdo técnico é apresentado.
    Estilização CSS: O plugin se encarrega de enfileirar e aplicar os estilos CSS necessários para assegurar que a emulação do terminal tenha uma aparência autêntica e esteja visualmente integrada ao resto do conteúdo do site.

Implementação Técnica

    Geração de Prompt Dinâmica: A classe Terminal contém métodos para gerar dinamicamente a prompt do terminal baseada nos atributos fornecidos pelo usuário, utilizando classes CSS para diferenciar visualmente usuários comuns de root.
    Criação de Saída Formatada: O plugin constrói a saída do terminal formatando o conteúdo encapsulado pelo shortcode. Isso inclui a adição de um cabeçalho de terminal, bem como a formatação do conteúdo como se estivesse sendo exibido em um terminal real.
    Estilos Customizáveis: A função register_styles gerencia o carregamento dos arquivos CSS necessários para estilizar o terminal, garantindo que a aparência do terminal seja consistente e profissional.
    Processamento de Conteúdo: O plugin divide o conteúdo do shortcode em linhas individuais, permitindo uma representação precisa de múltiplos comandos ou saídas dentro do terminal simulado.

Benefícios para o Usuário

O plugin “RRAlves Terminal” enriquece os posts com uma representação estética e funcional de terminais, elevando a qualidade do conteúdo técnico e educativo. Ele fornece uma maneira interativa de engajar os leitores, permitindo que conceitos técnicos sejam apresentados de forma clara e visualmente atraente.
