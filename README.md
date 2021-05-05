# Component deploy action

This action is intended for the continuous builds and deployments of the components so they can be continously 
pulled and tested with the continuous parent builds.

## Inputs

### `token`

**Required** The secret passphrase used to verify taht the project is allowed deploy to the testing nexus repository.

## Example usage

```
uses: xstefank/component-deploy-action@v1
with:
    token: ${{ secrets.NEXUS_SECRET_PASSPHRASE }}
```
