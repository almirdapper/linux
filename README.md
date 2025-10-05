# 🐧 Comandos Linux Mais Usados

Este guia resume os principais comandos do Linux divididos por categoria, com explicações e exemplos práticos.

---

## 📂 Manipulação de Arquivos e Diretórios

| Comando | Descrição | Exemplo |
|----------|------------|----------|
| `ls` | Lista arquivos e diretórios | `ls -la` |
| `cd` | Muda o diretório atual | `cd /home/usuario` |
| `pwd` | Mostra o diretório atual | `pwd` |
| `mkdir` | Cria um novo diretório | `mkdir projetos` |
| `rmdir` | Remove diretório vazio | `rmdir tmp` |
| `rm` | Remove arquivos ou diretórios | `rm -rf /tmp/teste` |
| `cp` | Copia arquivos ou diretórios | `cp arquivo.txt /backup/` |
| `mv` | Move ou renomeia arquivos | `mv dados.txt /home/backup/` |
| `touch` | Cria um arquivo vazio | `touch novo.txt` |
| `cat` | Exibe conteúdo de um arquivo | `cat arquivo.txt` |
| `head` | Mostra primeiras linhas | `head -n 10 log.txt` |
| `tail` | Mostra últimas linhas | `tail -f log.txt` |
| `find` | Busca arquivos no sistema | `find /home -name "*.log"` |
| `locate` | Localiza arquivos via índice | `locate config.yaml` |

---

## ⚙️ Permissões e Propriedades

| Comando | Descrição | Exemplo |
|----------|------------|----------|
| `chmod` | Altera permissões de arquivo | `chmod 755 script.sh` |
| `chown` | Altera dono e grupo | `chown user:grupo arquivo.txt` |
| `chgrp` | Altera grupo do arquivo | `chgrp admin arquivo.txt` |

---

## 📦 Gerenciamento de Pacotes

| Sistema | Instalar | Remover | Atualizar |
|----------|-----------|----------|------------|
| **Debian/Ubuntu (APT)** | `sudo apt install nginx` | `sudo apt remove nginx` | `sudo apt update && sudo apt upgrade` |
| **RedHat/CentOS (YUM/DNF)** | `sudo yum install nginx` | `sudo yum remove nginx` | `sudo yum update` |
| **Arch (PACMAN)** | `sudo pacman -S nginx` | `sudo pacman -R nginx` | `sudo pacman -Syu` |

---

## 👤 Usuários e Grupos

| Comando | Descrição | Exemplo |
|----------|------------|----------|
| `useradd` | Cria um novo usuário | `sudo useradd almir` |
| `passwd` | Define senha do usuário | `sudo passwd almir` |
| `usermod` | Modifica usuário | `sudo usermod -aG sudo almir` |
| `deluser` | Remove usuário | `sudo deluser almir` |
| `groups` | Mostra grupos do usuário | `groups almir` |

---

## 🌐 Rede

| Comando | Descrição | Exemplo |
|----------|------------|----------|
| `ping` | Testa conexão com host | `ping google.com` |
| `ifconfig` / `ip` | Mostra interfaces de rede | `ip addr show` |
| `netstat` | Mostra conexões e portas | `netstat -tuln` |
| `ss` | Substituto moderno do netstat | `ss -tuln` |
| `curl` | Faz requisições HTTP | `curl -I https://openai.com` |
| `wget` | Baixa arquivos da web | `wget https://site.com/arquivo.zip` |
| `scp` | Copia arquivos via SSH | `scp arquivo.txt user@server:/home/` |
| `ssh` | Conecta em servidor remoto | `ssh user@192.168.0.1` |

---

## 🧠 Processos e Sistema

| Comando | Descrição | Exemplo |
|----------|------------|----------|
| `ps` | Lista processos ativos | `ps aux` |
| `top` | Monitora processos em tempo real | `top` |
| `htop` | Interface avançada para processos | `htop` |
| `kill` | Encerra processo | `kill -9 PID` |
| `df` | Mostra uso de disco | `df -h` |
| `du` | Mostra tamanho de diretórios | `du -sh /home/*` |
| `free` | Exibe uso de memória | `free -h` |
| `uptime` | Mostra tempo ligado | `uptime` |
| `uname` | Exibe informações do sistema | `uname -a` |
| `dmesg` | Mostra logs do kernel | `dmesg | tail` |

---

## 🔍 Busca e Texto

| Comando | Descrição | Exemplo |
|----------|------------|----------|
| `grep` | Busca texto em arquivos | `grep "error" log.txt` |
| `awk` | Processa texto por padrão | `awk '{print $1}' arquivo.txt` |
| `sed` | Edita texto de forma automática | `sed 's/teste/ok/g' arquivo.txt` |
| `sort` | Ordena linhas | `sort lista.txt` |
| `uniq` | Remove duplicadas | `uniq lista.txt` |
| `wc` | Conta linhas, palavras, bytes | `wc -l arquivo.txt` |

---

## ⏱️ Atalhos e Histórico

| Comando | Descrição |
|----------|------------|
| `history` | Mostra histórico de comandos |
| `!!` | Repete o último comando |
| `!n` | Executa comando número *n* no histórico |
| `Ctrl + C` | Interrompe execução |
| `Ctrl + D` | Sai do terminal |
| `Ctrl + R` | Pesquisa comando anterior |

---

## 📦 Compactação e Arquivos

| Comando | Descrição | Exemplo |
|----------|------------|----------|
| `tar` | Compacta/descompacta arquivos | `tar -czvf backup.tar.gz /home/almir` |
| `gzip` | Compacta arquivo | `gzip arquivo.log` |
| `gunzip` | Descompacta arquivo | `gunzip arquivo.log.gz` |
| `zip` | Cria arquivo zip | `zip -r projeto.zip pasta/` |
| `unzip` | Extrai arquivo zip | `unzip projeto.zip` |

---

## 🧩 Dicas Úteis

- `man comando` → Mostra manual do comando  
- `sudo !!` → Repete o último comando com privilégios de root  
- `alias ll='ls -la'` → Cria um atalho personalizado  
- `history | grep texto` → Busca no histórico  
- `df -h` → Verifica espaço em disco  

---

📘 **Autor:** Almir R. Dapper  
🕓 **Última atualização:** 2025-10-04  