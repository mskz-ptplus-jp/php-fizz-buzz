# PHP Fizz Buzz

PHP CI on GitHub Actions

- phpstan
- phpunit
- e2e


## Docker

```
git clone git@github.com:mskz-ptplus-jp/docker-php83.git php-fizz-puzz
```

Next step) [Provisioning](https://github.com/mskz-ptplus-jp/docker-php83?tab=readme-ov-file#provisioning)

### Run
```
docker compose up -d
```

#### Run commands in terminal of app container

```
compose install
npm install
npx playwright install
```

##### Git

```
git config --local user.email <Your email>
git config --local user.name "<Your name>"
```

merge is --no-ff

```
git config --add merge.ff false
git config --add pull.ff only
```

Register SSH public key with GitHub

```
ssh-keygen -t ed25519 -f ~/.ssh/id_ed25519 -C www-data@php-fizz-buzz -N ""
xsel -bi < ~/.ssh/id_ed25519.pub    # Paste to clipboard
```

[Add new SSH key](https://github.com/settings/ssh/new) to GitHub


### Stop

```
docker compose down
```

### Remove

```
docker compose down --rmi all --volumes
```
