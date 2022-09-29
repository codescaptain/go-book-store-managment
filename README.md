# go-book-store-managment
With MySQl (grom) and Mux 

curl --location --request GET 'http://localhost:9010/book/'

#--##

curl --location --request POST 'http://localhost:9010/book/' \
--header 'Content-Type: application/json' \
--data-raw '{
    "Name": "Deneme Kitap İsmş",
    "Author": "Ahmet",
    "Publication": "Ahmet Yayinlari"
}'

#--##

curl --location --request PUT 'http://localhost:9010/book/1' \
--header 'Content-Type: application/json' \
--data-raw ' {
        "name": "zero to one 1",
        "author": "zero to one 1",
        "publication": "zero to one 1"
    }'

#--##

curl --location --request DELETE 'http://localhost:9010/book/1' \
--data-raw ''

#--##

curl --location --request GET 'http://localhost:9010/book/1'
