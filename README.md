# Flowrensic for DBOS CLI

Flowrensic runs beside your durable workflow engine and finds problems in your workflows. Flowrensic for DBOS reads the system database of DBOS and finds failed, stuck, dead letter and timed out workflows, queues that fall behind, and steps that keep retrying.

This is the command line client, dbos-flowrensic, for your CI. It asks a Flowrensic for DBOS server how it is.

Each release puts the binaries here, for Linux amd64, Linux arm64 and macOS arm64, with checksums.txt. This repo is written by the release and is not edited by hand.

Quickstart: https://dbos.flowrensic.com/docs/quickstart/

## Install

For Linux on arm64 or a Mac, change linux-amd64 to linux-arm64 or darwin-arm64:

    curl -fsSL -o dbos-flowrensic https://github.com/flowrensic/dbos-flowrensic-cli/releases/latest/download/dbos-flowrensic-linux-amd64
    chmod +x dbos-flowrensic

Check the binary against checksums.txt on the same release page.

## Use

    ./dbos-flowrensic status http://localhost:8080

It prints the health, the version and the number of findings of the server, and ends with 1 when the server is not healthy. Without a URL it asks http://localhost:8080.

    ./dbos-flowrensic version

prints the version of the CLI.

## Learn more

- Quickstart: https://dbos.flowrensic.com/docs/quickstart/

## License

Apache-2.0. See LICENSE.
