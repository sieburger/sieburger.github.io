---
layout: home
title: Arduino
---

<p align="center">
  <img width="230" height="150" src="/assets/arduino.png">
</p>


**Arduino**[[2\]](https://pt.wikipedia.org/wiki/Arduino#cite_note-olhardigital-2)[[4\]](https://pt.wikipedia.org/wiki/Arduino#cite_note-Harduwin-4)[[5\]](https://pt.wikipedia.org/wiki/Arduino#cite_note-5) é uma plataforma de [prototipagem](https://pt.wikipedia.org/wiki/Protótipo) eletrônica de [hardware livre](https://pt.wikipedia.org/wiki/Hardware_livre) e de [placa única](https://pt.wikipedia.org/wiki/Computadores_de_placa_única),[[6\]](https://pt.wikipedia.org/wiki/Arduino#cite_note-6) projetada com um [microcontrolador](https://pt.wikipedia.org/wiki/Microcontrolador) [Atmel AVR](https://pt.wikipedia.org/wiki/Atmel_AVR) com suporte de [entrada/saída](https://pt.wikipedia.org/wiki/Entrada/saída) embutido, uma [linguagem de programação](https://pt.wikipedia.org/wiki/Linguagem_de_programação)padrão,[[7\]](https://pt.wikipedia.org/wiki/Arduino#cite_note-Arduino,_Policy-7) a qual tem origem em [Wiring](https://pt.wikipedia.org/wiki/Wiring), e é essencialmente [C](https://pt.wikipedia.org/wiki/C_(linguagem_de_programação))/[C++](https://pt.wikipedia.org/wiki/C%2B%2B).[[8\]](https://pt.wikipedia.org/wiki/Arduino#cite_note-buildprocess-8) O objetivo do projeto é criar ferramentas que são acessíveis, com baixo custo, flexíveis e fáceis de se usar por principiantes e profissionais. Principalmente para aqueles que não teriam alcance aos controladores mais sofisticados e ferramentas mais complicadas.[[9\]](https://pt.wikipedia.org/wiki/Arduino#cite_note-Arduino,_homepage-9)

Pode ser usado para o desenvolvimento de [objetos interativos](https://pt.wikipedia.org/wiki/Arduino#Aplicações) independentes, ou ainda para ser conectado a um [computador hospedeiro](https://pt.wikipedia.org/wiki/Host). Uma típica placa Arduino é composta por um controlador, algumas linhas de E/S digital e analógica, além de uma [interface serial](https://pt.wikipedia.org/wiki/Interface_serial) ou [USB](https://pt.wikipedia.org/wiki/Universal_Serial_Bus), para interligar-se ao hospedeiro, que é usado para programá-la e interagi-la em tempo real. A placa em si não possui qualquer recurso de [rede](https://pt.wikipedia.org/wiki/Rede_de_área_pessoal), porém é comum combinar um ou mais Arduinos deste modo, usando extensões apropriadas chamadas de [shields](https://pt.wikipedia.org/wiki/Arduino#Acessórios)[[10\]](https://pt.wikipedia.org/wiki/Arduino#cite_note-10). A interface do hospedeiro é simples, podendo ser escrita em várias linguagens. A mais popular é a [Processing](https://pt.wikipedia.org/wiki/Processing_(linguagem_de_programação)), mas outras que podem comunicar-se com a conexão serial são: [Max/MSP](https://pt.wikipedia.org/wiki/Max_(programa)),[[11\]](https://pt.wikipedia.org/wiki/Arduino#cite_note-11) [Pure Data](https://pt.wikipedia.org/wiki/Pure_Data),[[12\]](https://pt.wikipedia.org/wiki/Arduino#cite_note-ANPPOM_2008-12) [SuperCollider](https://pt.wikipedia.org/wiki/SuperCollider),[[13\]](https://pt.wikipedia.org/wiki/Arduino#cite_note-13) [ActionScript](https://pt.wikipedia.org/wiki/ActionScript)[[14\]](https://pt.wikipedia.org/wiki/Arduino#cite_note-14) e [Java](https://pt.wikipedia.org/wiki/Java_(linguagem_de_programação)).[[15\]](https://pt.wikipedia.org/wiki/Arduino#cite_note-Arduino,_Other_language_interfacing-15) Em 2010 foi realizado um documentário sobre a plataforma chamado *Arduino: The Documentary*.



**História**

O projeto iniciou-se na cidade de [Ivrea](https://pt.wikipedia.org/wiki/Ivrea), [Itália](https://pt.wikipedia.org/wiki/Itália), em [2005](https://pt.wikipedia.org/wiki/2005), com o intuito de interagir em projetos escolares de forma a ter um orçamento menor que outros sistemas de [prototipagem](https://pt.wikipedia.org/wiki/Protótipo) disponíveis naquela época. O sucesso foi sinalizado com o obtenção de uma menção honrosa na categoria *Comunidades Digitais* em [2006](https://pt.wikipedia.org/wiki/2006), pela **Prix Ars Electronica**,[[16\]](https://pt.wikipedia.org/wiki/Arduino#cite_note-16)[[17\]](https://pt.wikipedia.org/wiki/Arduino#cite_note-17) além da marca de mais de 50.000 placas vendidas até outubro de [2008](https://pt.wikipedia.org/wiki/2008).[[18\]](https://pt.wikipedia.org/wiki/Arduino#cite_note-18)[[19\]](https://pt.wikipedia.org/wiki/Arduino#cite_note-info.abril-19)

Atualmente, o seu hardware é feito através de um microcontrolador [Atmel AVR](https://pt.wikipedia.org/wiki/Atmel_AVR), sendo que este não é um requisito formal e pode ser estendido se tanto ele quanto a ferramenta alternativa suportarem a linguagem arduino e forem aceites pelo seu projeto.[[7\]](https://pt.wikipedia.org/wiki/Arduino#cite_note-Arduino,_Policy-7) Considerando esta característica, muitos projetos paralelos inspiram-se em cópias modificadas com placas de expansões, e acabam recebendo os [seus próprios nomes](https://pt.wikipedia.org/wiki/Arduino#Clones).



**Hardware**

A sua placa consiste num microcontrolador [Atmel](https://pt.wikipedia.org/wiki/Atmel) AVR de 8 [bits](https://pt.wikipedia.org/wiki/Bit), com componentes complementares para facilitar a programação e incorporação noutros circuitos. Um importante aspecto é a maneira padrão como os conectores são expostos, permitindo o [CPU](https://pt.wikipedia.org/wiki/Microprocessador) ser interligado a outros módulos expansivos, conhecidos como [shields](https://pt.wikipedia.org/wiki/Arduino#Acessórios). Os Arduinos originais utilizam a série de chips *megaAVR*, especialmente os *ATmega8*, *ATmega168*, *ATmega328* e a *ATmega1280*; porém muitos outros processadores foram utilizados por clones deles.[[20\]](https://pt.wikipedia.org/wiki/Arduino#cite_note-UFPA_Marcelo-20)

A grande maioria de placas inclui um [regulador linear](https://pt.wikipedia.org/wiki/Regulador_linear) de 5 [volts](https://pt.wikipedia.org/wiki/Volt) e um [oscilador de cristal](https://pt.wikipedia.org/wiki/Oscilador_de_cristal) de 16 [MHz](https://pt.wikipedia.org/wiki/Hertz) (podendo haver variantes com um [ressonador cerâmico](https://pt.wikipedia.org/wiki/Ressonador_cerâmico)), embora alguns esquemas como o *LilyPad* usem até 8 MHz e dispensem um regulador de tensão embutido, por terem uma forma específica de restrições de fator. Além de ser microcontrolador, o componente também é pré-programado com um [bootloader](https://pt.wikipedia.org/wiki/Boot), o que simplifica o carregamento de programas para o chip de [memória flash](https://pt.wikipedia.org/wiki/Memória_flash) embutido, em comparação com outros aparelhos que geralmente demandam um [chip programador](https://pt.wikipedia.org/wiki/Programador_(dispositivo)) externo.[[20\]](https://pt.wikipedia.org/wiki/Arduino#cite_note-UFPA_Marcelo-20)

[![img](https://upload.wikimedia.org/wikipedia/commons/thumb/d/d9/Arduino_ftdi_chip-1.jpg/200px-Arduino_ftdi_chip-1.jpg)](https://pt.wikipedia.org/wiki/Ficheiro:Arduino_ftdi_chip-1.jpg)



[FTDI](https://pt.wikipedia.org/wiki/FTDI)  

Conceptualmente, quando o seu software é utilizado, ele monta todas as placas sobre uma programação de conexão serial [RS-232](https://pt.wikipedia.org/wiki/RS-232), mas a forma de implementação no hardware varia em cada versão. As suas placas de serie contêm um simples circuito inversor para converter entre os sinais dos níveis RS-232 e [TTL](https://pt.wikipedia.org/wiki/Transistor-Transistor_Logic). Atualmente, existem alguns métodos diferentes para realizar a transmissão dos dados, como por placas programáveis via USB, adicionadas através de um chip adaptador *USB-para-Serial,* como o [FTDI](https://pt.wikipedia.org/wiki/FTDI) FT232. Algumas variantes, como o Arduino Mini e o não oficial Boarduino, usam um módulo, cabo adaptador USB, [bluetooth](https://pt.wikipedia.org/wiki/Bluetooth) ou outros métodos. Nestes casos, são usados com ferramentas microcontroladoras ao invés do Arduino IDE, utilizando assim a programação padrão AVR ISP.[[21\]](https://pt.wikipedia.org/wiki/Arduino#cite_note-21)[[22\]](https://pt.wikipedia.org/wiki/Arduino#cite_note-22)

A maioria dos pinos de E/S dos microcontroladores são para uso de outros circuitos. A versão *Diecimila*, que substituiu a *Duemilanove*, por exemplo, disponibiliza 14 pinos digitais, 6 das quais podem produzir sinais [MLP](https://pt.wikipedia.org/wiki/Modulação_por_largura_de_pulso), além de 6 entradas analógicas. Estes estão disponíveis em cima da placa, através de conectores fêmeas de 0,1 [polegadas](https://pt.wikipedia.org/wiki/Polegada) (ou 0,25 [centímetros](https://pt.wikipedia.org/wiki/Centímetro)).[[23\]](https://pt.wikipedia.org/wiki/Arduino#cite_note-Makezine_everything-23)

O modelo *Nano*, *Boarduino* e placas compatíveis com estas, fornecem conectores machos na parte de baixo da placa, para serem conectados em [protoboards](https://pt.wikipedia.org/wiki/Protoboard).[[20\]](https://pt.wikipedia.org/wiki/Arduino#cite_note-UFPA_Marcelo-20)

**Software**



O **Arduino IDE** é uma aplicação [multiplataforma](https://pt.wikipedia.org/wiki/Multiplataforma) escrita em [Java](https://pt.wikipedia.org/wiki/Java_(linguagem_de_programação)) derivada dos projetos [Processing](https://pt.wikipedia.org/wiki/Processing_(linguagem_de_programação)) e [Wiring](https://pt.wikipedia.org/wiki/Wiring).[[20\]](https://pt.wikipedia.org/wiki/Arduino#cite_note-UFPA_Marcelo-20)[[24\]](https://pt.wikipedia.org/wiki/Arduino#cite_note-24) É esquematizado para introduzir a programação para artistas e para pessoas não familiarizadas com o desenvolvimento de software. Inclui um editor de código com recursos de [realce de sintaxe](https://pt.wikipedia.org/wiki/Realce_de_sintaxe), [parênteses correspondentes](https://pt.wikipedia.org/wiki/Realce_de_sintaxe#Parênteses_correspondentes) e identação automática, sendo capaz de compilar e carregar programas para a placa com um único clique. Com isso não há a necessidade de editar [Makefiles](https://pt.wikipedia.org/wiki/Make) ou rodar programas em ambientes de [linha de comando](https://pt.wikipedia.org/wiki/Interpretador_de_comandos).[[9\]](https://pt.wikipedia.org/wiki/Arduino#cite_note-Arduino,_homepage-9)[[25\]](https://pt.wikipedia.org/wiki/Arduino#cite_note-baixar-25)

Tendo uma biblioteca chamada "Wiring", ele possui a capacidade de programar em [C](https://pt.wikipedia.org/wiki/C_(linguagem_de_programação))/[C++](https://pt.wikipedia.org/wiki/C%2B%2B). Isto permite criar com facilidade muitas operações de entrada e saída, tendo que definir apenas duas funções no pedido para fazer um programa funcional:[[20\]](https://pt.wikipedia.org/wiki/Arduino#cite_note-UFPA_Marcelo-20)

- *setup()* – Inserida no início, na qual pode ser usada para inicializar configuração, e
- *loop()* – Chamada para repetir um bloco de comandos ou esperar até que seja desligada.

Habitualmente, o primeiro programa que é executado tem a simples função de piscar um [LED](https://pt.wikipedia.org/wiki/Diodo_emissor_de_luz). No ambiente de desenvolvimento, o utilizador escreve um programa exemplo como este:[[26\]](https://pt.wikipedia.org/wiki/Arduino#cite_note-IBM_explicacao1-26)



```C
// define LED_PIN 13
int LED_PIN = 13;

void setup () {
    pinMode (LED_PIN, OUTPUT);     // habilita o pino 13 para saída digital (OUTPUT).
}

void loop () {
    digitalWrite (LED_PIN, HIGH);  // liga o LED.
    delay (1000);                  // espera 1 segundo (1000 milissegundos).
    digitalWrite (LED_PIN, LOW);   // desliga o LED.
    delay (1000);                  // espera 1 segundo.
}
```

O código acima não seria visto pelo compilador como um programa válido, então, quando o utilizador tentar carregá-lo para a placa, uma cópia do código é escrita para um arquivo temporário com um cabeçalho extra incluído no topo, e uma simples **função principal**como mostrada abaixo:

```C
# include<WProgram.h>

void setup () {
    pinMode (LED_PIN, OUTPUT);     // habilita o pino 13 para saída digital (OUTPUT).
}

void loop () {
    digitalWrite (LED_PIN, HIGH);  // liga o LED.
    delay (1000);                  // espera 1 segundo (1000 milissegundos).
    digitalWrite (LED_PIN, LOW);   // desliga o LED.
    delay (1000);                  // espera 1 segundo.
}

int main(void)
{
    // define LED_PIN 13
    int LED_PIN = 13;

    init();

    setup();

    for (;;)
        loop();

    return 0;
}
```

**"WProgram.h"** é um recurso para referenciar a biblioteca Wiring, e a função *main( )* apenas faz três chamadas distintas: *init( )*, definida em sua própria biblioteca, *setup( )* e *loop( )*, sendo as duas últimas configuradas pelo usuário.

O Arduino IDE usa o [Conjunto de ferramentas GNU](https://pt.wikipedia.org/wiki/Conjunto_de_ferramentas_GNU) e o *AVR Libc* para compilar os programas, para depois, com o avrdude, enviar os programas para a placa.[[27\]](https://pt.wikipedia.org/wiki/Arduino#cite_note-Apresentacao_PET-27)



***

Referências

1.  [«Arduino - Notas de lançamento»](http://arduino.cc/en/Main/ReleaseNotes) (em inglês). Projeto Arduino. Consultado em 12 de novembro de 2015
2. ↑ ***Ir para:a*** ***b*** ***c*** [«Arduino: Robótica para iniciantes»](https://web.archive.org/web/20100325132730/http://olhardigital.uol.com.br/central_de_videos/video_wide.php?id_conteudo=10981&%2FARDUINO+ROBOTICA+PARA+INICIANTES). [Olhar Digital](https://pt.wikipedia.org/wiki/Olhar_Digital). 21 de março de 2010. Consultado em 2 de abril de 2010. Arquivado do [original](http://olhardigital.uol.com.br/central_de_videos/video_wide.php?id_conteudo=10981&/ARDUINO+ROBOTICA+PARA+INICIANTES)em 25 de março de 2010. Tradução do nome *Arduino* pela matéria porém mantida no título da mesma.
3. [↑](https://pt.wikipedia.org/wiki/Arduino#cite_ref-3) [«Arduino - Software»](http://arduino.cc/en/Main/Software) (em inglês). Projeto Arduino. Consultado em 29 de janeiro de 2012
4. [↑](https://pt.wikipedia.org/wiki/Arduino#cite_ref-Harduwin_4-0) Substantivo próprio na língua Italiana, usado para nomear pessoas, porém de origem germânica da palavra "Harduwin" ou "Hardwin", que pode ser traduzida como Forte e Amigo, este nome se tornou popular graças ao rei italiano Arduino de Ivrea (1002-1015)[«Italian Baby Names»](https://web.archive.org/web/20131017062642/http://italian.about.com/library/name/blname_arduino.htm) (em inglês). Consultado em 16 de outubro de 2013. Arquivado do [original](http://italian.about.com/library/name/blname_arduino.htm) em 17 de outubro de 2013
5. [↑](https://pt.wikipedia.org/wiki/Arduino#cite_ref-5) rcruz (17 de janeiro de 2011). [«Arduíno: robôs em código aberto»](https://web.archive.org/web/20121117033435/http://planetasustentavel.abril.com.br/blog/paisagem-fabricada/2011/01/17/arduino-robos-codigo-aberto-279305/). *Artigo (Paisagem Fabricada - Planeta Sustentável)*. [Editora Abril](https://pt.wikipedia.org/wiki/Editora_Abril). Consultado em 29 de janeiro de 2012. Arquivado do [original](http://planetasustentavel.abril.com.br/blog/paisagem-fabricada/2011/01/17/arduino-robos-codigo-aberto-279305/) em 17 de novembro de 2012
6. [↑](https://pt.wikipedia.org/wiki/Arduino#cite_ref-6) [«Arduino: Conheça esta a plaforma de hardware livre»](http://blog.fazedores.com/arduino-conheca-esta-plataforma-de-hardware-livre-e-suas-aplicacoes/)
7. ↑ ***Ir para:a*** ***b*** [«O que faz uma Placa Arduino ser um Arduino?»](http://arduino.cc/en/Main/Policy) (em inglês). Projeto Arduino
8. [↑](https://pt.wikipedia.org/wiki/Arduino#cite_ref-buildprocess_8-0) [«Processo de construção do Arduino»](http://arduino.cc/en/Hacking/BuildProcess) (em inglês). Projeto Arduino
9. ↑ ***Ir para:a*** ***b*** [«Página principal do projeto»](http://www.arduino.cc/) (em inglês)
10. [↑](https://pt.wikipedia.org/wiki/Arduino#cite_ref-10) Incremente seu arduino com shields
11. [↑](https://pt.wikipedia.org/wiki/Arduino#cite_ref-11) *eberdahl*, [Stanford](https://pt.wikipedia.org/wiki/Universidade_Stanford). [«DIVULGAÇÃO : Workshop sobre novos controladores de música 29 de junho- 2 de julho»](http://www.unicamp.br/ciddic/index.php?pag=informativo 16_2010.html). *Anúncio de Workshop*(em [inglês](https://pt.wikipedia.org/wiki/Língua_inglesa) e [português](https://pt.wikipedia.org/wiki/Língua_portuguesa)). [UNICAMP](https://pt.wikipedia.org/wiki/Universidade_Estadual_de_Campinas). Consultado em 12 de agosto de 2010
12. ↑ ***Ir para:a*** ***b*** ***c*** José Henrique Padovani e Sérgio Freire (2008). [«Manufatura e programação de controladores: possibilidades de desenvolvimento para aplicação em sistemas musicais interativos»](https://web.archive.org/web/20131207090831/http://www.anppom.com.br/anais/anaiscongresso_anppom_2008/comunicas/COM396 - Padovani et al.pdf) (PDF). *XVIII Congresso da Associação Nacional de Pesquisa e Pós-Graduação (ANPPOM)*. Associação Nacional de Pesquisa e Pós-Graduação em Música. Consultado em 12 de agosto de 2010. Arquivado do [original](http://www.anppom.com.br/anais/anaiscongresso_anppom_2008/comunicas/COM396 - Padovani et al.pdf)(PDF) em 7 de dezembro de 2013
13. [↑](https://pt.wikipedia.org/wiki/Arduino#cite_ref-13) [«Página principal LAPPSO»](http://www.dmu.uem.br/lappso/index.php?title=Página_principal). Laboratório de Pesquisa e Produção Sonora da [UEM](https://pt.wikipedia.org/wiki/Universidade_Estadual_de_Maringá). Consultado em 12 de agosto de 2010. [Cópia arquivada em 1 de Dezembro de 2012](https://archive.is/20121201112639/http://www.dmu.uem.br/lappso/manual/index.php/Tutorial_SuperCollider)
14. [↑](https://pt.wikipedia.org/wiki/Arduino#cite_ref-14) [«Arduino e Flash»](http://www.arduino.cc/playground/Interfacing/Flash) (em inglês). Projeto Oficial
15. [↑](https://pt.wikipedia.org/wiki/Arduino#cite_ref-Arduino,_Other_language_interfacing_15-0) [«Interface Arduino para outras linguagens»](https://web.archive.org/web/20120724094437/http://arduino.cc/playground/Main/InterfacingWithSoftware) (em inglês). Projeto Arduino. Consultado em 9 de novembro de 2009. Arquivado do [original](http://www.arduino.cc/playground/Main/InterfacingWithSoftware)em 24 de julho de 2012
16. [↑](https://pt.wikipedia.org/wiki/Arduino#cite_ref-16) [«Arquivo Ars Electronica»](http://90.146.8.18/de/archives/prix_archive/prix_year_cat.asp?iProjectID=13638&iCategoryID=12420) (em alemão). Consultado em 18 de fevereiro de 2009
17. [↑](https://pt.wikipedia.org/wiki/Arduino#cite_ref-17) [«Arquivo Ars Electronica / RECONHECIMENTO»](http://90.146.8.18/de/archives/prix_archive/prix_projekt.asp?iProjectID=13789#) (em alemão). Consultado em 18 de fevereiro de 2009
18. [↑](https://pt.wikipedia.org/wiki/Arduino#cite_ref-18) Thompson, Clive (20 de outubro de 2008). [«Monte Isso. Compartilhe Isso. Lucre. O hardware livre pode funcionar?»](http://www.wired.com/techbiz/startups/magazine/16-11/ff_openmanufacturing). *Wired* (em inglês). **16** (11): 166–176. Consultado em 30 de abril de 2009
19. [↑](https://pt.wikipedia.org/wiki/Arduino#cite_ref-info.abril_19-0) Maurício Grego (9 de março de 2009). [«O hardware em ''código aberto''»](https://web.archive.org/web/20090312034818/http://info.abril.com.br/professional/tendencias/hardware-livre-leve-e-solto.shtml). *Entrevista*. [Info Online](https://pt.wikipedia.org/wiki/Info_Exame), [Editora Abril](https://pt.wikipedia.org/wiki/Editora_Abril). Consultado em 1 de agosto de 2010. Arquivado do [original](http://info.abril.com.br/professional/tendencias/hardware-livre-leve-e-solto.shtml) em 12 de março de 2009
20. ↑ ***Ir para:a*** ***b*** ***c*** ***d*** ***e*** ***f*** ***g*** ***h*** ***i*** ***j*** ***k*** Diego Kasuo, Felipe Amarante, Rodrigo Medeiros e Silvia Lins. Sob supervisão do Professor [Marcelo Barretto](http://www3.ufpa.br/marcelo/apresent.htm) (24 de maio de 2010). [«Projetos com Arduino»](http://www3.ufpa.br/marcelo/Home Page/Docs-APSH/Sem_APSH_1-2010/Projetos_com_Arduino.pdf) (PDF). [UFPA](https://pt.wikipedia.org/wiki/Universidade_Federal_do_Pará). Consultado em 12 de agosto de 2010[*[ligação inativa\]*](https://pt.wikipedia.org/wiki/Wikipédia:Ligação_inativa)
21. [↑](https://pt.wikipedia.org/wiki/Arduino#cite_ref-21) [«Boarduino - Placa compatível com Arduino»](http://www.ladyada.net/make/boarduino/) (em inglês). Consultado em 28 de janeiro de 2010
22. [↑](https://pt.wikipedia.org/wiki/Arduino#cite_ref-22) [«ArduinoBoardMini»](http://arduino.cc/en/Main/ArduinoBoardMini) (em inglês). Consultado em 28 de janeiro de 2010
23. [↑](https://pt.wikipedia.org/wiki/Arduino#cite_ref-Makezine_everything_23-0) Torrone, Phillip (28 de novembro de 2008). [«Open source hardware 2008»](https://web.archive.org/web/20090228211055/http://blog.makezine.com/archive/2008/11/_draft_open_source_hardwa.html) (em inglês). Make Online Magazine. Consultado em 12 de agosto de 2010. Arquivado do [original](http://blog.makezine.com/archive/2008/11/_draft_open_source_hardwa.html) em 28 de fevereiro de 2009
24. [↑](https://pt.wikipedia.org/wiki/Arduino#cite_ref-24) [«Hardware.processing»](https://web.archive.org/web/20100411142044/http://hardware.processing.org/) (em inglês). Processing.org. Consultado em 27 de março de 2010. Arquivado do [original](http://hardware.processing.org/) em 11 de abril de 2010
25. ↑ ***Ir para:a*** ***b*** [«Baixar o Software Arduino»](http://www.arduino.cc/en/Main/Software) (em inglês). Projeto Arduino. Consultado em 12 de novembro de 2009
26. [↑](https://pt.wikipedia.org/wiki/Arduino#cite_ref-IBM_explicacao1_26-0) Duane O'Brien (22 de dezembro de 2008). [«Princípios básicos do Arduino»](http://www.ibm.com/developerworks/br/library/os-arduino1/section2.html). *Projeto de um Jogo de Laser*. [IBM](https://pt.wikipedia.org/wiki/IBM). Consultado em 12 de agosto de 2010
27. ↑ ***Ir para:a*** ***b*** [«Brincando de embarcados com o Arduino»](http://pet.inf.ufsc.br/files/Apresentacao PET.pdf) (PDF). *Apresentação*. Programa de Educação Tutorial da [UFSC](https://pt.wikipedia.org/wiki/Universidade_Federal_de_Santa_Catarina). 17 de novembro de 2006. Consultado em 12 de agosto de 2010[*[ligação inativa\]*](https://pt.wikipedia.org/wiki/Wikipédia:Ligação_inativa)
28. [↑](https://pt.wikipedia.org/wiki/Arduino#cite_ref-28) Erika Guimar~aes Pereira da Fonseca / Mathyan Motta Beppu. **Orientador**: Prof. Alexandre Santos de la Vega (Dezembro de 2010). [«Apostila Arduino»](http://www.telecom.uff.br/pet/petws/downloads/tutoriais/arduino/Tut_Arduino.pdf) (PDF). [UFF](https://pt.wikipedia.org/wiki/Universidade_Federal_Fluminense). Consultado em 29 de janeiro de 2011
29. [↑](https://pt.wikipedia.org/wiki/Arduino#cite_ref-29) Renato Cruz (30 de outubro de 2011). [«USP cria centro de tecnologias interativas»](http://www.estadao.com.br/noticias/impresso,usp-cria-centro-de-tecnologias-interativas-,792457,0.htm). [Estadão](https://pt.wikipedia.org/wiki/O_Estado_de_S._Paulo). Consultado em 29 de janeiro de 2012
30. [↑](https://pt.wikipedia.org/wiki/Arduino#cite_ref-30) Laboratório de Robótica Móvel. [«CaRINA - Carro Robótico Inteligente para Navegação Autônoma»](https://web.archive.org/web/20120518112501/http://www.lrm.icmc.usp.br/carina/veiculos.html). [USP](https://pt.wikipedia.org/wiki/Universidade_de_São_Paulo). Consultado em 29 de janeiro de 2012. Arquivado do [original](http://www.lrm.icmc.usp.br/carina/veiculos.html) em 18 de maio de 2012
31. [↑](https://pt.wikipedia.org/wiki/Arduino#cite_ref-31) Thiago Kenji Batisti Sato **Orientador:** Professor Alessandro Zimmer (2010). [«Sistema Automotivo de Notificação de Acidente»](http://www.eletrica.ufpr.br/ufpr2/tccs/147.pdf) (PDF). [UFP](https://pt.wikipedia.org/wiki/Universidade_Federal_do_Paraná). Consultado em 29 de janeiro de 2012
32. [↑](https://pt.wikipedia.org/wiki/Arduino#cite_ref-32) Bruno Moro e Ricardo Suzin. [«Automação de sistema de irrigação de pastagem»](http://www.fag.edu.br/novo/arquivos/graduacao/engenharias/resumos/resumo03.pdf) (PDF). [FAG](https://pt.wikipedia.org/wiki/Fundação_Assis_Gurgacz). Consultado em 29 de janeiro de 2012
33. [↑](https://pt.wikipedia.org/wiki/Arduino#cite_ref-33) Francisco J. Gomes, Igor L. de Paula, Laís A. Vitoi, Lucas R. Conceição, Paulo C. R. Marciano (2011). [«O tutorial do motor de passo»](http://www.ufjf.br/peteletrica/files/2011/08/PROPOSTA-DE-COMPLEMENTO-À-EDUCAÇÃO-NA-ENGENHARIA-UTILIZANDO-FERRAMENTA-INTERATIVA-BASEADA-EM-FOSS-O-TUTORIAL-DO-MOTOR-DE-PASSO.pdf)(PDF). *COBENGE acessodata=29 de janeiro de 2012*. [UFJF](https://pt.wikipedia.org/wiki/Universidade_Federal_de_Juiz_de_Fora)[*[ligação inativa\]*](https://pt.wikipedia.org/wiki/Wikipédia:Ligação_inativa)
34. ↑ ***Ir para:a*** ***b*** [«Hardware»](http://www.arduino.cc/en/Main/Hardware) (em inglês). Projeto Arduino. Consultado em 12 de novembro de 2009
35. [↑](https://pt.wikipedia.org/wiki/Arduino#cite_ref-35) [«Em Oficina do Construtor: Arduino Nano 3.0»](https://web.archive.org/web/20100326122224/http://blog.makezine.com/archive/2010/03/in_the_maker_shed_arduino_nano_3.html) (em inglês). MAKE Online Magazine. 22 de março de 2010. Consultado em 12 de agosto de 2010. Arquivado do [original](http://blog.makezine.com/archive/2010/03/in_the_maker_shed_arduino_nano_3.html) em 26 de março de 2010
36. [↑](https://pt.wikipedia.org/wiki/Arduino#cite_ref-36) Maw, Carlyn e Nugent, Rory (23 de outubro de 2008). [«Configurando um Arduino numa protoboard»](https://web.archive.org/web/20101002164907/http://itp.nyu.edu/physcomp/Tutorials/ArduinoBreadboard) (em inglês). Computação Física da [NYU](https://pt.wikipedia.org/wiki/Universidade_de_Nova_Iorque). Consultado em 12 de outubro de 2010. Arquivado do [original](http://itp.nyu.edu/physcomp/Tutorials/ArduinoBreadboard) em 2 de outubro de 2010
37. [↑](https://pt.wikipedia.org/wiki/Arduino#cite_ref-37) [«Bem-vindo ao Arduino LilyPad»](http://web.media.mit.edu/~leah/LilyPad/index.html) (em inglês). [MIT](https://pt.wikipedia.org/wiki/Instituto_de_Tecnologia_de_Massachusetts). Consultado em 12 de agosto de 2010
38. [↑](https://pt.wikipedia.org/wiki/Arduino#cite_ref-38) Torrone, Phillip (27 de junho de 2007). [«Arduino, Arduino, Arduino (NG Plus)»](http://blog.makezine.com/archive/2007/06/arduino_arduino_arduino_m.html) (em inglês). MAKE Online Magazine. Consultado em 12 de agosto de 2010
39. [↑](https://pt.wikipedia.org/wiki/Arduino#cite_ref-39) Carlos Henrique de Paula, Edmar Anderson Lanes Junior e Luana do Amaral Harada (27 de novembro de 2008). [«Sistema de Automação Residencial Personalizado para fins de Acessibilidade»](http://engcomp.dainf.ct.utfpr.edu.br/oficinas/IF62J/2008b/PaulaLanesJrHarada2008.pdf) (PDF). *Oficina*. [UFTPR](https://pt.wikipedia.org/wiki/Universidade_Tecnológica_Federal_do_Paraná). Consultado em 12 de agosto de 2010[*[ligação inativa\]*](https://pt.wikipedia.org/wiki/Wikipédia:Ligação_inativa)
40. [↑](https://pt.wikipedia.org/wiki/Arduino#cite_ref-40) [«Arduino Uno - Especificações»](http://www.makershed.com/ProductDetails.asp?ProductCode=MKSP4&Show=ExtInfo) (em inglês). Makeshed. Consultado em 10 de outubro de 2010
41. [↑](https://pt.wikipedia.org/wiki/Arduino#cite_ref-41) [«Buy Arduino in authorized and official Arduino distributors»](https://web.archive.org/web/20170414081213/http://www.arduino.org/buy/distributors). *Arduino.org* (em inglês). Consultado em 13 de abril de 2017. Arquivado do [original](http://www.arduino.org/buy/distributors) em 14 de abril de 2017
42. [↑](https://pt.wikipedia.org/wiki/Arduino#cite_ref-42) [«Arduino - Credits»](https://www.arduino.cc/en/main/credits). *www.arduino.cc* (em inglês). Consultado em 13 de abril de 2017
43. [↑](https://pt.wikipedia.org/wiki/Arduino#cite_ref-43) [«Buy Arduino in authorized and official Arduino distributors»](https://web.archive.org/web/20170414081213/http://www.arduino.org/buy/distributors#america). *Arduino.org* (em inglês). Consultado em 13 de abril de 2017. Arquivado do [original](http://www.arduino.org/buy/distributors#america) em 14 de abril de 2017
44. [↑](https://pt.wikipedia.org/wiki/Arduino#cite_ref-44) [«Arduino Blog » Send in the clones»](https://blog.arduino.cc/2013/07/10/send-in-the-clones/). Consultado em 13 de abril de 2017
45. [↑](https://pt.wikipedia.org/wiki/Arduino#cite_ref-45) [«Arduino - ArduinoShields»](http://www.arduino.cc/en/Main/ArduinoShields) (em inglês). Consultado em 20 de março de 2009
46. [↑](https://pt.wikipedia.org/wiki/Arduino#cite_ref-46) [«Então você quer fazer um Arduino»](http://www.arduino.cc/en/Main/Policy) (em inglês). Projeto Arduino. Consultado em 17 de março de 2009
47. [↑](https://pt.wikipedia.org/wiki/Arduino#cite_ref-47) [«Esquemas Abertos, Freeduino»](https://web.archive.org/web/20080410220309/http://www.freeduino.org/freeduino_open_designs.html) (em inglês). Consultado em 13 de março de 2008. Arquivado do [original](http://www.freeduino.org/freeduino_open_designs.html) em 10 de abril de 2008
48. [↑](https://pt.wikipedia.org/wiki/Arduino#cite_ref-48) [«Nome de Microcontroladores do "Rei Arduino"»](http://www.freeduino.org/duino.html) (em inglês). Freeduino. Consultado em 18 de agosto de 2010
49. [↑](https://pt.wikipedia.org/wiki/Arduino#cite_ref-49) Cunningham, Collin (9 de junho de 2008). [«Freeduino SB»](https://web.archive.org/web/20081013100900/http://blog.makezine.com/archive/2008/06/freeduino_sb.html) (em inglês). MAKE Online Magazine. Consultado em 14 de agosto de 2010. Arquivado do [original](http://blog.makezine.com/archive/2008/06/freeduino_sb.html) em 13 de outubro de 2008
50. ↑ ***Ir para:a*** ***b*** ***c*** [«Arquivos Esquemáticos de PCB Freeduino»](https://web.archive.org/web/20080410220309/http://www.freeduino.org/freeduino_open_designs.html) (em inglês). Freeduino Oficial. 27 de abril de 2008. Consultado em 14 de agosto de 2010. Arquivado do [original](http://www.freeduino.org/freeduino_open_designs.html) em 10 de abril de 2008
51. [↑](https://pt.wikipedia.org/wiki/Arduino#cite_ref-51) Priya Ganapati (19 de agosto de 2009). [«Hackers Criam uma Placa-mãe Modular»](http://www.wired.com/gadgetlab/2009/08/modular-motherboard/) (em inglês). [Wired](https://pt.wikipedia.org/wiki/Wired). Consultado em 14 de agosto de 2010
52. [↑](https://pt.wikipedia.org/wiki/Arduino#cite_ref-52) [«Componentes de Dispositivos Genéricos»](http://hackerspaces.org/wiki/GenericHardwareComponents) (em inglês). Hackerspaces. 18 de junho de 2009. Consultado em 14 de agosto de 2010
53. [↑](https://pt.wikipedia.org/wiki/Arduino#cite_ref-53) Marc de Vinck (21 de março de 2009). [«Em Oficina do Construtor: Seeeduino V1.1»](http://blog.makezine.com/archive/2009/03/in_the_maker_shed_seeeduino.html?CMP=OTC-0D6B48984890) (em inglês). MAKE Online Magazine. Consultado em 14 de agosto de 2010[*[ligação inativa\]*](https://pt.wikipedia.org/wiki/Wikipédia:Ligação_inativa)
54. [↑](https://pt.wikipedia.org/wiki/Arduino#cite_ref-54) Torrone, Phillip (23 de agosto de 2009). [«O Wiseduino»](http://blog.makezine.com/archive/2009/08/the_wiseduino.html) (em inglês). MAKE Online Magazine. Consultado em 14 de agosto de 2009[*[ligação inativa\]*](https://pt.wikipedia.org/wiki/Wikipédia:Ligação_inativa)
55. [↑](https://pt.wikipedia.org/wiki/Arduino#cite_ref-55) [«Brasuíno»](https://web.archive.org/web/20110711220321/http://brasuino.holoscopio.com/). Projeto oficial. Consultado em 19 de julho de 2011. Arquivado do [original](http://brasuino.holoscopio.com/) em 11 de julho de 2011


***
[home](./)

***
mail me: marcio at sieburger dot link