# first-workflow
This is a simple workflow that demonstrates the structire of the workflow <br>

```
name: firstWorkflow
on: workflow_dispatch
jobs:
  firstjob:
    runs-on: windows-latest
    steps:
      - name: print greeting
        run: echo "Hello world!"
      - name: print goodbye
        run: echo "Done - Good bye!"

```

Repositories can have one or more workflows, Workflows contains one or more jobs, jobs contains steps that executes in a sequence of certain task.

## Events
```
on: workflow_dispatch
```
workflow_dispatch is a event that has to be triggered manually.

```
    runs-on: windows-latest
```
this line indicates that the job ```firstjob``` runs on the windows-latest machine.
