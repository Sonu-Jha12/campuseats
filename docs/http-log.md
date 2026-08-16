# HTTP Request and Response Log

## Request 1 — GET /posts/1

### Full Request and Response

```text
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0* Host jsonplaceholder.typicode.com:443 was resolved.
* IPv6: 2606:4700:3037::ac43:a797, 2606:4700:3033::6815:3b13
* IPv4: 172.67.167.151, 104.21.59.19
*   Trying [2606:4700:3037::ac43:a797]:443...
*   Trying 172.67.167.151:443...
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0* Connected to jsonplaceholder.typicode.com (2606:4700:3037::ac43:a797) port 443
* ALPN: curl offers h2,http/1.1
} [5 bytes data]
* TLSv1.3 (OUT), TLS handshake, Client hello (1):
} [512 bytes data]
*  CAfile: /etc/ssl/certs/ca-certificates.crt
*  CApath: /etc/ssl/certs
{ [5 bytes data]
* TLSv1.3 (IN), TLS handshake, Server hello (2):
{ [122 bytes data]
* TLSv1.3 (IN), TLS handshake, Encrypted Extensions (8):
{ [19 bytes data]
* TLSv1.3 (IN), TLS handshake, Certificate (11):
{ [2490 bytes data]
* TLSv1.3 (IN), TLS handshake, CERT verify (15):
{ [79 bytes data]
* TLSv1.3 (IN), TLS handshake, Finished (20):
{ [52 bytes data]
* TLSv1.3 (OUT), TLS change cipher, Change cipher spec (1):
} [1 bytes data]
* TLSv1.3 (OUT), TLS handshake, Finished (20):
} [52 bytes data]
* SSL connection using TLSv1.3 / TLS_AES_256_GCM_SHA384 / X25519 / id-ecPublicKey
* ALPN: server accepted h2
* Server certificate:
*  subject: CN=typicode.com
*  start date: Jul 29 23:06:19 2026 GMT
*  expire date: Oct 28 00:04:44 2026 GMT
*  subjectAltName: host "jsonplaceholder.typicode.com" matched cert's "*.typicode.com"
*  issuer: C=US; O=Google Trust Services; CN=WE1
*  SSL certificate verify ok.
*   Certificate level 0: Public key type EC/prime256v1 (256/128 Bits/secBits), signed using ecdsa-with-SHA256
*   Certificate level 1: Public key type EC/prime256v1 (256/128 Bits/secBits), signed using ecdsa-with-SHA384
*   Certificate level 2: Public key type EC/secp384r1 (384/192 Bits/secBits), signed using ecdsa-with-SHA384
} [5 bytes data]
* using HTTP/2
* [HTTP/2] [1] OPENED stream for https://jsonplaceholder.typicode.com/posts/1
* [HTTP/2] [1] [:method: GET]
* [HTTP/2] [1] [:scheme: https]
* [HTTP/2] [1] [:authority: jsonplaceholder.typicode.com]
* [HTTP/2] [1] [:path: /posts/1]
* [HTTP/2] [1] [user-agent: curl/8.5.0]
* [HTTP/2] [1] [accept: */*]
} [5 bytes data]
> GET /posts/1 HTTP/2
> Host: jsonplaceholder.typicode.com
> User-Agent: curl/8.5.0
> Accept: */*
> 
  0     0    0     0    0     0      0      0 --:--:--  0:00:01 --:--:--     0{ [5 bytes data]
* TLSv1.3 (IN), TLS handshake, Newsession Ticket (4):
{ [230 bytes data]
* TLSv1.3 (IN), TLS handshake, Newsession Ticket (4):
{ [230 bytes data]
* old SSL session ID is stale, removing
{ [5 bytes data]
< HTTP/2 200 
< date: Sun, 16 Aug 2026 10:13:05 GMT
< content-type: application/json; charset=utf-8
< content-length: 292
< access-control-allow-credentials: true
< cache-control: max-age=43200
< etag: W/"124-yiKdLzqO5gfBrJFrcdJ8Yq0LGnU"
< expires: -1
< nel: {"report_to":"heroku-nel","response_headers":["Via"],"max_age":3600,"success_fraction":0.01,"failure_fraction":0.1}
< pragma: no-cache
< report-to: {"group":"heroku-nel","endpoints":[{"url":"https://nel.heroku.com/reports?s=PD3aZ5JXmnXLLbuM9yuy2jwg6ke8U5C2Yq%2BT0erzkj0%3D\u0026sid=e11707d5-02a7-43ef-b45e-2cf4d2036f7d\u0026ts=1775729378"}],"max_age":3600}
< reporting-endpoints: heroku-nel="https://nel.heroku.com/reports?s=PD3aZ5JXmnXLLbuM9yuy2jwg6ke8U5C2Yq%2BT0erzkj0%3D&sid=e11707d5-02a7-43ef-b45e-2cf4d2036f7d&ts=1775729378"
< server: cloudflare
< vary: Origin, Accept-Encoding
< via: 2.0 heroku-router
< x-content-type-options: nosniff
< x-powered-by: Express
< x-ratelimit-limit: 1000
< x-ratelimit-remaining: 730
< x-ratelimit-reset: 1775729393
< age: 6466
< accept-ranges: bytes
< cf-cache-status: HIT
< cf-ray: a2bfaa145b9dfdb0-SIN
< alt-svc: h3=":443"; ma=86400
< 
{ [292 bytes data]
100   292  100   292    0     0    166      0  0:00:01  0:00:01 --:--:--   166
* Connection #0 to host jsonplaceholder.typicode.com left intact
{
  "userId": 1,
  "id": 1,
  "title": "sunt aut facere repellat provident occaecati excepturi optio reprehenderit",
  "body": "quia et suscipit\nsuscipit recusandae consequuntur expedita et cum\nreprehenderit molestiae ut ut quas totam\nnostrum rerum est autem sunt rem eveniet architecto"
}```

**Status:** 200 OK — The request was successfully processed.

**Content-Type:** application/json; charset=utf-8 — The response contains JSON data.

---

## Request 2 — GET /posts/2

### Full Request and Response

```text
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0* Host jsonplaceholder.typicode.com:443 was resolved.
* IPv6: 2606:4700:3033::6815:3b13, 2606:4700:3037::ac43:a797
* IPv4: 104.21.59.19, 172.67.167.151
*   Trying [2606:4700:3033::6815:3b13]:443...
*   Trying 104.21.59.19:443...
* Connected to jsonplaceholder.typicode.com (2606:4700:3033::6815:3b13) port 443
* ALPN: curl offers h2,http/1.1
} [5 bytes data]
* TLSv1.3 (OUT), TLS handshake, Client hello (1):
} [512 bytes data]
*  CAfile: /etc/ssl/certs/ca-certificates.crt
*  CApath: /etc/ssl/certs
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0  0     0    0     0    0     0      0      0 --:--:--  0:00:01 --:--:--     0{ [5 bytes data]
* TLSv1.3 (IN), TLS handshake, Server hello (2):
{ [122 bytes data]
* TLSv1.3 (IN), TLS handshake, Encrypted Extensions (8):
{ [19 bytes data]
* TLSv1.3 (IN), TLS handshake, Certificate (11):
{ [2490 bytes data]
* TLSv1.3 (IN), TLS handshake, CERT verify (15):
{ [80 bytes data]
* TLSv1.3 (IN), TLS handshake, Finished (20):
{ [52 bytes data]
* TLSv1.3 (OUT), TLS change cipher, Change cipher spec (1):
} [1 bytes data]
* TLSv1.3 (OUT), TLS handshake, Finished (20):
} [52 bytes data]
* SSL connection using TLSv1.3 / TLS_AES_256_GCM_SHA384 / X25519 / id-ecPublicKey
* ALPN: server accepted h2
* Server certificate:
*  subject: CN=typicode.com
*  start date: Jul 29 23:06:19 2026 GMT
*  expire date: Oct 28 00:04:44 2026 GMT
*  subjectAltName: host "jsonplaceholder.typicode.com" matched cert's "*.typicode.com"
*  issuer: C=US; O=Google Trust Services; CN=WE1
*  SSL certificate verify ok.
*   Certificate level 0: Public key type EC/prime256v1 (256/128 Bits/secBits), signed using ecdsa-with-SHA256
*   Certificate level 1: Public key type EC/prime256v1 (256/128 Bits/secBits), signed using ecdsa-with-SHA384
*   Certificate level 2: Public key type EC/secp384r1 (384/192 Bits/secBits), signed using ecdsa-with-SHA384
} [5 bytes data]
* using HTTP/2
* [HTTP/2] [1] OPENED stream for https://jsonplaceholder.typicode.com/posts/2
* [HTTP/2] [1] [:method: GET]
* [HTTP/2] [1] [:scheme: https]
* [HTTP/2] [1] [:authority: jsonplaceholder.typicode.com]
* [HTTP/2] [1] [:path: /posts/2]
* [HTTP/2] [1] [user-agent: curl/8.5.0]
* [HTTP/2] [1] [accept: */*]
} [5 bytes data]
> GET /posts/2 HTTP/2
> Host: jsonplaceholder.typicode.com
> User-Agent: curl/8.5.0
> Accept: */*
> 
{ [5 bytes data]
* TLSv1.3 (IN), TLS handshake, Newsession Ticket (4):
{ [230 bytes data]
* TLSv1.3 (IN), TLS handshake, Newsession Ticket (4):
{ [230 bytes data]
* old SSL session ID is stale, removing
{ [5 bytes data]
< HTTP/2 200 
< date: Sun, 16 Aug 2026 10:13:44 GMT
< content-type: application/json; charset=utf-8
< content-length: 278
< access-control-allow-credentials: true
< cache-control: max-age=43200
< etag: W/"116-jnDuMpjju89+9j7e0BqkdFsVRjs"
< expires: -1
< nel: {"report_to":"heroku-nel","response_headers":["Via"],"max_age":3600,"success_fraction":0.01,"failure_fraction":0.1}
< pragma: no-cache
< report-to: {"group":"heroku-nel","endpoints":[{"url":"https://nel.heroku.com/reports?s=OEU8njcEseoc%2BWQeH%2FjCu8NTvmnyUb3trHBNEFU0v8Q%3D\u0026sid=e11707d5-02a7-43ef-b45e-2cf4d2036f7d\u0026ts=1786302470"}],"max_age":3600}
< reporting-endpoints: heroku-nel="https://nel.heroku.com/reports?s=OEU8njcEseoc%2BWQeH%2FjCu8NTvmnyUb3trHBNEFU0v8Q%3D&sid=e11707d5-02a7-43ef-b45e-2cf4d2036f7d&ts=1786302470"
< server: cloudflare
< vary: Origin, Accept-Encoding
< via: 2.0 heroku-router
< x-content-type-options: nosniff
< x-powered-by: Express
< x-ratelimit-limit: 1000
< x-ratelimit-remaining: 864
< x-ratelimit-reset: 1786302475
< age: 21952
< accept-ranges: bytes
< cf-cache-status: HIT
< cf-ray: a2bfab066854dde3-AMS
< alt-svc: h3=":443"; ma=86400
< 
{ [278 bytes data]
100   278  100   278    0     0    174      0  0:00:01  0:00:01 --:--:--   174
* Connection #0 to host jsonplaceholder.typicode.com left intact
{
  "userId": 1,
  "id": 2,
  "title": "qui est esse",
  "body": "est rerum tempore vitae\nsequi sint nihil reprehenderit dolor beatae ea dolores neque\nfugiat blanditiis voluptate porro vel nihil molestiae ut reiciendis\nqui aperiam non debitis possimus qui neque nisi nulla"
}```

**Status:** 200 OK — The requested resource was successfully returned.

**Content-Type:** application/json; charset=utf-8 — The response contains JSON data.

---

## Request 3 — GET /users/1

### Full Request and Response

```text
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0* Host jsonplaceholder.typicode.com:443 was resolved.
* IPv6: 2606:4700:3033::6815:3b13, 2606:4700:3037::ac43:a797
* IPv4: 172.67.167.151, 104.21.59.19
*   Trying [2606:4700:3033::6815:3b13]:443...
*   Trying 172.67.167.151:443...
* Connected to jsonplaceholder.typicode.com (2606:4700:3033::6815:3b13) port 443
* ALPN: curl offers h2,http/1.1
} [5 bytes data]
* TLSv1.3 (OUT), TLS handshake, Client hello (1):
} [512 bytes data]
*  CAfile: /etc/ssl/certs/ca-certificates.crt
*  CApath: /etc/ssl/certs
{ [5 bytes data]
* TLSv1.3 (IN), TLS handshake, Server hello (2):
{ [122 bytes data]
* TLSv1.3 (IN), TLS handshake, Encrypted Extensions (8):
{ [19 bytes data]
* TLSv1.3 (IN), TLS handshake, Certificate (11):
{ [2490 bytes data]
* TLSv1.3 (IN), TLS handshake, CERT verify (15):
{ [80 bytes data]
* TLSv1.3 (IN), TLS handshake, Finished (20):
{ [52 bytes data]
* TLSv1.3 (OUT), TLS change cipher, Change cipher spec (1):
} [1 bytes data]
* TLSv1.3 (OUT), TLS handshake, Finished (20):
} [52 bytes data]
* SSL connection using TLSv1.3 / TLS_AES_256_GCM_SHA384 / X25519 / id-ecPublicKey
* ALPN: server accepted h2
* Server certificate:
*  subject: CN=typicode.com
*  start date: Jul 29 23:06:19 2026 GMT
*  expire date: Oct 28 00:04:44 2026 GMT
*  subjectAltName: host "jsonplaceholder.typicode.com" matched cert's "*.typicode.com"
*  issuer: C=US; O=Google Trust Services; CN=WE1
*  SSL certificate verify ok.
*   Certificate level 0: Public key type EC/prime256v1 (256/128 Bits/secBits), signed using ecdsa-with-SHA256
*   Certificate level 1: Public key type EC/prime256v1 (256/128 Bits/secBits), signed using ecdsa-with-SHA384
*   Certificate level 2: Public key type EC/secp384r1 (384/192 Bits/secBits), signed using ecdsa-with-SHA384
} [5 bytes data]
* using HTTP/2
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0* [HTTP/2] [1] OPENED stream for https://jsonplaceholder.typicode.com/users/1
* [HTTP/2] [1] [:method: GET]
* [HTTP/2] [1] [:scheme: https]
* [HTTP/2] [1] [:authority: jsonplaceholder.typicode.com]
* [HTTP/2] [1] [:path: /users/1]
* [HTTP/2] [1] [user-agent: curl/8.5.0]
* [HTTP/2] [1] [accept: */*]
} [5 bytes data]
> GET /users/1 HTTP/2
> Host: jsonplaceholder.typicode.com
> User-Agent: curl/8.5.0
> Accept: */*
> 
{ [5 bytes data]
* TLSv1.3 (IN), TLS handshake, Newsession Ticket (4):
{ [230 bytes data]
* TLSv1.3 (IN), TLS handshake, Newsession Ticket (4):
{ [230 bytes data]
* old SSL session ID is stale, removing
{ [5 bytes data]
< HTTP/2 200 
< date: Sun, 16 Aug 2026 10:14:01 GMT
< content-type: application/json; charset=utf-8
< content-length: 509
< access-control-allow-credentials: true
< cache-control: max-age=43200
< etag: W/"1fd-+2Y3G3w049iSZtw5t1mzSnunngE"
< expires: -1
< nel: {"report_to":"heroku-nel","response_headers":["Via"],"max_age":3600,"success_fraction":0.01,"failure_fraction":0.1}
< pragma: no-cache
< report-to: {"group":"heroku-nel","endpoints":[{"url":"https://nel.heroku.com/reports?s=m23T6Tj%2BQUZnIwphHAim1ChY9yjwiqMeEy5yHiMrfN0%3D\u0026sid=e11707d5-02a7-43ef-b45e-2cf4d2036f7d\u0026ts=1785634999"}],"max_age":3600}
< reporting-endpoints: heroku-nel="https://nel.heroku.com/reports?s=m23T6Tj%2BQUZnIwphHAim1ChY9yjwiqMeEy5yHiMrfN0%3D&sid=e11707d5-02a7-43ef-b45e-2cf4d2036f7d&ts=1785634999"
< server: cloudflare
< vary: Origin, Accept-Encoding
< via: 2.0 heroku-router
< x-content-type-options: nosniff
< x-powered-by: Express
< x-ratelimit-limit: 1000
< x-ratelimit-remaining: 999
< x-ratelimit-reset: 1785635057
< age: 22919
< accept-ranges: bytes
< cf-cache-status: HIT
< cf-ray: a2bfab71cb529d5d-AMS
< alt-svc: h3=":443"; ma=86400
< 
{ [509 bytes data]
100   509  100   509    0     0    455      0  0:00:01  0:00:01 --:--:--   456
* Connection #0 to host jsonplaceholder.typicode.com left intact
{
  "id": 1,
  "name": "Leanne Graham",
  "username": "Bret",
  "email": "Sincere@april.biz",
  "address": {
    "street": "Kulas Light",
    "suite": "Apt. 556",
    "city": "Gwenborough",
    "zipcode": "92998-3874",
    "geo": {
      "lat": "-37.3159",
      "lng": "81.1496"
    }
  },
  "phone": "1-770-736-8031 x56442",
  "website": "hildegard.org",
  "company": {
    "name": "Romaguera-Crona",
    "catchPhrase": "Multi-layered client-server neural-net",
    "bs": "harness real-time e-markets"
  }
}```

**Status:** 200 OK — The request was successful.

**Content-Type:** application/json; charset=utf-8 — The response is JSON data.

---

## Request 4 — GET /comments/1

### Full Request and Response

```text
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0* Host jsonplaceholder.typicode.com:443 was resolved.
* IPv6: 2606:4700:3033::6815:3b13, 2606:4700:3037::ac43:a797
* IPv4: 104.21.59.19, 172.67.167.151
*   Trying [2606:4700:3033::6815:3b13]:443...
*   Trying 104.21.59.19:443...
* Connected to jsonplaceholder.typicode.com (2606:4700:3033::6815:3b13) port 443
* ALPN: curl offers h2,http/1.1
} [5 bytes data]
* TLSv1.3 (OUT), TLS handshake, Client hello (1):
} [512 bytes data]
*  CAfile: /etc/ssl/certs/ca-certificates.crt
*  CApath: /etc/ssl/certs
{ [5 bytes data]
* TLSv1.3 (IN), TLS handshake, Server hello (2):
{ [122 bytes data]
* TLSv1.3 (IN), TLS handshake, Encrypted Extensions (8):
{ [19 bytes data]
* TLSv1.3 (IN), TLS handshake, Certificate (11):
{ [2490 bytes data]
* TLSv1.3 (IN), TLS handshake, CERT verify (15):
{ [80 bytes data]
* TLSv1.3 (IN), TLS handshake, Finished (20):
{ [52 bytes data]
* TLSv1.3 (OUT), TLS change cipher, Change cipher spec (1):
} [1 bytes data]
* TLSv1.3 (OUT), TLS handshake, Finished (20):
} [52 bytes data]
* SSL connection using TLSv1.3 / TLS_AES_256_GCM_SHA384 / X25519 / id-ecPublicKey
* ALPN: server accepted h2
* Server certificate:
*  subject: CN=typicode.com
*  start date: Jul 29 23:06:19 2026 GMT
*  expire date: Oct 28 00:04:44 2026 GMT
*  subjectAltName: host "jsonplaceholder.typicode.com" matched cert's "*.typicode.com"
*  issuer: C=US; O=Google Trust Services; CN=WE1
*  SSL certificate verify ok.
*   Certificate level 0: Public key type EC/prime256v1 (256/128 Bits/secBits), signed using ecdsa-with-SHA256
*   Certificate level 1: Public key type EC/prime256v1 (256/128 Bits/secBits), signed using ecdsa-with-SHA384
*   Certificate level 2: Public key type EC/secp384r1 (384/192 Bits/secBits), signed using ecdsa-with-SHA384
} [5 bytes data]
* using HTTP/2
* [HTTP/2] [1] OPENED stream for https://jsonplaceholder.typicode.com/comments/1
* [HTTP/2] [1] [:method: GET]
* [HTTP/2] [1] [:scheme: https]
* [HTTP/2] [1] [:authority: jsonplaceholder.typicode.com]
* [HTTP/2] [1] [:path: /comments/1]
* [HTTP/2] [1] [user-agent: curl/8.5.0]
* [HTTP/2] [1] [accept: */*]
} [5 bytes data]
> GET /comments/1 HTTP/2
> Host: jsonplaceholder.typicode.com
> User-Agent: curl/8.5.0
> Accept: */*
> 
{ [5 bytes data]
* TLSv1.3 (IN), TLS handshake, Newsession Ticket (4):
{ [230 bytes data]
* TLSv1.3 (IN), TLS handshake, Newsession Ticket (4):
{ [230 bytes data]
* old SSL session ID is stale, removing
{ [5 bytes data]
< HTTP/2 200 
< date: Sun, 16 Aug 2026 10:14:17 GMT
< content-type: application/json; charset=utf-8
< content-length: 268
< access-control-allow-credentials: true
< cache-control: max-age=43200
< etag: W/"10c-KJ4I9RM/+33TKdV8CFsIvqsDSP0"
< expires: -1
< nel: {"report_to":"heroku-nel","response_headers":["Via"],"max_age":3600,"success_fraction":0.01,"failure_fraction":0.1}
< pragma: no-cache
< report-to: {"group":"heroku-nel","endpoints":[{"url":"https://nel.heroku.com/reports?s=C4h1dyT15nRwK%2F71KPxt4SaGNEn%2FaIGnlUSl%2Fzx9%2FNY%3D\u0026sid=e11707d5-02a7-43ef-b45e-2cf4d2036f7d\u0026ts=1785740413"}],"max_age":3600}
< reporting-endpoints: heroku-nel="https://nel.heroku.com/reports?s=C4h1dyT15nRwK%2F71KPxt4SaGNEn%2FaIGnlUSl%2Fzx9%2FNY%3D&sid=e11707d5-02a7-43ef-b45e-2cf4d2036f7d&ts=1785740413"
< server: cloudflare
< vary: Origin, Accept-Encoding
< via: 2.0 heroku-router
< x-content-type-options: nosniff
< x-powered-by: Express
< x-ratelimit-limit: 1000
< x-ratelimit-remaining: 919
< x-ratelimit-reset: 1785740416
< age: 8028
< accept-ranges: bytes
< cf-cache-status: HIT
< cf-ray: a2bfabd488fded05-AMS
< alt-svc: h3=":443"; ma=86400
< 
{ [268 bytes data]
100   268  100   268    0     0    186      0  0:00:01  0:00:01 --:--:--   186100   268  100   268    0     0    186      0  0:00:01  0:00:01 --:--:--   186
* Connection #0 to host jsonplaceholder.typicode.com left intact
{
  "postId": 1,
  "id": 1,
  "name": "id labore ex et quam laborum",
  "email": "Eliseo@gardner.biz",
  "body": "laudantium enim quasi est quidem magnam voluptate ipsam eos\ntempora quo necessitatibus\ndolor quam autem quasi\nreiciendis et nam sapiente accusantium"
}```

**Status:** 200 OK — The request was successfully processed.

**Content-Type:** application/json; charset=utf-8 — The response is JSON data.

---

## Request 5 — GET /posts/999999

### Full Request and Response

```text
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0* Host jsonplaceholder.typicode.com:443 was resolved.
* IPv6: 2606:4700:3033::6815:3b13, 2606:4700:3037::ac43:a797
* IPv4: 104.21.59.19, 172.67.167.151
*   Trying [2606:4700:3033::6815:3b13]:443...
*   Trying 104.21.59.19:443...
* Connected to jsonplaceholder.typicode.com (2606:4700:3033::6815:3b13) port 443
* ALPN: curl offers h2,http/1.1
} [5 bytes data]
* TLSv1.3 (OUT), TLS handshake, Client hello (1):
} [512 bytes data]
*  CAfile: /etc/ssl/certs/ca-certificates.crt
*  CApath: /etc/ssl/certs
{ [5 bytes data]
* TLSv1.3 (IN), TLS handshake, Server hello (2):
{ [122 bytes data]
* TLSv1.3 (IN), TLS handshake, Encrypted Extensions (8):
{ [19 bytes data]
* TLSv1.3 (IN), TLS handshake, Certificate (11):
{ [2490 bytes data]
* TLSv1.3 (IN), TLS handshake, CERT verify (15):
{ [79 bytes data]
* TLSv1.3 (IN), TLS handshake, Finished (20):
{ [52 bytes data]
* TLSv1.3 (OUT), TLS change cipher, Change cipher spec (1):
} [1 bytes data]
* TLSv1.3 (OUT), TLS handshake, Finished (20):
} [52 bytes data]
* SSL connection using TLSv1.3 / TLS_AES_256_GCM_SHA384 / X25519 / id-ecPublicKey
* ALPN: server accepted h2
* Server certificate:
*  subject: CN=typicode.com
*  start date: Jul 29 23:06:19 2026 GMT
*  expire date: Oct 28 00:04:44 2026 GMT
*  subjectAltName: host "jsonplaceholder.typicode.com" matched cert's "*.typicode.com"
*  issuer: C=US; O=Google Trust Services; CN=WE1
*  SSL certificate verify ok.
*   Certificate level 0: Public key type EC/prime256v1 (256/128 Bits/secBits), signed using ecdsa-with-SHA256
*   Certificate level 1: Public key type EC/prime256v1 (256/128 Bits/secBits), signed using ecdsa-with-SHA384
*   Certificate level 2: Public key type EC/secp384r1 (384/192 Bits/secBits), signed using ecdsa-with-SHA384
} [5 bytes data]
* using HTTP/2
* [HTTP/2] [1] OPENED stream for https://jsonplaceholder.typicode.com/posts/999999
* [HTTP/2] [1] [:method: GET]
* [HTTP/2] [1] [:scheme: https]
* [HTTP/2] [1] [:authority: jsonplaceholder.typicode.com]
* [HTTP/2] [1] [:path: /posts/999999]
* [HTTP/2] [1] [user-agent: curl/8.5.0]
* [HTTP/2] [1] [accept: */*]
} [5 bytes data]
> GET /posts/999999 HTTP/2
> Host: jsonplaceholder.typicode.com
> User-Agent: curl/8.5.0
> Accept: */*
> 
{ [5 bytes data]
* TLSv1.3 (IN), TLS handshake, Newsession Ticket (4):
{ [230 bytes data]
* TLSv1.3 (IN), TLS handshake, Newsession Ticket (4):
{ [230 bytes data]
* old SSL session ID is stale, removing
{ [5 bytes data]
< HTTP/2 404 
< date: Sun, 16 Aug 2026 10:14:33 GMT
< content-type: application/json; charset=utf-8
< content-length: 2
< access-control-allow-credentials: true
< cache-control: max-age=43200
< etag: W/"2-vyGp6PvFo4RvsFtPoIWeCReyIC8"
< expires: -1
< nel: {"report_to":"heroku-nel","response_headers":["Via"],"max_age":3600,"success_fraction":0.01,"failure_fraction":0.1}
< pragma: no-cache
< report-to: {"group":"heroku-nel","endpoints":[{"url":"https://nel.heroku.com/reports?s=bsGcMpOT7bW8ebun8Da5jTxfGjq6%2Fm0dB85K7xGxOnc%3D\u0026sid=e11707d5-02a7-43ef-b45e-2cf4d2036f7d\u0026ts=1786856720"}],"max_age":3600}
< reporting-endpoints: heroku-nel="https://nel.heroku.com/reports?s=bsGcMpOT7bW8ebun8Da5jTxfGjq6%2Fm0dB85K7xGxOnc%3D&sid=e11707d5-02a7-43ef-b45e-2cf4d2036f7d&ts=1786856720"
< server: cloudflare
< vary: Origin, Accept-Encoding
< via: 2.0 heroku-router
< x-content-type-options: nosniff
< x-powered-by: Express
< x-ratelimit-limit: 1000
< x-ratelimit-remaining: 999
< x-ratelimit-reset: 1786856742
< age: 18552
< cf-cache-status: HIT
< cf-ray: a2bfac3d6c48ae32-AMS
< alt-svc: h3=":443"; ma=86400
< 
{ [2 bytes data]
100     2  100     2    0     0      1      0  0:00:02  0:00:01  0:00:01     2100     2  100     2    0     0      1      0  0:00:02  0:00:01  0:00:01     2
* Connection #0 to host jsonplaceholder.typicode.com left intact
{}```

**Status:** 404 Not Found — The requested resource does not exist.

**Content-Type:** application/json; charset=utf-8 — The error response is returned in JSON format.
