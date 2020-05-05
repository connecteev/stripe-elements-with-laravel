Setup instructions:

1. git clone https://github.com/connecteev/stripe-elements-with-laravel connecteev_andre_madarang_stripe_elements_laravel_vue
(this is a clone of Andre Madarang's repo: https://github.com/drehimself/stripe-elements-with-laravel 
which is based on his youtube video: https://www.youtube.com/watch?v=BB-nXTPyNtE)

2. 
cd connecteev_andre_madarang_stripe_elements_laravel_vue
composer install
php artisan key:generate

3. 
cp .env.example .env
update .env with:
DB_DATABASE=connecteev_andre_madarang_stripe_elements_laravel_vue
DB_USERNAME=root     
DB_PASSWORD=root 

Put in the Stripe keys from https://dashboard.stripe.com/test/apikeys
STRIPE_KEY=
STRIPE_SECRET=

4. 
npm install

5. php artisan serve (or pas)
Go to http://localhost:8000
and you will see a payment form (with the credit card fields loaded in a Stripe iframe, although styled to match our form)

