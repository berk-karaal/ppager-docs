# Basic Structure

1. import
2. create an object
3. run()


~~~py
from ppager.ppager import Pager

my_text="""
Some kind of text.
ppager is mainly designed to display multiple line texts.
"""

# create a Pager object
my_pager = Pager(
    text=my_text.splitlines(),
    # other attributes (optional)
    )

# and run it
my_pager.run()
~~~

!!! info

    Pager.run() returns a code that informs you about how Pager object ended.
    You can read [Return codes documentation](./return_codes.md) for more.