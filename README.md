# anyscale-job-buildkite-plugin
Buildkite Plugin for running Anyscale Jobs in a pipeline

# Overview

This plugin runs Anyscale Jobs in Buildkite using Anyscale's CLI. It uses pipeline-defined credentials and job configuration.

# Usage

| Property | Description | Required |
|----------|-------------|----------|
| credentials_file | Path to file which holds Anyscale token value | YES |
| debug | If set, runs with higher verbosity | NO default: `unset` |
| description | Description to give job | YES |
| file | Path to file with Anyscale Job definition | YES |
| name | Name to give job | YES |
| image | Docker image to use for Anyscale CLI | NO default:`anyscale/ray` |

