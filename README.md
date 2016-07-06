# user-samba
Bash Script Simples para gerenciamento fácil de usuários ao SAMBA

Dependência: samba

Para usar basta adicionar o comando na pasta "/usr/bin" e deixá-lo com permissão de execução

Como funciona (Conteúdo do HELP):

Este comando é usado para "criar/adicionar" um usuário ao compartilhamento SAMBA e/ou Sistema.
Pode-se usar qualquer outro nome e senha para uso no SAMBA, para maior segurança, (recomendável)
Ou pode "adicionar/remover" um usuário já existente.
O usuário criado se torna um usuário "de sistema", ou seja, "sem login" - Não aparecerá na tela de login.

Parâmetros:

        --help|-h       Menú de ajuda.
        --list|-l       Lista usuários associados ao SAMBA.
        --remove|-rm    Remove um usuário específico do SAMBA e/ou Sistema.
        --ssh           Criar o usuário com suporte para uso com o ssh.
                        Se omitido, será criado um usuário sem suporte ao ssh
Exemplos:

 Criar um usuário associado ao SAMBA "SEM" suporte ao SSH (Recomendável):

        user-smb USUÁRIO

 Criar um usuário associado ao SAMBA "COM" suporte ao SSH:

        user-smb USUÁRIO --ssh

 Listar usuários associados ao compartilhamento SAMBA:

	user-smb --list

 Remover um usuário específico do SAMBA e/ou Sistema:

	user-smb USUARIO --remove

