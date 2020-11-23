This is a template for a [StackHead Module](https://docs.stackhead.io/stackhead-modules/stackhead-modules).

Make sure to adjust it to your needs.

---

# StackHead: [name] module

StackHead module for [description].

## Installation

Install it via `ansible-galaxy`:

```
ansible-galaxy install [vendor].stackhead_[type]_[name]
```

In order to use [name] with [StackHead](https://get.stackhead.io), set `stackhead__[type]` it in your inventory file:

```yaml
# inventory for integration test
---
all:
  vars:
    # Use Nginx as webserver
    stackhead__[type]: [vendor].stackhead_[type]_[name]
  hosts:
    myserver:
      ansible_host: 123.456.789 # ...
      stackhead:
        applications:
          # ...
```
