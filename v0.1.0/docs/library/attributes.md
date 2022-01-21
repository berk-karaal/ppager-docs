## Pager Attributes
~~~py
class Pager:

    def __init__(
        self,
        text: list,
        tab_size: int = 4,
        break_lines: bool = False,
        right_padding_for_text: int = 0,
        line_numbers: bool = False,
        line_numbers_fg: str = "-",
        line_numbers_bg: str = "-",
        separator: str = "│",
        separator_fg: str = "-",
        separator_bg: str = "-",
        space_after_separator: bool = True,
        title_text: str = "",
        center_title: bool = False,
        title_fg: str = "-",
        title_bg: str = "-",
        overflow_indicator: str = ">",
        overflow_indicator_fg: str = "black",
        overflow_indicator_bg: str = "white",
        end_text: str = "(END)",
        end_text_fg: str = "black",
        end_text_bg: str = "white",
        bottom_bar_text: str = "Quit(q) Help(h)",
        bottom_bar_fg: str = "black",
        bottom_bar_bg: str = "white",
        show_cursor_y_position: bool = True,
        show_cursor_y_percentage: bool = True,
        blink: bool = False,
    ):
~~~

---

|          Attribute           | Type  |      Default      | Description                                                                                                             |
| :--------------------------: | :---: | :---------------: | ----------------------------------------------------------------------------------------------------------------------- |
|      [**text**](#text)       | list  |       None        | Gets content to display.<br>Elements of given list should represent lines of content.                                   |
|         **tab_size**         |  int  |         4         | Defines how many spaces will be for a "\t".                                                                             |
|       **break_lines**        | bool  |       False       | True if break line mode is on.                                                                                          |
|  **right_padding_for_text**  |  int  |         0         | Gives padding(empty space) to right side of terminal as much as given int.                                              |
|       **line_numbers**       | bool  |       False       | True if line numbers should be displayed on startup.<br>(User can turn on or off line numbers while program is running) |
|     **line_numbers_fg**      |  str  |        "-"        | Foreground color of line numbers.<br>[Color Values](./colors.md)                                                        |
|     **line_numbers_bg**      |  str  |        "-"        | Background color of line numbers.<br>[Color Values](./colors.md)                                                        |
|        **separator**         |  str  |        "│"        | Defines separator.                                                                                                      |
|       **separator_fg**       |  str  |        "-"        | Foreground color of separator.<br>[Color Values](./colors.md)                                                           |
|       **separator_bg**       |  str  |        "-"        | Background color of separator.<br>[Color Values](./colors.md)                                                           |
|  **space_after_separator**   | bool  |       True        | True if there should be a space between separator and text.                                                             |
|        **title_text**        |  str  |        ""         | Defines title that should be displayed.<br>Empty string(default value) means do not display any title.                  |
|       **center_title**       | bool  |       False       | True if title should be displayed horizontally centered.                                                                |
|         **title_fg**         |  str  |        "-"        | Foreground color of title.<br>[Color Values](./colors.md)                                                               |
|         **title_bg**         |  str  |        "-"        | Background color of title.<br>[Color Values](./colors.md)                                                               |
|    **overflow_indicator**    |  str  |        ">"        | Defines overflow indicator.                                                                                             |
|  **overflow_indicator_fg**   |  str  |      "black"      | Foreground color of overflow indicator.<br>[Color Values](./colors.md)                                                  |
|  **overflow_indicator_bg**   |  str  |      "white"      | Background color of overflow indicator.<br>[Color Values](./colors.md)                                                  |
|         **end_text**         |  str  |      "(END)"      | Defines end text.                                                                                                       |
|       **end_text_fg**        |  str  |      "black"      | Foreground color of end text.<br>[Color Values](./colors.md)                                                            |
|       **end_text_bg**        |  str  |      "white"      | Background color of end text.<br>[Color Values](./colors.md)                                                            |
|     **bottom_bar_text**      |  str  | "Quit(q) Help(h)" | Defines text that should be displayed in bottom bar.                                                                    |
|      **bottom_bar_fg**       |  str  |      "black"      | Foreground color of bottom bar.<br>[Color Values](./colors.md)                                                          |
|      **bottom_bar_bg**       |  str  |      "white"      | Background color of bottom bar.<br>[Color Values](./colors.md)                                                          |
|  **show_cursor_y_position**  | bool  |       True        | True if cursor y position should be displayed in bottom bar.                                                            |
| **show_cursor_y_percentage** | bool  |       True        | True if cursor y percentage should be displayed in bottom bar.                                                          |
|     [**blink**](#blink)      | bool  |       False       | True if blink mode should be activated.                                                                                 |


## Attribute Usage Tips

### text
You can convert your multiline string to a list with [.splitlines()](https://docs.python.org/3/library/stdtypes.html#str.splitlines)<br>
[Check out example][1]

### blink
It's for developmental purposes. Do not activate it for endusers.

  [1]: https://github.com/berk-karaal/ppager/blob/8a20a592b9efb73e5588937ef6d1b1e8084c9d6d/examples/1)%20hello%20world/hello_world.py