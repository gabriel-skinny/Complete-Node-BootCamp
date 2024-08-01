# Contéudo Etapa-1 (Seção 1,2, 3)

## Nodejs 
Artigos base: https://nodejs.org/en/learn/getting-started/differences-between-nodejs-and-the-browser


Definição NodeJs: Um ambiente de runtime de Javascript separado do Browser que roda pelo V8

V8 Engine: É o runtime do Browser que executa o javascript no GoogleChrome

Vantagem do Nodejs: A Node.js app runs in a single process, without creating a new thread for every request. Node.js provides a set of asynchronous I/O primitives in its standard library that prevent JavaScript code from blocking and generally, libraries in Node.js are written using non-blocking paradigms, making blocking behavior the exception rather than the norm.

When Node.js performs an I/O operation, like reading from the network, accessing a database or the filesystem, instead of blocking the thread and wasting CPU cycles waiting, Node.js will resume the operations when the response comes back.

Diferença de rodar Javascript no Browser vs NodeJs: O Primeiro possui muitas funções da manipulação com a DOM, cokkies e outras funções especificas relacionadas com contexto do Browser em que se está inserido. E o segundo possui funções nativas para lidar com o sistema operacional.

Beneficios do Nodejs: Single-Thread, Baseado em Eventos, e não Bloquia o I/O. 
-  Bom Uso: Montar apps que precisam se servir de muitos dados. 
- Mal Uso: Apps que tem um processamento server-side muito grande. Outras linguagens: Rails, Php, Pyhton

## Como o Broswer Funciona
Referencia: 
- Socket: https://en.wikipedia.org/wiki/Network_socket
- TCP/IP: https://en.wikipedia.org/wiki/Internet_protocol_suite#

Modelo Cliente e Servidor: O Cliente requisita através do Browser informações de um servidor 

1 Etapa DNS: Transforma a url que o cliente colocou no broswer na url do servidor real

2 Etapa TCP/IP Socket: Quando o cliente bate na url uma conexação socket TCP/IP permanece ligada entre o servidor e o cliente. Eles definem como os dados irão trafegar na internet
 - TCP (Transfer Control Protocol): Quebra as request e responses em chunks antes de serem enviados, depois quando chegar no seu destino ele juntará todos os pacotes na response original
 -  IP (Internet Protocol): Envia e roteia os pacotes separados pelo TCP

3 Etapa Http request: O Cliente envia uma request https para o servidor
 - Http: É um sistema de comunicação que determina uma serie de regras para a transmissão de dados

4 Etapa Http response: O Servidor retorna com uma resposta regular pelo formato Http

5 Etapa Http Responses dos recursos: O Html, Css e todas as imagens e arquivos contidos no servidor são devolvidos ao cliente através do Http por multiplas responses.

## Divisão da Web

Front-End: Desenvolvimento de Arquivos staticos de um web-server(Html, Css e Javascript)

Back-End: Desenvolvimento de Aplicativo ou Api que torna o web-Server dinâmico, retornando dados mutaveis de um Database
- Web-Server -> Um computador que está conectado na internet, que possui os arquivos de código e um servidor Http que se comunica na internet.
- Server-side-rendering -> Conjunto de códigos de uma linguagem de programção que manipula os arquivos do web server e os retorna pelo Http.
- Client-Side-Renering(Api) -> Conjunto de códigos que manipula e retorna dados puros  