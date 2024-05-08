# Cloudflare Automation with Pulumi

This project is designed to automate various tasks related to Cloudflare accounts, zones, and services using Pulumi.

## Dependency Management

This project uses [Poetry](https://python-poetry.org/) for dependency management. To install dependencies, you need to have Poetry installed. If you don't have it, you can install it by following the instructions on the [Poetry website](https://python-poetry.org/docs/#installation).

Once you have Poetry installed, you can install the project dependencies with:

```bash
poetry install
```
This will install all the necessary dependencies as specified in the pyproject.toml file.

## Project Structure

The project is structured as follows:

```
.
├── src
│   └── modules
│       ├── account
│       └── zones
├── tests
│   └── unit
├── automation
├── .gitignore
└── README.md
```

- `src/modules`: This directory contains the main code for the project. It is divided into subdirectories for each account, zone, and service.
- `tests/unit`: This directory contains unit tests for the code in the `src/modules` directory. It mirrors the structure of the `src/modules` directory.
- `automation`: This directory contains scripts and other files related to automation of tasks such as building, testing, and deploying the project.

## Setup

1. Clone the repository: `git clone https://github.com/d-saurabh/cloudflare-automation.git`
2. Navigate to the project directory: `cd cloudflare-automation`
3. Install the required packages: `pip install -r requirements.txt`
4. Install Pulumi: `brew install pulumi`
5. Login to Pulumi: `pulumi login`
6. Initialize Pulumi project: `pulumi new cloudflare-python`

## Usage

Run the Pulumi up command to preview and deploy changes: `pulumi up`

## Testing

Run the tests: `python -m unittest discover tests`

## Contributing


## License

`none`