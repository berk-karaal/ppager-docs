# Colors

### colors are defined in ppager as:
~~~py
curses_colors = {
    "-": -1, # Use default value which is used by terminal
    "black": curses.COLOR_BLACK,
    "blue": curses.COLOR_BLUE,
    "cyan": curses.COLOR_CYAN,
    "green": curses.COLOR_GREEN,
    "magenta": curses.COLOR_MAGENTA,
    "red": curses.COLOR_RED,
    "white": curses.COLOR_WHITE,
    "yellow": curses.COLOR_YELLOW,
}
~~~


### Usage example:
~~~py
my_pager = Pager(
    text=...,
    line_numbers_fg="black",
    line_numbers_bg="yellow",
    separator_bg="blue",
    separator_fg="white",
    overflow_indicator_bg="cyan",
    overflow_indicator_fg="red",
    end_bg="magenta",
    end_fg="green",
)
~~~

