# zCore Resume Builder
Uses Python to build zCore branded resumes, this project is using Poetry with `docx` as a dependency, and includes a template generator script for creating Word documents.

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites

- Python 3.6 or higher
- Poetry for dependency management

### Installing Poetry

Poetry is used for dependency management and packaging. If you haven't installed Poetry yet, follow these instructions:

#### For Unix, Linux, macOS:

```bash
curl -sSL https://install.python-poetry.org | python3 -
```

#### For Windows (PowerShell):

```powershell
(Invoke-WebRequest -Uri https://install.python-poetry.org -UseBasicParsing).Content | py -
```

Given your requirements, I've updated the README to assume the project already exists as a Poetry project named `resume-builder`. Here's the revised version:

Here's an added section for cloning the repository to include in your README:

## Cloning the Repository

To get started with the `resume-builder` project, first, you need to clone the repository to your local machine. Use the following git command:

```bash
git clone https://github.com/zCoreGroup/resume-builder.git
```

After cloning, navigate into the project directory to begin setup:

```bash
cd resume-builder
```

Follow the subsequent setup instructions to install dependencies and run the project.

### Installing Dependencies

This project uses Poetry to manage its dependencies. Ensure you have Poetry installed. If not, refer to Poetry's [official documentation](https://python-poetry.org/docs/) for installation instructions.

After cloning the project and navigating to the project directory, install the project dependencies by running:

```bash
poetry install
```

This command reads the `pyproject.toml` file and installs all specified dependencies in a virtual environment specific to this project.

### Adding the Template Generator Script

1. **Script Location**

   The template generator script is located at `resume_builder/template_generator.py`. This script uses the `python-docx` library to generate a Word document with customizable sections.

2. **Prepare Required Assets**

   The script expects a `logo.png` file to be present in the project directory. Ensure you have this file, or adjust the script to include the correct path to your logo file.

### Running the Script

To run the script within Poetry's virtual environment, ensuring all dependencies are correctly resolved, use the following command:

```bash
poetry run python resume_builder/template_generator.py
```

This will generate a Word document based on the script's logic and save it to the specified location.

## Contributing

Contributions are welcome! Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details on our code of conduct and the process for submitting pull requests.

## Versioning

We use [SemVer](http://semver.org/) for versioning. For the available versions, see the [tags on this repository](https://github.com/zCoreGroup/resume-builder/tags).

## Authors

* **Michael Bastos** - *Initial work* - [@bastosmichael](https://github.com/bastosmichael)

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.
