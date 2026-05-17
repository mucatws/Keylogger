# 🔐 Keylogger — Exemplo Educacional

> **⚠️ AVISO: Este projeto existe exclusivamente para fins educacionais.**
> Não use este código em máquinas de terceiros sem consentimento explícito.
> O uso não autorizado é ilegal em praticamente todos os países.

---

## O que é isso?

Este é um exemplo didático de como um **keylogger** funciona por dentro — um dos tipos mais simples de malware usados por hackers para coletar informações de usuários comuns.

O objetivo é mostrar, de forma transparente, como esse tipo de ameaça é construída, para que qualquer pessoa possa entender o risco e se proteger.

---

## O que esse código FAZ

- Registra as teclas digitadas e salva em um arquivo `log.txt` local
- **Roda apenas na máquina de quem o executa**

## O que esse código NÃO FAZ

- ❌ Não envia nada para nenhum servidor
- ❌ Não se comunica com hackers ou terceiros
- ❌ Não se instala no sistema automaticamente
- ❌ Não tem persistência (para quando o processo é encerrado)

---

## Por que hackers usam keyloggers?

Keyloggers são usados para capturar silenciosamente:

- Senhas de e-mail, bancos e redes sociais
- Números de cartão de crédito digitados
- Mensagens privadas
- Credenciais corporativas

Em ataques reais, o código é disfarçado dentro de outro programa e os dados são enviados automaticamente para o atacante — diferente deste exemplo, que não faz nenhuma exfiltração.

---

## Como se proteger

- **Não execute arquivos desconhecidos** recebidos por e-mail, Discord, WhatsApp ou baixados de fontes duvidosas
- **Use um antivírus atualizado** — keyloggers conhecidos são detectados por assinatura
- **Prefira autenticação de dois fatores (2FA)** — mesmo que uma senha seja capturada, o acesso fica bloqueado
- **Verifique processos em execução** no Gerenciador de Tarefas (Windows) ou `htop` (Linux) se suspeitar de algo
- **Em ambientes corporativos**, soluções de EDR (Endpoint Detection and Response) detectam comportamento de keylogger em tempo real

---

## Requisitos

```bash
pip install pynput
```

## Como executar (somente em máquina própria)

```bash
python keylogger.py
```

As teclas digitadas serão salvas em `log.txt` no mesmo diretório. Encerre com `Ctrl+C`.

---

## Licença

MIT — veja `LICENSE`. O uso é permitido somente para estudo e testes em ambiente próprio.
