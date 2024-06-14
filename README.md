# olas_agent_enclave
This is a demo to show how to build the enclave image of an agent created with the Open AEA framework. This enclave image can be run in a Marlin Oyster Trusted Execution Environments (TEE) instance.

## Build the Enclave Builder image
`docker build -t enclave .`

## Run the docker container
```
docker run -it --privileged -v `pwd`:/app/mount enclave
```

This will generate the enclave image `.eif` file in the `/enclave` folder.

## The agent we run in this demo
https://open-aea.docs.autonolas.tech/http-echo-demo/
