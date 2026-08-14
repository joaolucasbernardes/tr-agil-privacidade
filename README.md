# tr-agil-privacidade

Política de privacidade da extensão **TR Ágil**, as ferramentas da CPE para as
Turmas Recursais no eproc do TJMG.

Este repositório tem uma página só, o `index.html`. Não existe código da extensão
aqui. A Chrome Web Store exige que a política de privacidade fique num endereço
público, que o revisor consiga abrir de fora de qualquer rede corporativa, e é
esse endereço que este repositório serve.

No ar em:

```
https://joaolucasbernardes.github.io/tr-agil-privacidade/
```

É o endereço que fica no campo *Privacy policy URL* da ficha da extensão na loja.

## Por que ele é separado do repositório da extensão

No plano gratuito do GitHub, o Pages publica a partir de repositório público. Se
a política fosse uma pasta do repositório do código, o código inteiro teria que
ficar público junto com ela. Separando, cada coisa fica no lugar certo: este
repositório é público e tem uma página, o do código continua privado.

## A página

O `index.html` é autossuficiente. Todo o estilo mora dentro do próprio arquivo, e
ela não busca script, fonte nem folha de estilo de fora. Isso significa que ela
abre igual em qualquer navegador, não depende da rede do TJMG e não coloca
rastreador nenhum na frente de quem lê uma política de privacidade.

O texto explica, em linguagem direta:

* o que a extensão lê da tela do eproc e em que momento;
* o que ela guarda no navegador, com as chaves do `chrome.storage` listadas uma
  a uma e o que cada uma serve;
* quais endereços ela consulta, incluindo a consulta pública do PJe e o painel de
  impedimentos na rede interna do TJMG;
* o que ela grava nos autos, sempre depois de um clique de quem está usando;
* o papel do Gemini na triagem, já que a nota vem de um texto colado pelo próprio
  usuário.

O texto que está publicado corresponde à versão 1.10.7 da extensão e foi
atualizado em 14 de agosto de 2026.

## De onde vem o texto

A mesma política vai dentro do pacote da extensão, em
`src/options/privacidade.html`, porque a loja pede a divulgação sobre dados na
própria interface do produto e não só num link externo. O texto nasce lá, no
repositório da extensão, e chega aqui por cópia.

Os dois arquivos são idênticos, byte a byte. Quando um muda e o outro não, quem
está no ar deixa de valer para a versão que está instalada, então eles andam
sempre juntos.

Uma versão em Markdown da política não existe de propósito. Ela acabaria
divergindo das outras duas, e as que valem são a que está publicada e a que vai
no pacote.
