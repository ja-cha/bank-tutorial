### technology stack:
 * Akka Actors
 * Akka Persistence 
 * Akka Http
 * Cats Validation
 * Cassandra

### relevant curl requests:
```curl
 curl --request POST \
      --url http://localhost:8080/bank \
      --header 'Content-Type: application/json' \
      --data '{
        "user":"Hans Zimmer", 
        "currency": "EUR", 
	    "balance": 1000.00
      }'
```

```curl
 curl --request GET \
      --url http://localhost:8080/bank/account-2ce9d302-b894-4dbd-9475-d9a3fc68c85c \
      --header 'Content-Type: application/json' \
```

```curl
 curl --request PUT \
      --url http://localhost:8080/bank/account-2ce9d302-b894-4dbd-9475-d9a3fc68c85c \
      --header 'Content-Type: application/json' \
      --cookie PHPSESSID=kj1en0m29o8oih40s84tfff615 \
      --data '{
        "user":"Jan Abt", 
        "currency": "USD", 
        "amount": -16
      }'
```
