# npm

npm is a quick way to get started with n8n on your local machine. You must have [Node.js](https://nodejs.org/en/){:target=_blank .external-link} installed.

## Try n8n with npx

You can try n8n without installing it using npx.

From the terminal, run:

```bash
npx n8n
```

This command will download everything that is needed to start n8n. You can then access n8n and start building workflows by opening [http://localhost:5678](http://localhost:5678){:target=_blank .external-link}.

## Install globally with npm

If you want to install n8n globally, use npm:

```bash
npm install n8n -g
```

After the installation, start n8n by running:

```bash
n8n
# or
n8n start
```

!!! note "Keep in mind"
    Windows users remember to change into the `.n8n` directory of your Home folder (`~/.n8n`) before running `n8n start`.

### Next steps

Try out n8n using the [Quickstarts](/try-it-out/).

## Updating

To update your n8n instance to the latest released version, run:

```bash
npm update -g n8n
```

To install/update to a specific version of n8n use the `@` syntax to specify the desired version. For example:

```bash
npm install n8n@0.126.1
```

--8<-- "_snippets/self-hosting/installation/tunnel.md"

Start n8n with `--tunnel` by running:

```bash
n8n start --tunnel
```

## Windows troubleshooting

If you are experiencing issues running n8n on Windows, make sure your Node.js environment is correctly set up. Follow Microsoft's guide to [Install NodeJS on Windows](https://learn.microsoft.com/en-us/windows/dev-environment/javascript/nodejs-on-windows){:target=_blank .external-link}.
