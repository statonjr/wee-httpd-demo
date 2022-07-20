# Introduction

This project demonstrates the use of [babashka](https://github.com/babashka/babashka) and [caxa](https://github.com/leafac/caxa) to run an HTTP server.

## Dependencies

- [NodeJS](https://nodejs.org/en/)

## Up and Running

### Install babashka locally

```
bash <(curl https://raw.githubusercontent.com/babashka/babashka/master/install) --dir .
```

### Create an executable

We'll use caxa to create the executable:

```
npx caxa --input . --output server "{{caxa}}/bb" "{{caxa}}/wee-httpd.bb"
```

If you don't have `caxa` installed, then `npx` will ask you if you want to install it.

### Run the server

```
./server
```

## Send HTTP Requests

```
http://localhost:4444/
```