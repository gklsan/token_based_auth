`https://www.pluralsight.com/guides/token-based-authentication-with-ruby-on-rails-5-api`

    User.create!(email: 'test@mail.com' , password: 'test123' , password_confirmation: 'test123')
    
    curl -H "Content-Type: application/json"  -X POST -d '{"email": "test@mail.com","password": "test123"}'  http://localhost:3000/authenticate
    
    curl -H "Authorization: TOKEN" http://localhost:3000/items
