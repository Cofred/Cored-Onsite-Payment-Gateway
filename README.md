# Cored Onsite Payment Gateway
Onsite payment gateway sponsored by Cofred to pay via Cofred, Credit/Debit Cards and Mobile Money.

Cofred onsite payment can be used to receive payments from Cofred, Credit/Debit Cards and Mobile Money on your website.

Follow the details below to implement Cofred pay button on your website-

You will need to set javascript parameters and load a Cofred Javascript library

Load Cofred library like this in your page
<script src="https://cofredpay.com/sdk/cofred.js"></script>

https://cofredpay.com/sdk/cofred.js is the Javascript library url.

# Required Javacript variables-

1) cfd_merchantid - Your Cofred merchant ID here.
2) cfd_accesstoken - Your Cofred access token here.
3) amount - Add amount you want to debit using the API.
4) item_name - Your Item name.
5) payment_method - You need to select which method you need to apply to pay. (E.g. - Cofred, Card, MobileMoney)
6) currency - Pass currency you want to charge user (Supported currencies GHS, NGN, USD, KES, UGX, TZS)
7) merchant_ref - Your transaction reference number to identify transaction in callbacks.
8) notify_url - Here you need to pass url where you want to receive callbacks of each transactions.
9) success_url - Pass url to redirect after payment success.
10) cancel_url - Pass url to redirect in case of payment cancellations.

# Load button at your place

You can load Cofred payment button whereever you need. You just need to add below code where you need the payment button

<div id="cofred-button-container"></div>

Or load "cofred-button-container" in your ID of any HTML tags.

# Process to receive callback

