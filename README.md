# flowrs

---

**This is an exercise in development in rust and shouldn't be viewed as a serious project.**
\_\_

flowrs is intended to be a api-integration system. It will make liberal use of existing products until the level of rust has improved.

It runs on GCP using an API gateway for routing to cloudrun containers. Loadbalancing is done by cloudflare.

Ideally, flowrs becomes a configurable container that accepts an OpenAPI v3 spec and credentials through secret manager in order to
access a variety of endpoints, servers and datastores where it will retrieve data -> parse, enrich, clone or destroy -> write or output
the result.

PoC is:
[] have tests before implementation
[] have automated deploy
[] configure datastore endpoint and storage client with env file
[] get data from s3, gcs, azure blob storage
[] read json, xml and text
[] parse and stdout
[] enrich data
[] delete old file
[] write data to s3, gcs, azure blob storage
