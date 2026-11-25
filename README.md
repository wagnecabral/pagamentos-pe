# Pagamentos PE — protótipo do módulo gerencial

Protótipo navegável para discutir o MVP do módulo administrativo de pagamentos do Governo de Pernambuco. Inclui visão geral, cobranças, cadastro de serviços pagos, conciliação e integrações.

## Executar

Abra `dist/index.html` no navegador. Não há dependências nem instalação.

Para servir localmente, opcionalmente execute:

```bash
python3 -m http.server 8000 --directory dist
```

Depois acesse `http://localhost:8000`.

## Publicar no GitHub Pages

1. Em **Settings → Pages → Build and deployment**, selecione **GitHub Actions**.
2. O workflow `.github/workflows/pages.yml` publicará o conteúdo de `dist/` a cada envio para `main`.

## Escopo do protótipo

As telas usam dados ilustrativos. Os formulários e botões demonstram navegação; não há persistência, autenticação, integração real com Portal PE, Sefaz ou PagBank, nem movimentação financeira. O cadastro permite selecionar simultaneamente **Cartão, PIX, Boleto e DAE**. DAE é um documento de arrecadação; meios de quitação, destinatário e conciliação dependem das regras autorizadas para cada serviço.

Antes da implementação produtiva, validar o fluxo do serviço piloto, a configuração de arrecadação, o contrato das APIs, os perfis de acesso e as regras de segurança e auditoria.

## Estrutura

```text
dist/index.html              Protótipo estático navegável
.github/workflows/pages.yml  Publicação pelo GitHub Pages
README.md                    Instruções e limites do protótipo
```
