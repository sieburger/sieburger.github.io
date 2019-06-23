---
layout: home
title: Email personalizado no Github
---


[Fonte original](https://blog.johansen.software/custom-email-domain-via-gmail-when-github-pages-is-your-web-host-e4a9d7e03d36)

Desde o ano passado, hospedei meu site e blog pessoal por meio do serviço de páginas gratuito do GitHub. Qualquer repositório GitHub com uma configuração Jekyll pode se tornar automaticamente um site estático hospedado, que um registro CNAME pode colocar em um domínio personalizado. Meu repositório atualmente vive em http://johansen.software.

É uma configuração de desenvolvedor bastante comum, mas e o e-mail? Você poderia manter uma única micro instância viva para atuar como um servidor de correio, mas esse tipo de derrota o propósito. Recentemente, precisei configurar o gian@johansen.software e ver qual seria a maneira mais simples de fazer isso.

### Roteamento de e-mail por meio de um provedor de e-mail em nuvem

Ao final desse processo, você terá seu endereço de e-mail personalizado configurado para enviar e receber e-mails, e todos eles serão encaminhados para uma conta de e-mail secundária, como o gmail, por meio de um serviço de e-mail em nuvem. Dessa forma, você evita a necessidade de um host e pode gerenciar todos os seus e-mails através de uma única conta.

#### Etapa 1: inscreva-se com uma solução de email empresarial

O Google Apps é o mais comum, mas recentemente abandonou o nível gratuito, por isso estão fora. Acabei indo com o [Mailgun](https://www.mailgun.com/), embora você pudesse usar o Zoho ou outra plataforma, se quiser.

Depois de se inscrever, clique em **Domínios** e, em seguida, em **Adicionar novo domínio**. Você será solicitado a inserir o URL do domínio em que deseja receber o e-mail.

#### Etapa 2: configurar os registros MX do DNS

![custom-email-1.png](https://cdn-images-1.medium.com/max/1200/1*1L6pYQbzsc5-fs0Q6TFXOQ.png)

Um registro MX diz para onde rotear o SMTP. Um registro TXT armazena texto simples, geralmente para configuração. Configurar o Mailgun significará atualizar seus registros MX e TXT para apontar para eles.
Eu sempre usei o Cloudflare, mas é sempre o mesmo processo. Se você não tem certeza de como ou onde fazer isso, é mais provável que tenha sido feito onde quer que você tenha comprado o nome do seu domínio.
Crie os registros DNS que eles solicitam que você crie e clique em continuar. Você desejará definir o TTL o mais baixo possível, por enquanto, para reduzir os tempos de cache. Depois que isso estiver configurado, você poderá empurrá-los de volta para automático.

#### Etapa 3: configurar rotas de email

No menu superior da Mailgun, clique em **Routes** e, em seguida, em **Create A Route**. Uma expressão *catchall* será acionada em qualquer email enviado para esse domínio, o que provavelmente é o que você deseja.

Em **Actions**, você precisará marcar a caixa de seleção **forward** e digitar o endereço de e-mail para enviar e receber e-mails. Depois de adicionar a rota, você poderá receber e-mails usando seu domínio personalizado. Tente enviar um e-mail para o endereço e você verá o encaminhamento automaticamente.

#### Etapa 4: Configurar o SMTP da área de trabalho

![custom-email-2.png](https://cdn-images-1.medium.com/max/1200/1*uYVg05gp9Mq-vidixgskoA.png)

Para enviar e-mails, você precisará usar o SMTP porque, sem um host, você não terá uma interface on-line. Eu configurei o meu com o Apple Mail, mas há muitas opções diferentes aqui. Você encontrará suas informações de SMTP na seção Domains.

No Apple Mail, os servidores de correio de saída são inseridos em Preferências, em Contas e, em seguida, em Configurações do servidor. Não estamos configurando o IMAP para isso porque as mensagens recebidas chegarão até você por meio do endereço de e-mail de encaminhamento que você configurou anteriormente. Você selecionará um servidor de saída quando enviar uma mensagem.

Depois disso, você configura tudo para enviar e receber e-mails. Deixe um comentário se você ficar preso a qualquer momento.

***
[home](../)
<br>
[github](../github.html)
<br>