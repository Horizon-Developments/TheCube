# unfinished project.

# The Cube
A small TypeScript utility to start and manage a Bedrock Dedicated Server.
## What's the point?

If your host doesn't support Bedrock (common on free hosts), you can use this utility instead.

## what are the available JS runtimes?

### Node.js
```bashnode TheCube```
### Bun
```bashbun run TheCube```
### Deno
```bashdeno run --allow-all TheCube/index.js```

## Tutorial: Setting up InstallationCopy 

`TheCube.zip` and place it on your server.  Once unzipped, set your startup command depending on your JS runtime.

## Tutorial: Setting up Config

Go to the file `storage.json` in TheCube folder.change `"server_port": null,` to  `"server_port": YourServerPort,`  **warning** it must be a valid JSON. on finding the port, it'susually somewhere. maybe IP:PORT

## Tutorial: Setting up backups

for backups, use **https://blackblaze.com**sign in and make a master key.head over to `storage.json` and add this to `"accounts": [...]`
```js
["unique identifier name aka hotdog", "Key ID", "Application Key"],
```
it can hold lots of accounts.

remember to not remove the `,`

Do not delete ["END"].

Do not delete or create files on the Backblaze account unless it’s done through the console.

The account expects the Free plan (10 GB). Even if upgraded, it will still only store a maximum of 10 GB.
