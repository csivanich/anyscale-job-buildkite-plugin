# Example

Ported from [Submit your first Anyscale Job](https://docs.anyscale.com/productionize/jobs/get-started#submit-your-first-anyscale-job)

This runs a 'hello world' Ray application using your default cloud, cluster environment, and compute environment.

It first uses the `seek-oss/aws-sm` plugin to read the Anyscale CLI Token into a file. This file is then passed to the `anyscale-job` plugin via the `credentials_file` property.

The `job.yaml` file is then uploaded using the credentials in the file, and the job is started.

## Requirements

- An AWS Secrets Manager secret `anyscale_cli_token` whose contents are a working Anyscale Token.
- A Buildkite Agent Queue which can read `anyscale_cli_token` from AWS Secrets Manager.

