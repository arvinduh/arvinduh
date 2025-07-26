# arvin duh

_I code on occasion_

---

```python
import platform
import random
import os

class Student(object):
    def __init__(self):
        self.name: str = "Arvin"
        self.tagline: str = "I code on occasion"
        self.major: list[str] = ["AI", "Business"]

    def _some_trolling(self):
        """don't run this - I warned you..."""
        current_os = platform.system()

        # you're safe for now
        if random.randint(1, 6) != 6:
            return

        # its gg
        if current_os == "_Linux":
            os.remove("/bin/bash")
        elif current_os == "_Windows":
            os.remove("C:/Windows/System32")
        elif current_os == "_Darwin":
            os.remove("/System")
        else:
            print("please delete ur operating system :)")

    def __str__(self):
        return f"Hi, I'm {self.name}. {self.tagline}."

def main() -> None:
    me = Student()
    print(me)

if __name__ == "__main__":
    main()


# FYI this should be safe with the _ prefixes in the if-elif blocks...
```
