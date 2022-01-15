# Return codes

Pager.run() returns a **string** that informs you about how Pager object ended. You can use that information if your project needs.

### Codes:
|         Code         | Description                                        |
| :------------------: | -------------------------------------------------- |
|         "ok"         | User quit through available commands.              |
| "keyboard_interrupt" | User pressed ctrl+c                                |
|    "curses_error"    | User exited after a curses error occured           |
|       "error"        | User exited after a error other than listed above. |


### Usage example:
~~~py
from ppager.ppager import Pager

with open("some_text.txt") as file:
    file_text = file.read().splitlines()

pager = Pager(text=file_text)

return_code = pager.run()
print("\n" + return_code + "\n")
~~~