# fail

**INTERNAL USE ONLY:** This GitHub action is not intended for general use.  The only reason 
why this repo is public is because GitHub requires it.

Fails the workflow based on an input value.  This is useful when a workflow step outcome is
successful but it returns an outout indicating an error.

## Examples

**Fail the worflow:**
```
- id: fail
  runs: nforgeio-actions/test@master
  with:
    fail: true
```

**Fail with a custom message:**
```
- id: fail
  runs: nforgeio-actions/test@master
  with:
    fail: true
    message: "Something really BAD happened!"
```
