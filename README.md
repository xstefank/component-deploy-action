# EAP component deploy action

This action is intended for the continuous builds and deployments of the EAP components so they can be continously 
pulled and tested with the continuous builds of JBoss EAP.

## Inputs

### `token`

**Required** The secret passphrase used to verify taht the project is allowed deploy to the testing EAP nexus repository.

## Example usage

```
uses: xstefank/eap-component-deploy-action@v1
with:
    token: ${{ secrets.EAP_NEXUS_SECRET_PASSPHRASE }}
```
