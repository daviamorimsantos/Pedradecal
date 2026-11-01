# Ateliê de Doces — site institucional

Site estático responsivo para divulgação de doces artesanais em Pedra de Cal, Riachão das Neves — BA.

## O que está implementado

- Página única responsiva com navegação mobile.
- Catálogo com os produtos e preços que foram informados nas imagens: mousse no potinho (250 ml, R$ 7,00) e cremosinho (R$ 3,00).
- Botões de pedido que abrem o WhatsApp comercial `+55 77 99970-2260`, com mensagem preenchida.
- Fotos fornecidas para o projeto, textos alternativos, metadados básicos e favicon.
- Não há painel administrativo ou banco de dados: o catálogo é conteúdo estático e deve ser atualizado no código quando houver mudanças.

## Executar localmente

Não há etapa de build nem dependências. Abra `index.html` no navegador ou execute um servidor local na pasta do projeto:

```bash
python -m http.server 8000
```

Depois acesse `http://localhost:8000`.

## Publicar no GitHub

1. Crie um repositório vazio no GitHub.
2. Envie todos os arquivos desta pasta para a raiz do repositório (incluindo `assets/`).
3. Faça commit e push.

## Publicar na Vercel

1. Entre na Vercel e escolha **Add New → Project**.
2. Importe o repositório GitHub.
3. Como é um site estático sem etapa de build, deixe o framework como **Other** e não configure Build Command nem Output Directory.
4. Clique em **Deploy**. A raiz do projeto contém o `index.html`.

Também é possível fazer deploy pela CLI da Vercel, executando `vercel` na pasta do projeto.

## Dados que precisam ser confirmados antes da divulgação

- Nome comercial definitivo (o site usa “Ateliê de Doces” provisoriamente).
- Se há entrega, retirada ou ambos; taxas e áreas atendidas, se existirem.
- Horários, formas de pagamento e sabores disponíveis.
- Confirmar se os preços anunciados nas imagens continuam válidos.

## Observações

- Os links de WhatsApp usam o número informado e dependem de o número estar ativo no WhatsApp.
- O site não recebe pagamentos nem registra pedidos em banco de dados; encaminha o cliente para conversar diretamente pelo WhatsApp.
- As fontes são carregadas do Google Fonts; se estiverem indisponíveis, há fontes de sistema como alternativa.
