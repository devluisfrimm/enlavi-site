# enlavi.com.br — página de vendas

Abra a pasta no Antigravity para editar.

## Antes de publicar
1. `index.html` → bloco CONFIG no fim do arquivo:
   - `checkoutUrl`: link do checkout do produto na Kiwify
   - `metaPixelId`: ID do Pixel da Meta (pode ficar vazio por enquanto)
2. `index.html`, `termos.html` e `privacidade.html` → rodapé: troque
   `[NOME DO RESPONSÁVEL] · [CPF OU CNPJ] · [ENDEREÇO: CIDADE – UF]`
   (exigência do Decreto 7.962/2013).

## Publicar na Vercel
1. Suba esta pasta num repositório no GitHub (devluisfrimm/enlavi-site).
2. vercel.com → Add New → Project → importe o repositório → Deploy (sem build, é HTML puro).
3. Project → Settings → Domains → adicione `enlavi.com.br` e `www.enlavi.com.br`.
4. No registro.br → enlavi.com.br → DNS → "Editar zona", crie os registros que a Vercel mostrar
   (normalmente A `@` → 76.76.21.21 e CNAME `www` → cname.vercel-dns.com).
5. Aguarde a propagação e teste no celular.
