# Architecture

```text
                    Hermes Agent
                         |
                         v
                Successful task run
                         |
                         v
                  Modiqo Rote
             records the working path
                         |
                         v
                  Released Play
                         |
                         v
                 Public Registry
                  /            \
                 v              v
      npm-package-report   service-health-report
             |                    |
             v                    v
       package=input        service=input
             |                    |
             v                    v
      deterministic         deterministic
        replay                replay
```

## Design principle

The project follows the Playoffs idea of preserving a successful execution path instead of rediscovering the same workflow repeatedly.

## Play 1

Three parallel data-gathering steps:
- package metadata
- download statistics
- distribution-tag confirmation

## Play 2

A service-health procedure resolves a public status source and returns the current status and overall verdict.

Both artifacts are parameterized, versioned, released, and publicly runnable.
