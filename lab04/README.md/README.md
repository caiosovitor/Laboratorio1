TAREFA 04
-----------
Encontre dois serviços REST interessantes, que recebam no mínimo dois parâmetros e execute pelo menos uma consulta em cada um deles. Apresente para cada serviço que você escolheu:

* o título do serviço
* a URI do serviço
* uma breve descrição do mesmo
* o cabeçalho HTTP da requisição
* o cabeçalho e conteúdo JSON, XML ou outro formato da resposta


Serviço 01: FireBrowse Beta
 -----------------------
* **Titulo** : Pesquisa FireBrowse
* **Descrição** : Busca por registros de Transposiçao Corrigida por Grandes Artérias TCGA (cardiopatia)
* **URL da Requisiçao** :https://any-api.com:8443/http://firebrowse.org/api/v1/Analyses/CopyNumber/Genes/Focal?format=json&cohort=SKCM&gene=UBE2Q1&tcga_participant_barcode=TCGA-GF-A4EO&sort_by=cohort



* **Cabeçalho HTTP da chamada**: 
~~~ http
:authority: any-api.com:8443
:method: GET
:path: /http://firebrowse.org/api/v1/Analyses/CopyNumber/Genes/Focal?format=json&cohort=SKCM&gene=UBE2Q1&tcga_participant_barcode=TCGA-GF-A4EO&sort_by=cohort
:scheme: https
accept: application/json
accept-encoding: gzip, deflate, br
accept-language: en-US,en;q=0.9
origin: https://any-api.com
referer: https://any-api.com/firebrowse_org/firebrowse_org/console/Analyses/Focal
sec-fetch-dest: empty
sec-fetch-mode: cors
sec-fetch-site: same-site
user-agent: Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_6) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/84.0.4147.105 Safari/537.36
~~~
* **Cabeçalho HTTP da resposta**: 
~~~ http
access-control-allow-methods: HEAD, GET
access-control-allow-origin: *
access-control-expose-headers: date,server,access-control-allow-origin,access-control-allow-methods,access-control-max-age,content-type,vary,content-encoding,content-length,connection,x-final-url
access-control-max-age: 21600
cf-cache-status: DYNAMIC
cf-ray: 5c9ad5deef4a09e0-GIG
cf-request-id: 04d4a3ff4d000009e076359200000001
content-encoding: br
content-type: application/json
date: Fri, 28 Aug 2020 03:09:47 GMT
expect-ct: max-age=604800, report-uri="https://report-uri.cloudflare.com/cdn-cgi/beacon/expect-ct"
server: cloudflare
set-cookie: __cfduid=deaeefc3f678b1aac2208512af5fd74b11598584186; expires=Sun, 27-Sep-20 03:09:46 GMT; path=/; domain=.any-api.com; HttpOnly; SameSite=Lax
status: 200
vary: Accept-Encoding
x-final-url: http://firebrowse.org/api/v1/Analyses/CopyNumber/Genes/Focal?format=json&cohort=SKCM&gene=UBE2Q1&tcga_participant_barcode=TCGA-GF-A4EO&sort_by=cohort
x-request-url: http://firebrowse.org/api/v1/Analyses/CopyNumber/Genes/Focal?format=json&cohort=SKCM&gene=UBE2Q1&tcga_participant_barcode=TCGA-GF-A4EO&sort_by=cohort
~~~
* **Conteúdo HTTP da resposta**: 

~~~ json
{
  "Focal": [
    {
      "cohort": "SKCM",
      "cytoband": "1q21.3",
      "date": "Thu, 28 Jan 2016 00:00:00 GMT",
      "focal_copy_number": 0,
      "gene": "UBE2Q1",
      "locus_id": "55585",
      "tcga_participant_barcode": "TCGA-GF-A4EO"
    }
  ]
}

~~~



 Serviço 02: GetGames
 -----------------------
* **Titulo** : Getgames Collegial Footbal
* **Descrição** : Busca por Técnico chamado Mark que atuou no ano de 2018   
* **URL da Requisiçao** : Request URL: https://any-api.com:8443/https://api.collegefootballdata.com/coaches?firstName=Mark&year=2018
* **Cabeçalho HTTP da chamada**: 
~~~ http
:authority: any-api.com:8443
:method: GET
:path: /https://api.collegefootballdata.com/coaches?firstName=Mark&year=2018
:scheme: https
accept: */*
accept-encoding: gzip, deflate, br
accept-language: en-US,en;q=0.9
if-none-match: W/"36b-hsLROB7WqJknXLkjlN5FyQkyY5E"
origin: https://any-api.com
referer: https://any-api.com/collegefootballdata_com/collegefootballdata_com/console/coaches/getCoaches
sec-fetch-dest: empty
sec-fetch-mode: cors
sec-fetch-site: same-site
user-agent: Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_6) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/84.0.4147.105 Safari/537.36
~~~
* **Cabeçalho HTTP da resposta**: 
~~~ http
access-control-allow-origin: *
access-control-expose-headers: server,date,connection,x-dns-prefetch-control,x-frame-options,strict-transport-security,x-download-options,x-content-type-options,x-xss-protection,access-control-allow-origin,etag,x-final-url
cf-cache-status: DYNAMIC
cf-ray: 5c9ab5f96c69dbac-GIG
cf-request-id: 04d4900fdd0000dbac5b171200000001
content-encoding: br
content-type: application/json; charset=utf-8
date: Fri, 28 Aug 2020 02:48:00 GMT
etag: W/"36b-hsLROB7WqJknXLkjlN5FyQkyY5E"
expect-ct: max-age=604800, report-uri="https://report-uri.cloudflare.com/cdn-cgi/beacon/expect-ct"
server: cloudflare
set-cookie: __cfduid=dde73b37d78fcd45e65e636320f46d6e01598582880; expires=Sun, 27-Sep-20 02:48:00 GMT; path=/; domain=.any-api.com; HttpOnly; SameSite=Lax
status: 304
strict-transport-security: max-age=15552000; includeSubDomains
x-content-type-options: nosniff
x-dns-prefetch-control: off
x-download-options: noopen
x-final-url: https://api.collegefootballdata.com/coaches?firstName=Mark&year=2018
x-frame-options: SAMEORIGIN
x-request-url: https://api.collegefootballdata.com/coaches?firstName=Mark&year=2018
x-xss-protection: 1; mode=block
~~~

* **Conteúdo HTTP da resposta**: 
~~~ json
[
  {
    "first_name": "Mark",
    "last_name": "Dantonio",
    "seasons": [
      {
        "school": "Michigan State",
        "year": 2018,
        "games": 13,
        "wins": 7,
        "losses": 6,
        "ties": 0,
        "preseason_rank": 11,
        "postseason_rank": null
      }
    ]
  },
  {
    "first_name": "Mark",
    "last_name": "Ivey",
    "seasons": [
      {
        "school": "Appalachian State",
        "year": 2018,
        "games": 1,
        "wins": 1,
        "losses": 0,
        "ties": 0,
        "preseason_rank": null,
        "postseason_rank": null
      }
    ]
  },
  {
    "first_name": "Mark",
    "last_name": "Richt",
    "seasons": [
      {
        "school": "Miami",
        "year": 2018,
        "games": 13,
        "wins": 7,
        "losses": 6,
        "ties": 0,
        "preseason_rank": 8,
        "postseason_rank": null
      }
    ]
  },
  {
    "first_name": "Mark",
    "last_name": "Stoops",
    "seasons": [
      {
        "school": "Kentucky",
        "year": 2018,
        "games": 13,
        "wins": 10,
        "losses": 3,
        "ties": 0,
        "preseason_rank": null,
        "postseason_rank": null
      }
    ]
  },
  {
    "first_name": "Mark",
    "last_name": "Whipple",
    "seasons": [
      {
        "school": "UMass",
        "year": 2018,
        "games": 12,
        "wins": 4,
        "losses": 8,
        "ties": 0,
        "preseason_rank": null,
        "postseason_rank": null
      }
    ]
  }
]
~~~
