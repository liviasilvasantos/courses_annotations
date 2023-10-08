## Rodar Redis no Docker

> docker run -d --name redis-stack -p 6379:6379 -p 8001:8001 redis/redis-stack:latest

## Conectar usando redis-cli

> docker exec -it redis-stack redis-cli

## Comandos

**set key value**  
adciona uma chave string "key" com valor "value"

**get key**  
recupera valor de uma chave "key"

**del key**  
remove uma chave "key"

**exists key**  
verifica se existe uma chave "key"

**keys \***  
retorna todas as chaves

**flushall**  
remove todas as chaves

**ttl key**  
mostra o ttl (time to live, em segundos) de uma chave "key"

**expire key ttl**  
determina o ttl de uma chave "key"

**setex key ttl value**  
cria uma chave "key" com ttl "ttl" e valor "value"

**lpush key item**  
adiciona o item no início de uma chave/lista

**lrange key 0 -1**  
recupera todos os itens de uma chave/lista

**rpush key item**  
adiciona o item no fim de uma chave/lista

**lpop key**  
remove o primeiro item de uma chave/lista

**rpop key**  
remove o último item de uma chave/lista

**sadd key value**  
adiciona o item no início de uma chave/set (lista com valores únicos)

**smembers key**  
mostra todos os itens de uma chave/set

**srem key value**  
remove o item de uma chave/set

**hset key field value**  
cria uma chave/hash com campo "field" e valor "value"

**hget key field**  
recupera o campo de uma chave/hash

**hgetall key**  
recupera todos os campos e valores de uma chave/hash

**hexists key field**  
verifica se existe um campo na chave/hash


