# Python Event

Add the Event class to your code and enjoy C#-like syntax to subscribe, unsubscribe and call events in Python

Usage:

```
def on_name_changed(value):
    print(value)

name_changed = Event()
name_changed += on_name_changed  # subscribe a function. can be unsubscribed
name_changed += lambda x: print(x)  # subscribe a lambda. cannot be unsubscribed
name_changed("Vera1")

name_changed -= on_name_changed  # unsubscribe from event
name_changed("Vera2")
```
