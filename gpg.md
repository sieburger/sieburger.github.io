---
layout: home
title: GPG keys
---



**GNU Privacy Guard** (**GnuPG** ou **GPG**) é um [software livre](https://pt.wikipedia.org/wiki/Software_livre) alternativo ao conjunto de softwares [criptográficos](https://pt.wikipedia.org/wiki/Criptografia) [PGP](https://pt.wikipedia.org/wiki/Pretty_Good_Privacy) da [Symantec](https://pt.wikipedia.org/wiki/Symantec),[[2\]](https://pt.wikipedia.org/wiki/GNU_Privacy_Guard#cite_note-2) e em conformidade com o [RFC 4880](https://tools.ietf.org/html/rfc4880), a especificação de rastreio de padrões [IETF](https://pt.wikipedia.org/wiki/Internet_Engineering_Task_Force) do [OpenPGP](https://pt.wikipedia.org/wiki/OpenPGP). Versões modernas do PGP (e Filecrypt da Veridis) possuem [interoperabilidade](https://pt.wikipedia.org/wiki/Interoperabilidade) com o GnuPG e com outros sistemas compatíveis com o OpenPGP.

GnuPG é parte da [Free Software Foundation](https://pt.wikipedia.org/wiki/Free_Software_Foundation) e do [Projeto GNU](https://pt.wikipedia.org/wiki/Projeto_GNU). Além disso, ele recebeu grande patrocínio do [Governo Alemão](https://pt.wikipedia.org/wiki/Política_da_Alemanha).[[3\]](https://pt.wikipedia.org/wiki/GNU_Privacy_Guard#cite_note-3)
<br>

***

# Artigos

[Buscando chaves existentes](./gpg/checking-keys.html)
<br>
[Gerando uma nova chave GPG](./gpg/generating-gpg.html)
<br>
[Adicionando a chave GPG a conta do Github](./gpg/add-gpg.html)
<br>
[Commits usando GPG](./gpg/commits-gpg.html)

***


**História**

O projeto GnuPG foi iniciado em 1997 pelo o [alemão](https://pt.wikipedia.org/wiki/Alemães) [Werner Koch](https://pt.wikipedia.org/wiki/Werner_Koch), que ainda é o principal desenvolvedor e o programa de criptografia de e-mail foi inicialmente desenvolvido por [Phil Zimmermann](https://pt.wikipedia.org/wiki/Phil_Zimmermann). A versão 1.0.0 foi anunciada em 7 de setembro de 1999. O [Ministério Federal Alemão de Economia e Tecnologia](https://pt.wikipedia.org/w/index.php?title=Ministério_Federal_Alemão_de_Economia_e_Tecnologia&action=edit&redlink=1) patrocinou a documentação e a portabilidade para o sistema [Microsoft Windows](https://pt.wikipedia.org/wiki/Microsoft_Windows) em 2000. A versão 2.0 foi anunciada em 13 de novembro de 2006. O antigo ramo 1.x, cuja última versão é o 1.4.11 será continuado em paralelo com o novo GnuPG 2 pois existem mudanças significativas na arquitetura do programa.[[4\]](https://pt.wikipedia.org/wiki/GNU_Privacy_Guard#cite_note-4)

**Visão Geral**



O GnuPG é um programa de software de [criptografia híbrida](https://pt.wikipedia.org/w/index.php?title=Criptografia_híbrida&action=edit&redlink=1) porque usa uma combinação de [criptografia de chave simétrica](https://pt.wikipedia.org/wiki/Criptografia_de_chave_simétrica) convencional por questões de velocidade e [criptografia de chave pública](https://pt.wikipedia.org/wiki/Criptografia_de_chave_pública) para facilitar a troca segura de chaves, geralmente usando a chave pública do destinatário para criptografar uma [chave de sessão](https://pt.wikipedia.org/w/index.php?title=Chave_de_sessão&action=edit&redlink=1) que é usada apenas uma vez. Este modo de operação faz parte do padrão OpenPGP e faz parte do PGP desde sua primeira versão.

A série GnuPG 1.x usa uma biblioteca criptográfica integrada, enquanto a série GnuPG 2.x a substitui por [Libgcrypt](https://pt.wikipedia.org/w/index.php?title=Libgcrypt&action=edit&redlink=1).

O GnuPG criptografa mensagens usando [pares de chaves assimétricas](https://pt.wikipedia.org/wiki/Criptografia_de_chave_pública) geradas individualmente pelos usuários do GnuPG. As chaves públicas resultantes podem ser trocadas com outros usuários de diversas maneiras, como [servidores de chaves](https://pt.wikipedia.org/w/index.php?title=Servidro_de_chaves_(criptografia)&action=edit&redlink=1) da Internet. Eles devem sempre ser trocados cuidadosamente para evitar falsificação de identidade corrompendo correspondências de identidade de "proprietário" de chave pública. Também é possível adicionar uma [assinatura digital](https://pt.wikipedia.org/wiki/Assinatura_digital) criptográfica a uma mensagem, para que a integridade e o remetente da mensagem possam ser verificados, se uma correspondência específica invocada não tiver sido corrompida.

O GnuPG também suporta algoritmos de [criptografia simétrica](https://pt.wikipedia.org/wiki/Criptografia_simétrica). Por padrão, o GnuPG usa o algoritmo simétrico [CAST5](https://pt.wikipedia.org/wiki/CAST5). O GnuPG não usa software ou algoritmos patenteados ou restritos. Em vez disso, o GnuPG usa uma variedade de outros algoritmos não patenteados.[[5\]](https://pt.wikipedia.org/wiki/GNU_Privacy_Guard#cite_note-5)



**Utilização**



Apesar do programa básico do GnuPG ter uma interface de linha de comando, existem várias interfaces gráficas.

Por exemplo, GnuPG esta integrado ao [Kmail](https://pt.wikipedia.org/wiki/Kmail), cliente de e-mail do [KDE](https://pt.wikipedia.org/wiki/KDE) e ao [Evolution](https://pt.wikipedia.org/w/index.php?title=Software_Evolution&action=edit&redlink=1), o cliente de email do [GNOME](https://pt.wikipedia.org/wiki/GNOME). KDE e GNOME são os desktops [Linux](https://pt.wikipedia.org/wiki/Linux) mais populares. Além da integração com os clientes de e-mail, existem as interfaces gráficas [Seahorse](https://pt.wikipedia.org/wiki/Seahorse) para GNOME e [KGPG](https://pt.wikipedia.org/w/index.php?title=KGPG&action=edit&redlink=1) para KDE.

Para [Mac OS X](https://pt.wikipedia.org/wiki/Mac_OS_X), o projeto Mac GPG provê diversas interfaces [Aqua](https://pt.wikipedia.org/wiki/Aqua_(interface)) para integração com a criptografia e gerenciamento de chaves, assim como instalações GnuPG via o instalador do Mac OS X:.[[6\]](https://pt.wikipedia.org/wiki/GNU_Privacy_Guard#cite_note-6) Além disso o software [GPGTools](https://pt.wikipedia.org/w/index.php?title=GPGTools&action=edit&redlink=1)[[7\]](https://pt.wikipedia.org/wiki/GNU_Privacy_Guard#cite_note-7) instala todas as aplicações OpenPGP ([GPG Keychain Access](https://pt.wikipedia.org/w/index.php?title=GPG_Keychain_Access&action=edit&redlink=1)), plugins ([GPGMail](https://pt.wikipedia.org/w/index.php?title=GPGMail&action=edit&redlink=1)) e dependências ([MacGPG](https://pt.wikipedia.org/w/index.php?title=MacGPG&action=edit&redlink=1)) para utilizar criptografia usando o GnuPG.

Aplicações de mensagens instantâneas como o [Psi](https://pt.wikipedia.org/w/index.php?title=Psi_(instant_messaging_client)&action=edit&redlink=1) e [Fire](https://pt.wikipedia.org/w/index.php?title=Fire_(cliente_de_mensagens_instantâneas&action=edit&redlink=1) podem trocar mensagens seguras automaticamente quando o GnuPG esta instalado e configurado. Softwares Web-based, como o [Horde](https://pt.wikipedia.org/wiki/Horde) também utiliza o GnuPG. O plugin [Enigmail](https://pt.wikipedia.org/wiki/Enigmail) prove suporte GnuPG as plataformas [Mozilla Thunderbird](https://pt.wikipedia.org/wiki/Mozilla_Thunderbird) e [SeaMonkey](https://pt.wikipedia.org/wiki/SeaMonkey). De maneira similar, o [Enigform](https://pt.wikipedia.org/w/index.php?title=Enigform&action=edit&redlink=1) prove suporte para que o [Mozilla Firefox](https://pt.wikipedia.org/wiki/Mozilla_Firefox). [FireGPG](https://pt.wikipedia.org/w/index.php?title=FireGPG&action=edit&redlink=1) (extensão para o Mozilla Firefox) foi descontinuado em 7 de Junho de 2010.

Em 2005 o G10 Code e o Intervation anunciaram o [Gpg4win](https://pt.wikipedia.org/wiki/Gpg4win), um software que inclui o GnuPG para o Windows e plugins para [Windows Explorer](https://pt.wikipedia.org/wiki/Windows_Explorer) e [Outlook](https://pt.wikipedia.org/wiki/Microsoft_Outlook). Essas ferramentes estão unificadas em um instalador tornando fácil seu uso na plataforma Windows.



**Processos**



GnuPg criptografa mensagens utilizando a [criptografia de chaves assimétricas](https://pt.wikipedia.org/wiki/Criptografia_de_chaves_assimétricas). O resultado é que chaves públicas podem ser trocadas com outros usuários de várias maneiras, uma delas são os [servidores de chaves](https://pt.wikipedia.org/w/index.php?title=Servidores_de_chaves&action=edit&redlink=1). As chaves devem sempre ser trocadas com cuidado para evitar o roubo de identidade. É possível também adicionar uma [assinatura digital](https://pt.wikipedia.org/wiki/Assinatura_digital) a mensagem de maneira que a integridade da mensagem e do remetente possam ser verificadas. GnuPG também suporta algoritmos de [criptografia simétrica](https://pt.wikipedia.org/wiki/Criptografia_simétrica). Por padrão GnuPG usa o algoritmo simétrico [CAST5](https://pt.wikipedia.org/wiki/CAST5).

GnuPG não utiliza algoritmos patenteados ou restritos, como por exemplo o algoritmo [IDEA](https://pt.wikipedia.org/wiki/International_Data_Encryption_Algorithm) utilizado no PGP (Na verdade é possível utilizar o IDEA no GnuPG fazendo o download de um plugin, entretanto isso pode requerer a compra de licença em alguns países aonde o IDEA é patenteado). Ao invés disso, GnuPG usa uma variedade de outros algoritmos não patenteados, incluindo:[[8\]](https://pt.wikipedia.org/wiki/GNU_Privacy_Guard#cite_note-8)

- Cifra de Blocos (algoritmos simetricos ou de chave privada): [CAST5](https://pt.wikipedia.org/wiki/CAST5), [Camellia](https://pt.wikipedia.org/w/index.php?title=Camellia_(cipher)&action=edit&redlink=1), [Triple DES](https://pt.wikipedia.org/w/index.php?title=Triple_DES&action=edit&redlink=1), [AES](https://pt.wikipedia.org/wiki/Advanced_Encryption_Standard), [Blowfish](https://pt.wikipedia.org/w/index.php?title=Blowfish_(cipher)&action=edit&redlink=1), and [Twofish](https://pt.wikipedia.org/wiki/Twofish).
- Cifras assimetricas (algoritmos de chave pública) : [ElGamal](https://pt.wikipedia.org/w/index.php?title=ElGamal&action=edit&redlink=1) and [RSA](https://pt.wikipedia.org/w/index.php?title=RSA_(algorithm)&action=edit&redlink=1)
- Criptografia de Hash: [RIPEMD-160](https://pt.wikipedia.org/wiki/RIPEMD-160), [MD5](https://pt.wikipedia.org/wiki/MD5), [SHA-1](https://pt.wikipedia.org/wiki/SHA-1), [SHA-2](https://pt.wikipedia.org/wiki/SHA-2), and [Tiger](https://pt.wikipedia.org/w/index.php?title=Tiger_(cryptography)&action=edit&redlink=1)
- Assinatura digital: [DSA](https://pt.wikipedia.org/w/index.php?title=Digital_Signature_Algorithm&action=edit&redlink=1) and [RSA](https://pt.wikipedia.org/w/index.php?title=RSA_(algorithm)&action=edit&redlink=1)

GnuPG é um software de criptografia hibrido que utiliza a combinação de [criptografia de chaves simétricas](https://pt.wikipedia.org/w/index.php?title=Criptografia_de_chaves_simétricas&action=edit&redlink=1) para velocidade e [criptografia de chaves publicas](https://pt.wikipedia.org/w/index.php?title=Criptografia_de_chaves_publicas&action=edit&redlink=1) para a troca de mensagens seguras. Isso é conseguido utilizando a criptografia de chave pública para encriptar uma [chave de sessão](https://pt.wikipedia.org/w/index.php?title=Chave_de_sessão&action=edit&redlink=1) que é utilizada apenas uma vez. Esse modo de operação é parte do padrão OpenPGP e é parte do PGP desde sua primeira versão.



**Problemas**



O padrão OpenPGP especifica diversos métodos de [assinatura digital](https://pt.wikipedia.org/wiki/Assinatura_digital). Em 2003, ao tentar tornar um desses métodos mais eficiente, uma vulnerabilidade de segurança no GnuPG foi introduzida. Esse erro afetou apenas um método de assinatura de mensagens, e apenas algumas versões do GnuPG (1.0.2 ao 1.2.3). Como existiam menos de 1000 chaves desse tipo nos servidores[[9\]](https://pt.wikipedia.org/wiki/GNU_Privacy_Guard#cite_note-9) e a maioria das pessoas não utilizava esse método, o dano causado por esse erro parece ter sido minimo. Suporte a esse método foi removido das versões do GnuPG após a descoberta desse erro (nas versões 1.2.4 e posteriores).

Duas outras vulnerabilidades foram descobertas em 2006. A primeira é que a utilização de scripts que utilizam o GnuPG para verificação de assinatura poderiam resultar em falsos positivos.[[10\]](https://pt.wikipedia.org/wiki/GNU_Privacy_Guard#cite_note-10) A segunda é que mensagens non-MIME eram vulneráveis a inserção de dados não cobertas pela assinatura digital que seriam erroneamente reportadas como parte da mensagem assinada:[[11\]](https://pt.wikipedia.org/wiki/GNU_Privacy_Guard#cite_note-11) Em ambos os casos, versões atualizadas do GnuPG foram disponibilizas.

GnuPG é um sistema baseado em linha de comando e não possui uma [API](https://pt.wikipedia.org/wiki/Application_programming_interface) que possa ser incorporado em outros softwares. [GPGME](https://pt.wikipedia.org/w/index.php?title=GPGME&action=edit&redlink=1) é uma [API wrapper](https://pt.wikipedia.org/w/index.php?title=API_wrapper&action=edit&redlink=1) que lê a saída do GnuPG. Várias interfaces gráficas foram criadas utilizando o GPGME. Como o GPGME utiliza uma interface especial do GnuPG desenvolvida para o uso automatizado, uma API estável entre os componentes é possível. Possíveis erros de segurança em uma aplicação não se propagam para o código do GnuPG devido a barreira entre os processos. Existem outros softwares que encapsulam a linha de comando em um script [Perl](https://pt.wikipedia.org/wiki/Perl) (por exemplo: [gpg-dialog](https://pt.wikipedia.org/w/index.php?title=Gpg-dialog&action=edit&redlink=1)).

***

**Referências**

1.  [«Release notes»](https://www.gnupg.org/download/release_notes.html). gnupg.org. 28 de dezembro de 2016. Consultado em 27 de junho de 2017
2. [↑](https://pt.wikipedia.org/wiki/GNU_Privacy_Guard#cite_ref-2) [«Gnu Privacy Guard»](https://www.gnupg.org/faq/gnupg-faq.html#compatible). GnuPG.org
3. [↑](https://pt.wikipedia.org/wiki/GNU_Privacy_Guard#cite_ref-3) Florian Rötzer (15 de novembro de 1999). [«Bundesregierung fördert Open Source»](https://www.heise.de/newsticker/meldung/Bundesregierung-foerdert-Open-Source-24110.html). heise online. Consultado em 27 de junho de 2017
4. [↑](https://pt.wikipedia.org/wiki/GNU_Privacy_Guard#cite_ref-4) Werner Koch (13 de novembro de 2006). [«GnuPG 2.0 released»](https://lists.gnupg.org/pipermail/gnupg-announce/2006q4/000239.html). gnupg.org. Consultado em 27 de junho de 2017
5. [↑](https://pt.wikipedia.org/wiki/GNU_Privacy_Guard#cite_ref-5) [«GnuPG Features»](https://www.gnupg.org/features.en.html). Consultado em 1 de outubro de 2009
6. [↑](https://pt.wikipedia.org/wiki/GNU_Privacy_Guard#cite_ref-6) [«Mac GNU Privacy Guard»](http://macgpg.sourceforge.net/). *sourceforge*. Consultado em 27 de junho de 2017
7. [↑](https://pt.wikipedia.org/wiki/GNU_Privacy_Guard#cite_ref-7) [«GPGTools Installer»](http://www.gpgtools.org/). *gpgtools*. Consultado em 27 de junho de 2017
8. [↑](https://pt.wikipedia.org/wiki/GNU_Privacy_Guard#cite_ref-8) [«GnuPG Features»](http://www.gnupg.org/features.en.html). Consultado em 27 de junho de 2017
9. [↑](https://pt.wikipedia.org/wiki/GNU_Privacy_Guard#cite_ref-9) Werner Koch (27 de novembro de 2003). [«GnuPG's ElGamal signing keys compromised»](https://lists.gnupg.org/pipermail/gnupg-announce/2003q4/000160.html). gnupg.org. Consultado em 27 de junho de 2017
10. [↑](https://pt.wikipedia.org/wiki/GNU_Privacy_Guard#cite_ref-10) Werner Koch (15 de fevereiro de 2006). [«False positive signature verification in GnuPG»](https://lists.gnupg.org/pipermail/gnupg-announce/2006q1/000211.html). gnupg.org. Consultado em 17 de junho de 2017
11. [↑](https://pt.wikipedia.org/wiki/GNU_Privacy_Guard#cite_ref-11) Werner Koch (9 de março de 2006). [«GnuPG does not detect injection of unsigned data»](https://lists.gnupg.org/pipermail/gnupg-announce/2006q1/000218.html). gnupg.org. Consultado em 27 de junho de 2017

***

[fonte](https://pt.wikipedia.org/wiki/GNU_Privacy_Guard)


***

[home](./)

***
mail me: marcio at sieburger dot link
