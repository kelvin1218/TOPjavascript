Variable naming

There are two limitations on variable names in JavaScript:

    The name must contain only letters, digits, or the symbols $ and _.
    The first character must not be a digit.


Case matters

Variables named apple and APPLE are two different variables.

To declare a constant (unchanging) variable, use const instead of let:

const myBirthday = '18.04.1982';

Variables declared using const are called “constants”. They cannot be reassigned. An attempt to do so would cause an error

There is a widespread practice to use constants as aliases for difficult-to-remember values that are known before execution.

Such constants are named using capital letters and underscores.

For instance, let’s make constants for colors in so-called “web” (hexadecimal) format:

const COLOR_RED = "#F00";
const COLOR_GREEN = "#0F0";
const COLOR_BLUE = "#00F";
const COLOR_ORANGE = "#FF7F00";

// ...when we need to pick a color
let color = COLOR_ORANGE;
alert(color); // #FF7F00

Benefits:

    COLOR_ORANGE is much easier to remember than "#FF7F00".
    It is much easier to mistype "#FF7F00" than COLOR_ORANGE.
    When reading the code, COLOR_ORANGE is much more meaningful than #FF7F00.


**In other words, capital-named constants are only used as aliases for “hard-coded” values.**