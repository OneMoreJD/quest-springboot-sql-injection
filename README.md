# BankZecure Web Application

All the instructions are in the quest!

The fake customer accounts' credentials are listed [here](https://github.com/WildCodeSchool/quest-springboot-sql-injection/blob/master/FakeAccountsCredentials.md).

## Update vulnerability

As the identifier is used to select the customer to update, we can use postman and send the request below.
So, we can change the email and the password of an unknown customer and access to his account

POST /customers/update?identifier=' or id>1; -- '&email=autre@mail.com&password=0000