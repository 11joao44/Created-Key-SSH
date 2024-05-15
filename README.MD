# Criar Chave SSH

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