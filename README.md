# Guia de Comandos Linux 

Este repositório contém uma referência rápida dos principais diretórios e comandos do ecossistema Linux.

---

##  Estrutura de Diretórios (FHS)

| Diretório | Função Principal | Exemplo |
| :--- | :--- | :--- |
| `/bin` | Executáveis essenciais para todos os usuários | `ls`, `cp`, `cat` |
| `/sbin` | Executáveis de administração do sistema (root) | `iptables`, `fdisk` |
| `/etc` | Arquivos de configuração global do sistema | `/etc/ssh/sshd_config` |
| `/home` | Diretórios pessoais dos usuários | `/home/usuario` |
| `/var` | Dados variáveis (logs, filas de impressão) | `/var/log/syslog` |
| `/usr` | Binários, bibliotecas e documentação de usuários | `/usr/bin/grep` |
| `/tmp` | Arquivos temporários (limpos na reinicialização) | `/tmp/sess_123` |

> **LEMBRAR:** Utilizar o comando `history` quando querer visualizar o histórico de comandos executados na sessão.

---

## Navegação e Manipulação de Arquivos

### Deslocamento pelo Sistema
| Comando | Descrição | Exemplo |
| :--- | :--- | :--- |
| `pwd` | Mostra o caminho do diretório atual | `pwd` |
| `cd` | Alterna entre diretórios | `cd /etc` |
| `ls` | Lista conteúdo (`-l` detalhes, `-a` ocultos, `-h` legível) | `ls -lah` |

### Criação, Cópia e Remoção
| Comando | Ação | Exemplo |
| :--- | :--- | :--- |
| `mkdir` | Cria um novo diretório | `mkdir projetos` |
| `touch` | Cria um arquivo vazio ou atualiza a data | `touch notas.txt` |
| `cp` | Copia arquivos ou pastas (`-r` para pastas) | `cp foto.jpg ~/backup/` |
| `mv` | Move ou renomeia arquivos/diretórios | `mv notas.txt notas_old.txt` |
| `rm` | Remove arquivos ou pastas (`-rf` para recursivo e forçado) | `rm -rf tmp/` |

---

## Visualização e Busca de Conteúdo

| Comando | Descrição | Exemplo |
| :--- | :--- | :--- |
| `cat` | Exibe todo o conteúdo do arquivo na tela | `cat read.me` |
| `less` | Navegação interativa (ideal para logs grandes) | `less install.log` |
| `tail` | Exibe as últimas linhas de um arquivo | `tail -n 10 install.log` |
| `grep` | Busca por termos específicos dentro de arquivos | `grep "ERROR" logs/*.log` |
| `find` | Localiza arquivos na hierarquia do sistema | `find . -name "*.txt"` |

---

## Administração e Monitoramento

| Comando | Descrição | Exemplo |
| :--- | :--- | :--- |
| `df` | Monitora o espaço disponível em disco | `df -Th` |
| `ps` | Lista os processos ativos no sistema | `ps -aux` |
| `top` | Monitora o uso de recursos em tempo real | `top -u admin` |
| `sudo` | Executa comandos com privilégios de superusuário | `sudo apt update` |
| `chmod` | Altera as permissões de acesso de arquivos | `chmod +x script.sh` |

## Atalhos Úteis do Terminal
* `Tab`: Autocompleta comandos e nomes de arquivos.
* `Ctrl + C`: Cancela o processo em execução.
* `Ctrl + L`: Limpa o terminal (igual ao comando `clear`).
* `Ctrl + R`: Pesquisa comandos no histórico.
* `!!`: Executa o último comando novamente (útil com `sudo `).
---
