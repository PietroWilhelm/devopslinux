# Comandos Linux

## Diretório | Função principal  | Exemplo
/bin | Executáveis essenciais disponíveis a todos os usuários| ls, cp

/sbin | Executáveis de administração de sistema (root) | ifconfig, iptables

/etc | Arquivos de configuração global | /etc/ssh/sshd_config

/home | Diretórios pessoais dos usuários | /home/joao

/var | Dados variáveis (logs, spool) | /var/log/syslog

/usr | Programas de usuário, manuais e bibliotecas compartilhadas | /usr/bin/grep

/tmp | Arquivos temporários limpos em reinicialização |  /tmp/socke

## History -> comando para ver o historico de comandos usados

# | Navegação e Manipulação de Arquivos

## Deslocamento pelo Sistema 

### Comando | Descrição | Exemplo
pwd | Mostra diretório atual | pwd

cd  | Troca de diretório | cd /etc

ls [-l -a -h] | Lista conteúdo (longa, ocultos, tamanhos legíveis) | ls -lah

## Criação, Cópia e Remoção

### Comando | Ação | Dica
mkdir | Cria diretório | mkdir projetos

touch | Cria arquivo vazio | touch notas.txt

cp [-r] | Copia arquivos ou pastas |  cp foto.jpg ~/backup/

mv | Move ou renomeia |  mv notas.txt notas_old.txt

rm [-r -f] | Remove (recursivo, forçado) | rm -rf tmp/

## Visualização de Conteúdo
Comando | Descrição | Exemplo

Cat | Exibe arquivo inteiro | cat read.me

less | Rolagem interativa, ideal para logs grandes | less install.log

head/tail-n | Primeiras ou últimas linhas | tail -10 install.log

## | Comandos Adicionais para Administração de Sistema
### Comando | Descrição | Exemplo
find | Localizar arquivos específicos no SO find | . -name "*.txt"

grep | Buscar textos dentro dos arquivo | grep "ERROR" logs/*.log

df  | Monitorar o espaço disponível no sistema | df -Th

ps | Lista processos no sistema | ps -aux

top | Monitora o sistema em Tempo Real | top -u admln
