# Next.js DevContainer Template Repository

To get started, follow the steps below to install the node_modules/:

```bash
cd my-app
yarn install
```

Afterwards, you can run the development server using the following command:

```bash
yarn dev
```


## Environment

| Name    | Version                |
| ------- | ---------------------- |
| Node.js | v18.16.1               |
| Yarn    | Latest (as of 23/6/21) |
| Next.js | Latest (as of 23/6/21) |

## Development Support

- Auto linting with ESLint
- Auto formatting with Prettier

## Initialization Steps

```bash
yarn create next-app
# (Answer "yes" to all prompts)
cp ./devcontainer/template/* ./my-app/
# (Copy eslint and prettier configuration files)
```

Off course, you can remove `my-app/` and init with your own way.
