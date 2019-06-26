---
layout: home
title: Secure Shell (SSH)
comments: true
---



**Secure Shell** (**SSH**) é um [protocolo de rede](https://pt.wikipedia.org/wiki/Protocolo_de_rede) [criptográfico](https://pt.wikipedia.org/wiki/Criptografia) para operação de serviços de rede de forma segura sobre uma rede insegura.[[1\]](https://pt.wikipedia.org/wiki/Secure_Shell#cite_note-rfc4251-1) O melhor exemplo de aplicação conhecido é para [login](https://pt.wikipedia.org/wiki/Login) remoto de usuários a sistemas de computadores.

O SSH fornece um [canal seguro](https://pt.wikipedia.org/wiki/Canal_seguro) sobre uma rede insegura em uma arquitetura [cliente-servidor](https://pt.wikipedia.org/wiki/Cliente-servidor), conectando uma aplicação [cliente SSH](https://pt.wikipedia.org/w/index.php?title=Cliente_SSH&action=edit&redlink=1) com um [servidor SSH](https://pt.wikipedia.org/w/index.php?title=Servidor_SSH&action=edit&redlink=1).[[2\]](https://pt.wikipedia.org/wiki/Secure_Shell#cite_note-rfc4252-2) Aplicações comuns incluem [login](https://pt.wikipedia.org/wiki/Login) em [linha de comando](https://pt.wikipedia.org/wiki/Linha_de_comando) remoto e execução remota de comandos, mas qualquer [serviço de rede](https://pt.wikipedia.org/w/index.php?title=Serviço_de_rede&action=edit&redlink=1) pode ser protegido com SSH. A especificação do protocolo distingue entre duas versões maiores, referidas como SSH-1 e SSH-2.

A aplicação mais visível do protocolo é para acesso a [contas shell](https://pt.wikipedia.org/w/index.php?title=Conta_shell&action=edit&redlink=1) em sistemas operacionais do [tipo Unix](https://pt.wikipedia.org/wiki/Tipo_Unix), mas também verifica-se algum uso limitado no [Windows](https://pt.wikipedia.org/wiki/Windows). Em 2015, a Microsoft anunciou que incluiriam suporte nativo para SSH em uma liberação futura.[[3\]](https://pt.wikipedia.org/wiki/Secure_Shell#cite_note-3)

O SSH foi projetado como um substituto para o [Telnet](https://pt.wikipedia.org/wiki/Telnet) e para protocolos de [shell](https://pt.wikipedia.org/wiki/Shell) remotos inseguros como os protocolos Berkeley [rlogin](https://pt.wikipedia.org/wiki/Rlogin), [rsh](https://pt.wikipedia.org/wiki/Remote_Shell) e [rexec](https://pt.wikipedia.org/w/index.php?title=Remote_Process_Execution&action=edit&redlink=1). Estes protocolos enviam informações, notavelmente [senhas](https://pt.wikipedia.org/wiki/Senha), em [texto puro](https://pt.wikipedia.org/wiki/Texto_puro), tornando-os suscetíveis à interceptação e divulgação usando [análise de pacotes](https://pt.wikipedia.org/wiki/Analisador_de_pacotes).[[4\]](https://pt.wikipedia.org/wiki/Secure_Shell#cite_note-4) A [criptografia](https://pt.wikipedia.org/wiki/Criptografia) usada pelo SSH objetiva fornecer confidencialidade e integridade de dados sobre uma rede insegura, como a [Internet](https://pt.wikipedia.org/wiki/Internet), apesar dos arquivos vazados por [Edward Snowden](https://pt.wikipedia.org/wiki/Edward_Snowden) indicarem que a [Agência de Segurança Nacional](https://pt.wikipedia.org/wiki/Agência_de_Segurança_Nacional) pode algumas vezes descriptografar o SSH, permitindo-os ler o conteúdo de sessões SSH.[[5\]](https://pt.wikipedia.org/wiki/Secure_Shell#cite_note-Spiegel2014-5)

***

# Artigos

[Sobre SSH](./ssh/about-ssh.html)
<br>

[Conferindo chaves SSH existentes](./ssh/checking-ssh.html)
<br>

[Testando SSH Key](./ssh/testing.html)
<br>

[Adicionando ao agente ssh](./ssh/agent-ssh.html)
<br>

[Adicionando chave SSH para a conta do Github](./ssh/ssh-github.html)
<br>

***

### Definição



O SSH usa [criptografia de chave pública](https://pt.wikipedia.org/wiki/Criptografia_de_chave_pública) para [autenticar](https://pt.wikipedia.org/wiki/Autenticação) o computador remoto e e permiti-lo autenticar o usuário, se necessário.[[2\]](https://pt.wikipedia.org/wiki/Secure_Shell#cite_note-rfc4252-2) Há várias maneiras de usar o SSH, uma é usar pares de chave pública-privada geradas automaticamente para simplesmente encriptar uma conexão de rede e então usar autenticação por [senha](https://pt.wikipedia.org/wiki/Senha) para logar.

Outra maneira é usar um par de chaves pública-privada geradas manualmente para realizar a autenticação, permitindo que usuários ou programas loguem sem ter que especificar uma senha. Neste cenário, qualquer um pode produzir um par correspondente de chaves diferentes (pública e privada). A chave pública é colocada em todos os computadores que devem permitir o acesso ao proprietário da chave privada correspondente (o proprietário mantem o segredo da chave privada). Uma vez que a autenticação é baseada na chave privada, a chave em si nunca é transferida por meio da rede durante a autenticação. O SSH apenas verifica se a mesma pessoa que oferece a chave pública também possui a chave privada correspondente. Em todas as versões do SSH é importante verificar [chaves públicas](https://pt.wikipedia.org/wiki/Criptografia_de_chave_pública) desconhecidas, isto é, [associar as chaves públicas com as identidades](https://pt.wikipedia.org/wiki/Criptografia_de_chave_pública#Associando_chaves_públicas_a_identidades), antes de aceitá-las como válidas. Aceitar a chave pública de um atacante sem validação autorizará o atacante como um usuário válido.



***
[home](./)

***

#### Referências

1. [↑](https://pt.wikipedia.org/wiki/Secure_Shell#cite_ref-rfc4251_1-0) Network Working Group of the IETF, January 2006, [RFC 4251](https://tools.ietf.org/html/rfc4251), The Secure Shell (SSH) Protocol Architecture
2. ↑ ***Ir para:a*** ***b*** ***c*** Network Working Group of the IETF, January 2006, [RFC 4252](https://tools.ietf.org/html/rfc4252), The Secure Shell (SSH) Authentication Protocol
3. [↑](https://pt.wikipedia.org/wiki/Secure_Shell#cite_ref-3) Peter Bright (June 2, 2015). [«Microsoft bringing SSH to Windows and PowerShell»](http://arstechnica.com/information-technology/2015/06/microsoft-bringing-ssh-to-windows-and-powershell/). [Ars Technica](https://pt.wikipedia.org/w/index.php?title=Ars_Technica&action=edit&redlink=1) Verifique data em: [ajuda](https://pt.wikipedia.org/wiki/Ajuda:Erros_nas_referências#bad_date)
4. [↑](https://pt.wikipedia.org/wiki/Secure_Shell#cite_ref-4) [SSH Hardens the Secure Shell](http://www.serverwatch.com/news/print.php/3551081), Serverwatch.com
5. [↑](https://pt.wikipedia.org/wiki/Secure_Shell#cite_ref-Spiegel2014_5-0) [«Prying Eyes: Inside the NSA's War on Internet Security»](http://www.spiegel.de/international/germany/inside-the-nsa-s-war-on-internet-security-a-1010361.html). [Spiegel Online](https://pt.wikipedia.org/wiki/Spiegel_Online). December 28, 2014 Verifique data em: [ajuda](https://pt.wikipedia.org/wiki/Ajuda:Erros_nas_referências#bad_date)
6. [↑](https://pt.wikipedia.org/wiki/Secure_Shell#cite_ref-6) [SSH setup manual](http://wiki.qnap.com/wiki/How_To_Set_Up_Authorized_Keys)
7. [↑](https://pt.wikipedia.org/wiki/Secure_Shell#cite_ref-7) [«Service Name and Transport Protocol Port Number Registry»](http://www.iana.org/assignments/port-numbers). *iana.org*