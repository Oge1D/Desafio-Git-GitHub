# Desafio Dio

### Desafio utilizando os comandos do GIT Bash e push GitHub ou pull Github para máquina local.

###### Abaixo irei descrever os comandos que aprendi durante o curso da DIO.

- **_CD:_** CD + "Nome da Pasta" _vai até a pasta_ ou CD + " .. " _volta uma pasta anterior._
- **_DIR:_** Mostra as pastas dentro do diretório;
- **_Tecla_TAB:_** Complementa o nome da pasta ou do arquivo;
- **_MKDIR:_** Cria uma nova pasta dentro do diretório;
- **_LS:_** Lista o conteúdo dentro da pasta;
- **_LS -a:_** Mostra os itens ocultos na pasta
- **_Git Status:_** Diz os Status de cada arquivo inserido, modificado ou que será empurrado;
- **_MV:_** Move um arquivo;
- **_Git ADD:_** é divido em **Git add**, **Git Add ***, **Git Add .**, **Git Add -A**. *(Todos eles adicionam o arquivo para STAGED)*;
- **_Git Commit -m "Mensagem":_** Pega os arquivos em *STAGED* e deixa pronto para commita-los.
- ***Git config --global user.email "seu e-mail":*** Você ira inserir este e-mail com o mesmo que criou sua conta no GitHub para não haver desencontros de informações.
- ***Git config --global --unset user.email "seu e-mail":*** Remove o e-mail cadastrado no seu ambiente de desenvolvimento;
- ***Git config --global user.name seu nome":*** Você ira inserir com o mesmo que criou sua conta no GitHub para não haver desencontros de informações.
- ***Git config --global --unset user.name "seu nome":*** Remove o nome cadastrado no seu ambiente de desenvolvimento;
- **Git pull origin main ou master:** Quando se da o comando *Git pull origin "Endereço de onde se quer puxar o repositório* sai do Servidor Remoto (GitHub) para o seu ambiente de desenvolvimento;

- **Git Push origin main ou master:**  Quando se da esse comando sai do *Git commit -m "mensagem"* ambiente de desenvolvimento para o servidor remoto *(GitHub)*;
- **Git Clone "Endereço":** Cópia o endereço dos repositórios *(seu ou de terceiros)* para a sua máquina;
- **Git Remote -v:** Mostra o endereço onde esse repositorio está localizado



#### Há 2 tipos de ambientes, são eles:



1. **Ambiente de Desenvolvimento -** Nossa máquina;
2. **Servidor (GitHub) -** Repositório Remoto;



### O que é SHA1?

É um conjunto de funções HASH criptográficas projetas pela _(NSA - Agência de Segurança Nacional dos E.U.A)_

E gera um conjunto de caracteres de 40 dígitos.



### Configurações antes de criar uma commit:

###### Configuração de E-mail:

Git config --global user.email "seu e-mail":

**Você ira inserir este e-mail com o mesmo que criou sua conta no GitHub para não haver desencontros de informações.**

Git config --global --unset user.email "seu e-mail":

***Remove o e-mail cadastrado no seu ambiente de desenvolvimento;***



###### Configuração de nome:

Git config --global user.name "seu nome"

**Você ira inserir com o mesmo que criou sua conta no GitHub para não haver desencontros de informações.**

Git config --global --unset user.name "seu nome":

***Remove o nome cadastrado no seu ambiente de desenvolvimento;***



### Criando uma Commit:

Os comandos utilizados são:

- **Git Init:** Inicia o Git;
- **Git Add:** Adiciona os arquivos para área Stage (Fica aguardando um comando para ir ao servidor remoto);
- **Git Commit:** Sai do _Stage_ em direção *commit*, e ao usar o Git commit -m "mensagem", cria uma commit;
- **Git pull origin main ou master:** Quando se da o comando *Git pull origin "Endereço de onde se quer puxar o repositório* sai do Servidor Remoto (GitHub) para o seu ambiente de desenvolvimento;
- **Git Push origin main ou master:**  Quando se da esse comando sai do *Git commit -m "mensagem"* ambiente de desenvolvimento para o servidor remoto *(GitHub)*;



#### Git Init

A duas principais divisões:

- **Tracked -** Arquivos rastreáveis pelo Git;
- **Untracked -** Arquivos não rastreáveis pelo Git;

E no Tracked há 3 subdiviões:

- **Unmodified:** Arquivo não modificado;
- **Modified:** Arquivo que era _unmodified_ e foi modificado;
- **Staged:** Arquivos prontos para serem utilizados para *modified* ou voltar para *unmodified*;



### Objetos do Git.

São divido em 3 categorias que se complementam:

**_Blobs -_** Podem ser objetos de imagem, áudio, apesar que as vezes é código binário executável ser armazenado como um blob.

**_Tree -_** Em vez de ter somente os valores, como o blob, ele também armazena os Blob. Também tem o nome do Arquivo e a composição do Blob. Alterando algo no arquivo, muda a encriptação da TREE.

**_Commit -_** A commit junta todos os arquivos e ele aponta para a **Tree e a Tree** para **Blob** e tem os dados da **Tree**, Parente _(outra Commit)_, autor e a mensagem _(readme.md)_



### CHAVES SSH:

Usando o comando:

**_ SSH-keygen -t ed 25519 -C "seu e-mail"_**

Gera um código de acesso entre o seu servidor local (Git - Computador) e o servidor remoto (GitHub) no qual você não precisa de vinculações cotidianas, e ele informará em qual local está salvo sua chave pública e privada

**OBS:** Faça somente isso em sua máquina de confiança! E a chave a ser inserida no GitHub será a chave pública.



