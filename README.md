# GENREVAN SCHEDULER
[![Build Status](https://travis-ci.org/go-squads/genrevan-scheduler.svg?branch=master)](https://travis-ci.org/go-squads/genrevan-scheduler)
[![Go Report Card](https://goreportcard.com/badge/github.com/go-squads/genrevan-scheduler)](https://goreportcard.com/report/github.com/go-squads/genrevan-scheduler)

Genrevan Scheduler is an open source project to allocate new container efficiently based on load from LXD worker.
This scheduler use worker's metrics like CPU and memory usage to decide which LXD available to create new container.

## Limitation
- Cannot decide which LXD worker will allocate by disk usage.

## Depedencies
- Gorilla Mux
- Testify
- Postgresql

## Build
``` go install genrevan-scheduler ```

## Run
``` genrevan-scheduler ```

## Test
``` go test -v ```
