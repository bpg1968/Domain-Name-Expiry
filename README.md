# exp

`exp` is a simple shell script that reports the expiration dates of domain names using the `whois` command. It reads domain names from a file or accepts one directly via the command line and outputs formatted, colour-coded expiration information. This utility is useful for monitoring domain ownership and availability.

> **Note:** This project is produced with the help of AI, using tools such as OpenAI's ChatGPT.

## Features

- Supports reading from a file (default: `~/.domains.txt`)
- Command line options for specifying an alternate file or a single domain
- Outputs expiration dates in a readable format
- Colour-coded status:
  - **Green** — Domain is available
  - **Red** — Domain has expired
  - **Yellow/Orange** — Domain expires within 3 months
  - **White** — Domain is valid for more than 3 months
- 1 second delay between checks to respect server limits
- Graceful error handling if input file is missing

## Installation

```sh
git clone https://github.com/yourusername/exp.git
cd exp
chmod +x exp
```

## Usage

```sh
./exp                # Uses ~/.domains.txt
./exp -f mylist.txt  # Uses custom file
./exp -d example.com # Checks a single domain
./exp --version      # Displays version
./exp --help         # Shows help message
```

## Requirements

- Linux (or Unix-like environment)
- `whois`, `tput`, and standard core utilities (`date`, etc.)

## License

This project is licensed under the GNU General Public License v3.0. See `LICENSE.txt` for details.

## Contributing

This project is **largely unmaintained**. Contributions are welcome, but please note that **issues and pull requests may not receive a timely response**. 

Please see the [CONTRIBUTING.md](CONTRIBUTING.md) and [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md) for guidelines.

## Disclaimer

This script makes live `whois` queries and should be used responsibly to avoid rate limiting or abuse issues.


