# 2025-2 - Notas - Tutorial de Conceitos Básicos de Linux

Este tutorial abordará os fundamentos do Linux, incluindo sua estrutura básica, comandos essenciais e conceitos importantes para iniciantes.  

Foi construído com o auxílio do [deepseek](https://chat.deepseek.com/).

---
## Sumário
1. O que é Linux?
2. Distribuições (Distros) mais populares:
3. Estrutura de Diretórios no Linux
4. Comandos Básicos no Terminal
5. Editores de Texto no Terminal
6. Gerenciamento de Pacotes

---

## 1. O que é Linux?
Linux é um **sistema operacional de código aberto** baseado no kernel Linux, criado por **Linus Torvalds** em 1991. Ele é amplamente utilizado em servidores, desktops e dispositivos embarcados.  

---

## 2. Distribuições (Distros) mais populares:
- [Ubuntu](https://ubuntu.com/)  
- [Debian](https://www.debian.org/)  
- [Fedora](https://getfedora.org/)  
- [CentOS](https://www.centos.org/)  
- [Arch Linux](https://archlinux.org/)  
- [Linux Mint](https://linuxmint.com/)  

---

## 3. Estrutura de Diretórios no Linux
O Linux segue uma hierarquia de diretórios padrão:  

| Diretório       | Descrição |  
|----------------|-----------|  
| **/**          | Raiz do sistema |  
| **/bin**       | Binários essenciais |  
| **/etc**       | Arquivos de configuração |  
| **/home**      | Diretórios dos usuários |  
| **/var**       | Arquivos variáveis (logs, bancos de dados) |  
| **/tmp**       | Arquivos temporários |  
| **/usr**       | Programas e bibliotecas |  
| **/root**      | Home do superusuário (root) |  

---

## 4. Comandos Básicos no Terminal

### 4.1. Navegação
| Comando        | Descrição |  
|---------------|-----------|  
| `pwd`         | Mostra o diretório atual |  
| `ls`          | Lista arquivos e pastas |  
| `cd [pasta]`  | Muda de diretório |  
| `cd ..`       | Volta um nível |  
| `cd ~`        | Vai para a home do usuário |  

### 4.2. Manipulação de Arquivos
| Comando        | Descrição |  
|---------------|-----------|  
| `touch [arquivo]` | Cria um arquivo vazio |  
| `mkdir [pasta]`   | Cria uma pasta |  
| `cp [origem] [destino]` | Copia arquivos |  
| `mv [origem] [destino]` | Move ou renomeia arquivos |  
| `rm [arquivo]`    | Remove arquivos |  
| `rm -r [pasta]`   | Remove pastas recursivamente |  

### 4.3. Permissões
| Comando        | Descrição |  
|---------------|-----------|  
| `chmod [permissões] [arquivo]` | Altera permissões |  
| `chown [usuário:grupo] [arquivo]` | Muda dono/grupo |  

Exemplo:  
```bash
chmod 755 script.sh  # Dá permissão de execução  
chown root:root arquivo.txt  # Define dono como root  
```

### 4.4. Tarefas (Processos) e Sistema
| Comando        | Descrição |  
|---------------|-----------|  
| `ps`          | Lista processos ativos |  
| `top`         | Monitora processos em tempo real |  
| `kill [PID]`  | Encerra um processo |  
| `df -h`       | Mostra espaço em disco |  
| `free -h`     | Mostra uso de memória |  

### 4.5. Rede
| Comando       | Descrição |  
|--------------|-----------|  
| `ping [host]` | Testa conexão com um servidor |  
| `ifconfig`   | Mostra interfaces de rede |  
| `ssh [usuário@host]` | Conecta-se remotamente |  

---

## 5. Editores de Texto no Terminal

### 5.1. Nano (Simples)
```bash
nano arquivo.txt  # Abre o editor Nano  
```
- `Ctrl + O` → Salva  
- `Ctrl + X` → Sai  

### 5.2. Vim (Avançado)
```bash
vim arquivo.txt  # Abre o Vim  
```
- Modos:  
  - `i` → Modo de inserção  
  - `ESC` → Volta ao modo normal  
  - `:wq` → Salva e sai  

---

## 6. Gerenciamento de Pacotes

### 6.1. Debian/Ubuntu (APT)
```bash
sudo apt update          # Atualiza lista de pacotes  
sudo apt install [pacote] # Instala um pacote  
sudo apt remove [pacote]  # Remove um pacote  
```

### 6.2. Fedora (DNF)
```bash
sudo dnf install [pacote]  
sudo dnf remove [pacote]  
```

### 6.3. Arch Linux (Pacman)
```bash
sudo pacman -S [pacote]    # Instala  
sudo pacman -R [pacote]    # Remove  
```

---
