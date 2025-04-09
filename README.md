# Script de Atualização e Deploy de Aplicação Web

## Descrição

Este script shell automatiza o processo de atualização de um servidor Linux, instalação do Apache, e deploy de uma aplicação web estática contida em um arquivo `.zip`.

## Etapas executadas

1. **Atualização do sistema:**
   - `apt-get update`: Atualiza a lista de pacotes.
   - `apt-get upgrade -y`: Atualiza os pacotes instalados.

2. **Instalação de pacotes:**
   - `apache2`: Servidor web.
   - `unzip`: Utilitário para descompactar arquivos `.zip`.

3. **Deploy da aplicação:**
   - Acessa o diretório `/tmp`.
   - Descompacta o arquivo `main.zip`.
   - Entra na pasta `linux-site-dio-main`.
   - Copia todos os arquivos da aplicação para o diretório `/var/www/html`.

## Observações

- Certifique-se de que o arquivo `main.zip` esteja previamente presente no diretório `/tmp`.
- Execute este script com privilégios de superusuário (`sudo`).
- O conteúdo anterior de `/var/www/html` será substituído.

## Uso

```bash
sudo ./nome-do-script.sh
```

## Requisitos

- Distribuição baseada em Debian (ex: Ubuntu).
- Permissões de root.

## Autor
Script criado para fins educacionais e organizacionais.

#### **💻Feito por Guilherme Gugelmin** 

