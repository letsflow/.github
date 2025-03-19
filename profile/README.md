Letsflow is a **human-centric workflow automation** engine that blends automation with human decision-making, enabling dynamic interactions between people and automated steps.

```yaml
actors:
  user:
    title: The user
    properties:
      feeling: !default sad

actions:
  complete:
    title: Complete the process
    update:
      set: actors.user.feeling
      value: happy

states:
  initial:
    on: complete
    goto: (done)
```

The *scenario* models a *process* as a fine-state machine. The *actors* are persons, organizations, or systems that can participate in the process by performing *actions*. Which actions can be performed depends on the current *state* of the process. By executing an action, the process can *transition* to a different state.

---

### [Read the documentation](https://www.letsflow.io/)
