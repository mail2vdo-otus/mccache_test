Реализован LRU кэш с memcached. в values.yaml memcached.mode = 0 - кэш не используется.  memcached.expiration - время жизни значения в кэше в секундах.

Все методы GET  запросов сделаны с задержкой на 1 секунду, которая проявляется в случае   отсутствия значения в кэше или при memcached.mode = 0 

