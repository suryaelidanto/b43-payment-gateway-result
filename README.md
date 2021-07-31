# Payment gateway with midtrans

`Midtrans` is a payment gateway that facilitates the needs of online businesses by providing services in various payment methods. This service allows industry players to operate more easily and increase sales. The payment methods provided are card payment, bank transfer, direct debit, e-wallet, over the counter, and others.

## Prepare

#### How to use ngrok for create public URLs

- Run application `npm run dev` on server side

- Download [ngrok](https://ngrok.com/) and place it in the payment-gateway or project folder

- Open terminal

* Run ngrok with port `3000` for client side :

  ```text
    ./ngrok http 3000
  ```

* Run ngrok with port `5000` for server side :

  ```text
    ./ngrok http 5000
  ```

#### Configuration on midtrans

- Create [midtrans](https://midtrans.com/) account and login

* Insert public URLs for Payment Notification :

  > Path : `settings/configuration`

  ![alt text](./notification.png "Payment Notification")

* Insert public URLs for Redirection Finish URL :

  > Path : `settings/snap preferences` and scroll down

  ![alt text](./finish.png "Redirection Finish URL")

* Install midtrans-client on server side

  ```text
  npm i midtrans-client
  ```
