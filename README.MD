# Criar Chave SSH

## Via PowerShell (ADMINISTRADOR)

**Abrir o PowerShell como administrador:**

```bash
ssh-keygen -t ed25519 -C "11joao44@gmail.com"
```

**Habilitar o serviço ssh-agent:**

```bash
Set-Service -Name ssh-agent -StartupType Manual
```

**Iniciar o serviço ssh-agent:**

```bash
Start-Service ssh-agent
```

**Adicionar a chave SSH ao ssh-agent:**

```bash
ssh-add C:\Users\11joa\.ssh\id_ed25519
```

**Adicionar a chave SSH ao GitHub:**

```bash
Get-Content C:\Users\11joa\.ssh\id_ed25519.pub | clip
```

**Copie o conteúdo da sua chave pública para a área de transferência:**

## Verificar se possui uma chave SSH no diretório

```bash
$ ls ~/.ssh/
```

## Gerar nova Chave SSH

```bash
$ ssh-keygen -t ed25519 -C "your_email@example.com"
```

## Iniciar ssh-agent

```bash
$ eval "$(ssh-agent -s)"
```

## Verificar qual o caminho da chave publica

```bash
$ $ ls ~/.ssh/id_ed25519.pub
```

## Acessar o caminho chave publica

```bash
$ cd ~/.ssh/
```

## Veriicar a chave publica dentro da pasta

```bash
$ cat id_ed25519
```

## Verificar se o agente SSH está em execução

```bash
$ ps aux | grep ssh-agent
```