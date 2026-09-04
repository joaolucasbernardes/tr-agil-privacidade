# tr-agil-privacidade

Política de privacidade da **TR Ágil**, extensão que reúne as ferramentas da CPE
usadas pelas Turmas Recursais no EPROC do TJMG.

Há somente uma página neste repositório: `index.html`. O código da extensão não
fica aqui. A Chrome Web Store exige uma política de privacidade em endereço
público, acessível ao revisor mesmo fora de uma rede corporativa, e este
repositório existe para publicar esse endereço.

No ar em:

```
https://joaolucasbernardes.github.io/tr-agil-privacidade/
```

Esse é o endereço informado no campo *Privacy policy URL* da página da extensão
na loja.

## Por que ele é separado do repositório da extensão

No plano gratuito do GitHub, o Pages só publica conteúdo vindo de um repositório
público. Manter a política junto do código obrigaria a tornar público também o
repositório inteiro da extensão. A separação resolve isso: aqui fica apenas a
página pública, enquanto o código continua em seu repositório privado.

## A página

O `index.html` funciona sozinho. Seus estilos estão no próprio arquivo, sem
scripts, fontes ou folhas de estilo externas. Assim, a página abre da mesma
forma em qualquer navegador, não depende da rede do TJMG e não submete o leitor
a nenhum rastreamento.

Em linguagem direta, a página informa:

* quais dados são lidos da tela do EPROC e quando isso acontece;
* o que permanece no navegador, com cada chave do `chrome.storage` e sua
  finalidade;
* quais endereços recebem consultas, entre eles a consulta pública do PJe e o
  painel de impedimentos da rede interna do TJMG;
* o que pode ser gravado nos autos, sempre após uma ação de quem usa a extensão;
* como o Gemini participa da triagem, pois a resposta utilizada é colada pelo
  próprio usuário.

A política publicada corresponde à versão 1.14.7 da extensão e recebeu sua
última atualização em 2 de setembro de 2026.

## De onde vem o texto

A política também acompanha o pacote da extensão em
`src/options/privacidade.html`. A loja pede que as informações sobre o uso de
dados apareçam na interface do produto, além do endereço externo. A versão
mantida no repositório da extensão é a origem desta cópia.

Os dois arquivos precisam permanecer idênticos, byte por byte. Se apenas um
deles for atualizado, a página publicada deixa de corresponder ao que acompanha
a versão instalada; por isso, qualquer alteração deve alcançar ambos.

Não há uma terceira versão da política em Markdown. Isso evita mais uma cópia
sujeita a divergências: valem somente a página publicada e o arquivo incluído no
pacote.
