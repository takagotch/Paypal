### Paypal
---
https://www.paypal.com/myaccount/money/

https://github.com/paypal

###### エクスプレスチェックアウト paypal
https://www.paypal.com/bizsignup/#/checkAccount

###### paypal developer
https://developer.paypal.com/developer/applications/edit/SB:QWRyaTZXYkxLLXo1WjVMV0ZqbWxWYWtaOWRLQlJ1MEhKM1QtNnlLSndMODlKR3VMYmhQQUlFT3FMbmNpZ294eDR2WWxwUDFJUDNvYXZHQy0=

(Register with Cardinal Commerce)[https://paypal3dsregistration.cardinalcommerce.com/UI/Registration.aspx]


###### cardinal
https://cardinaldocs.atlassian.net/wiki/spaces/CC/pages/7929857/Cardinal+Cruise+Standard

```
# かんたん決済　html
# スマート決済
# スマートボタン

<div id="smart-button-container">
      <div style="text-align: center;">
        <div id="paypal-button-container"></div>
      </div>
    </div>
  <script src="https://www.paypal.com/sdk/js?client-id=sb&currency=USD" data-sdk-integration-source="button-factory"></script>
  <script>
    function initPayPalButton() {
      paypal.Buttons({
        style: {
          shape: 'pill',
          color: 'gold',
          layout: 'vertical',
          label: 'buynow',
          
        },

        createOrder: function(data, actions) {
          return actions.order.create({
            purchase_units: [{"amount":{"currency_code":"USD","value":1}}]
          });
        },

        onApprove: function(data, actions) {
          return actions.order.capture().then(function(details) {
            alert('Transaction completed by ' + details.payer.name.given_name + '!');
          });
        },

        onError: function(err) {
          console.log(err);
        }
      }).render('#paypal-button-container');
    }
    initPayPalButton();
  </script>


```

```
# 今すぐ購入
# カートに入れる
# Smart Subscribe
# 購読する


```

```
```



```
```

```
```



```
```

```
```



```
```

```
```



```
```

```
```



```
```

```
```


