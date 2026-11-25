# Pagamentos PE — protótipo do módulo gerencial

Protótipo navegável para discutir o MVP do módulo administrativo de pagamentos do Governo de Pernambuco. Inclui visão geral, cobranças, cadastro de serviços pagos, conciliação e integrações.

## Acessar

O protótipo é publicado pelo GitHub Pages a partir de `index.html` na raiz da branch `main`.

Para executar localmente, abra `index.html` no navegador. Não há dependências nem instalação.

## Escopo do protótipo

As telas usam dados ilustrativos. Os formulários e botões demonstram navegação; não há persistência, autenticação, integração real com Portal PE, Sefaz ou PagBank, nem movimentação financeira. O cadastro permite selecionar simultaneamente **Cartão, PIX, Boleto e DAE**. DAE é um documento de arrecadação; meios de quitação, destinatário e conciliação dependem das regras autorizadas para cada serviço.

Antes da implementação produtiva, validar o fluxo do serviço piloto, a configuração de arrecadação, o contrato das APIs, os perfis de acesso e as regras de segurança e auditoria.

## Estrutura

- `index.html`: protótipo estático publicado pelo GitHub Pages.
- `dist/index.html`: cópia do protótipo para empacotamento e desenvolvimento.
