# Binary Firefox New Tab Clock

A minimal **4×6 binary clock** designed to be used as a custom Firefox New Tab page.

The clock displays the current time using six columns:

```text
H H M M S S
```

Each column represents one decimal digit, while the four rows represent the binary values:

```text
8
4
2
1
```

Active bits glow softly against a dark Firefox-style background.

## Preview

```text
○ ● ○ ○ ● ○
○ ○ ● ○ ○ ●
● ○ ○ ● ○ ○
○ ○ ○ ● ● ○
```

The actual pattern changes every second as the time changes.

## Features

* 12-hour clock
* Seconds included
* 4 × 6 dot layout
* Binary representation
* Soft glowing active dots
* Dark Firefox-style background
* No text or unnecessary UI
* Automatically updates every second
* Centered slightly above the middle of the page
* Pure HTML, CSS, and JavaScript
* No dependencies

## Layout

The six columns represent:

| Column | Digit        |
| ------ | ------------ |
| 1      | Hour tens    |
| 2      | Hour units   |
| 3      | Minute tens  |
| 4      | Minute units |
| 5      | Second tens  |
| 6      | Second units |

The four rows represent:

| Row | Binary value |
| --- | -----------: |
| 1   |            8 |
| 2   |            4 |
| 3   |            2 |
| 4   |            1 |

For example, the digit `5` is:

```text
0
1
0
1
```

because:

```text
4 + 1 = 5
```

## Installation

1. Save the HTML file somewhere on your computer, for example:

```text
~/binary-clock.html
```

2. Install the Firefox extension **New Tab Override**.

3. Configure New Tab Override to use your local HTML file.

4. Open a new tab.

Your Firefox New Tab page should now display the binary clock.

## Customization

The clock can easily be customized through the CSS.

### Background

Current background:

```css
background: #2b2a33;
```

### Dot size

```css
width: 28px;
height: 28px;
```

### Spacing

```css
gap: 10px;
```

### Vertical position

The clock is currently positioned at:

```css
top: 45%;
```

Increase the value to move it down.

Decrease the value to move it up.

### Glow

Active dots use:

```css
box-shadow:
    0 0 5px #fff,
    0 0 12px rgba(255, 255, 255, 0.65),
    0 0 20px rgba(255, 255, 255, 0.3);
```

## License

Use, modify, and customize it however you want.
