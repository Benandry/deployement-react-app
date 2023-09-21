[![view on npm](https://badgen.net/npm/v/command-line-args)](https://www.npmjs.org/package/command-line-args)
[![js-standard-style](https://img.shields.io/badge/code%20style-standard-brightgreen.svg)](#)

# Note for all configuration :+1::+1:

![Screenshot of a comment on a GitHub issue showing an image, added in the Markdown, of an Octocat smiling and raising a tentacle.](https://myoctocat.com/assets/images/base-octocat.svg)

## Deployement d'un application react sur github

### Etape1 :

- Créer un repository.

### Etape2 :

- #### Configuration de repository

  ```
  git init
  ```

  ```
  git add .
  ```

  ```
  git commit -m "first commit
  ```

  ```
  git branch -M main
  ```

  ```
  git remote add origin https://github.com/<username>/<rep Name>.git
  ```

  ```
  git push -u origin main
  ```

### Etape3 :

- #### Installer le paquet de dependance de pages

  ```
  npm install gh-pages --save-dev
  ```

### Etape 4 : Mettre le homepage sur le package.json

```
"homepage": "https://<Username>.github.io/<Repository-name>"
```

### Etape5 :Mettre le script de deployement sur package.json

    ```js
    "scripts":{
    "predeploy": "npm run build",
    "deploy": "gh-pages -d build"
    }
    ```

### Etape 6: Mettre a jour le repository

    ```

    git add .

    ```

    ```

    git commit -m "commit"

    ```

    ```

    git push

    ```

### Et Etape 7 : Deployer votre application

    ```
       npm run deploy
    ```

> [!NOTE]
> Pour voir le url de votre site :Cliquer sur le parametre de votre repository et ensuite sur le pages

## Deployement d'un application react sur netlify

### Etape 1 : Installer un projet react

```
npx create-react-app nom_app --template typescript

```

### Etape 2 : Installer le paquet de dependance de netlify.

```

npm install netlify-cli --save-dev

```

```

npm install netlify-cli -g

```

### Etape 3 : Builder votre application

```

npm run build

```

### Etape 4 : Deployer preprod

```

netlify deploy

```

### Etape 5 : Deployer officiellement

```

netlify deploy --prod

```
