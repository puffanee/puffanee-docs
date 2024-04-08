# Status App API | Puffanee Public API (PAPI)
## APPS
- **Web app**
- **Require** Puffanee Accesss Key

### GET Requests
- **Access key** is required for GET request
- **APP ID** is required for GET request

- ***Example ALL Get Request***;
```
/all/app/
-------------------------
?pf_access=ACCESS_KEY
```

- ***Example Get Request***;
```
/app/
-------------------------
?pf_access=ACCESS_KEY
?appId=GET_APP_ID
```
### POST Requests
- **Access key** is required for POST request

- ***Example Post Request***;
```
{
    pf_access: ACCESS_KEY,
    appData: APP_JSON_DATA
}
```
- ***Example App Data***;
```
{
    title: APP_TITLE,
    type: APP_DATA_TYEPE (0: Website or 1: IP:PORT),

    url: IF TYPE 0 REQUIRED VALID WEBSITE URL,

    host: IF TYPE 1 REQUIRED VALID IP ADRESS,
    port: IF TYPE 1 REQUIRED VALID PORT NUMBER,
}
```