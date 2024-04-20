# huston

A Bash script that enhances terminal output with colorful text. It allows you to set text and background colors using RGB values and hexadecimal codes. 

## Usage

```
huston [-h] [-r] [-g] [-b] [-H HEX | -R RED -G GREEN -B BLUE] [-c] [-p] [-w] [-y] TEXT
```

### Options

- `-h, --help`: Display the help message.
- `-r`: Set the text color to red.
- `-g`: Set the text color to green.
- `-b`: Set the text color to blue.
- `-c`: Set the text color to cyan.
- `-p`: Set the text color to pink.
- `-w`: Set the text color to white.
- `-y`: Set the text color to yellow.
- `-H HEX`: Set the text color to the specified HEX value (e.g., 'ff0000').
- `-R RED`: Set the text color using the specified RED value (0-255).
- `-G GREEN`: Set the text color using the specified GREEN value (0-255).
- `-B BLUE`: Set the text color using the specified BLUE value (0-255).

## Examples

```bash
huston -r -T 'Hello, world!'
```
Print 'Hello, world!' in red text.

```bash
huston -R 255 -T 'Hello, world!'
```
Same as above.

```bash
huston -H FF0000 -T 'Hello, world!'
```
Same as above.

```bash
echo 'Hello, world!' | huston -R 155
```
Print 'Hello, world!' in dark red text.

## Pipe Support

`huston` supports reading input from a pipe, allowing you to use it in combination with other commands.

## Project Details

- **Language**: Bash
- **Compatibility**: Linux systems only
- **Tested On**: Debian-based systems (Ubuntu 20.04.6 LTS x86_64)
  
## Dependencies
This project requires the <a href="https://github.com/AmosNimos/flag">flag</a> script for parsing command-line arguments. Make sure to have the flag script installed and accessible in your PATH.

## License

This software is released under the MIT License. See the `LICENSE` file for more details.

## Author

This software was created by Amosnimos.

---
