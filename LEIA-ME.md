# Perfil DOMINADOR · Voz do Ser convida

Site do resultado do teste de perfil de comunicação.
Arquivo único e autossuficiente: o logo está embutido no HTML, não há pasta `assets`.

## Publicar no GitHub Pages

1. Crie um repositório com este nome exato (copie da linha sozinha abaixo,
   sem espaço nem pontuação no fim):

       perfil-dominador

   Se o GitHub disser "will be created as perfil-dominador-", sobrou um caractere
   no fim do campo: apague o último e o hífen some.
2. Suba os DOIS arquivos desta pasta: `index.html` e `.nojekyll`
   (o `.nojekyll` é oculto no Windows — ative "Itens ocultos" na aba Exibir do Explorador).
3. Em **Settings › Pages**, escolha a branch `main` e a pasta `/ (root)`.
4. O endereço fica: `https://SEU-USUARIO.github.io/perfil-dominador/`

> Atenção: no plano gratuito o GitHub Pages só funciona em repositório público,
> e mesmo no plano pago o site publicado é público. Por isso o `index.html`
> já nasce com `<meta name="robots" content="noindex, nofollow">`: ele não é
> indexado pelo Google, mas quem tiver o link consegue abrir.

## Nome do convidado no link

Acrescente `?n=` com o primeiro nome (ou nome e sobrenome) no fim do endereço:

    https://SEU-USUARIO.github.io/perfil-dominador/?n=Ricardo
    https://SEU-USUARIO.github.io/perfil-dominador/?n=Ana%20Paula

A pessoa vê "Olá, Ricardo." na abertura. Sem o `?n=`, aparece só "Olá.".
Use `%20` no lugar do espaço.

## Gênero do texto no link

Alguns trechos do resultado flexionam ("é empático" / "é empática"). Acrescente `&g=`:

    ...?n=Ricardo&g=m     → masculino
    ...?n=Ana&g=f         → feminino
    ...?n=Alex            → neutro (padrão, quando o `g` não vem)

No **neutro** as frases são reescritas para não flexionar — não fica "empático(a)",
fica "Tem empatia". Use quando não souber, ou quando a pessoa preferir assim.

Não precisa montar isso na mão: abra o **`GERADOR DE LINKS - PERFIS.html`**, na raiz
do projeto. Você escolhe o perfil, digita o nome, marca o gênero e ele monta o link
e a mensagem de WhatsApp prontos para copiar.

## O que editar

Tudo que muda está no bloco `CONFIG`, no fim do `index.html`:

- `solucoes` — link do botão principal. Já configurado com
  `https://vozdoser.netlify.app/` (a página do QR Code). Se ficar vazio,
  o botão passa a apontar para `CONFIG.site`.
- `solucoesTitulo` / `solucoesSub` — texto do botão principal
- `whatsapp`, `waTexto` — número e mensagem pronta do WhatsApp
- `site`, `instagram`, `linkedin`, `endereco`

Não edite nada fora do bloco CONFIG sem necessidade.
