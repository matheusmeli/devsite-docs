## Obter informações de pagamento

Este endpoint é utilizado para obter os dados de um Advanced Payment feito a partir de seu id.  Veja o diagrama abaixo que ilustra o processo de captura de pagamento por meio da API de Advanced Payments.

![get-payment-info](/images/wallet-connect/get-payment-information.pt.png)


Para obter informações de determinado pagamento, envie um **GET** ao endpoint [/v1/advanced_payments/{advanced_payment_id}](/developers/pt/reference/wallet_connect/_advanced_payments_advanced_payment_id/get) e execute a requisição ou, se preferir, utilize o `curl` abaixo.

[[[
```curl

curl -X GET \
    'https://api.mercadopago.com/v1/advanced_payments/ADVANCED_PAYMENT_ID?client.id=CLIENT_ID' \
      -H 'Authorization: Bearer YOUR_ACCESS_TOKEN'

```
]]]

Ao executar o `request` você poderá receber diferentes tipos de respostas originadas por razões específicas. Veja a seção [Respostas](/developers/pt/docs/wallet-connect/advanced-payments/get-payment-information/returns) para mais informações.