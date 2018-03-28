# Vectordash

For the github repository visit the [vectordash-cli github](https://github.com/Vectordash/vectordash-cli).

## Introduction

Welcome to [Vectordash](https://vectordash.com/)! Here you'll find comprehensive information for training and deploying your deep learning and AI applications with our platform. We do our best to make this documentation clear and user friendly, but if you have unanswered questions, please visit the community forum or contact us.

The fastest way to get up and running is to use our quickstart guide, which walks through an entire FloydHub training job step-by-step. You'll create a new Project on the FloydHub web dashboard, connect it to a local directory on your computer, and then kick-off a job using the FloydHub CLI to train your deep learning model on FloydHub's GPU servers.

## Commands

* `vectordash select [secret-token]` - Updates the user's secret token locally.

* `vectordash list` - Lists all machines the user is currently renting and can connect to.

* `vectordash ssh [machine-id]` - Connects to the machine via SSH command.

* `vectordash push [machine-id] [from-path] [to-path]` - Transfers files to the machine from [from-path] to [to-path] via SCP command. If [to-path] is not included, it will default to the machine's home directory.

* `vectordash pull [machine-id] [from-path] [to-path]` - Transfers files from the machine from [from-path] to [to-path] via SCP command. If [to-path] is not included, it will default to the local current directory.

## Project layout

    mkdocs.yml    # The configuration file.
    docs/
        index.md  # The documentation homepage.
        ...       # Other markdown pages, images and other files.
