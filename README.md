# bitwarden-cli

bitwarden-cli docker image

this is based on the code in the [external-secrets documentation](https://external-secrets.io/v0.10.4/examples/bitwarden/).

both the `Dockerfile` and `entrypoint.sh` are a near-identical copy/paste.

the only change was to the `Dockerfile` to convert `BW_CLI_VERSION` from an `ENV` to an `ARG`,
so that the official upstream version can be read from the `VERISON` file for the `ARG` as well as the image tag

# tag convention

```bash
docker pull ghcr.io/dramirez-qb/bitwarden-cli:<official bitwarden cli version>
```

check [VERSION](/VERSION) to see what the actual value is.
when this doc was created it was `2024.9.0` so the full image was:

```bash
ghcr.io/dramirez-qb/bitwarden-cli:2024.9.0
```
