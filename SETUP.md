### Running This Project

This guide explains how to set up and run the SlapThatLikeButton-TestingStarterProject, including the role of each configuration file.

---

### **1. Install Dependencies**

#### Recommended:

Open a terminal in the project's root directory and run:

```bash
pip install .[testing]
```

This installs all runtime and development dependencies as defined in **setup.cfg**.

#### Alternatively:

You can install dependencies from the requirements files:

```bash
pip install -r requirements.txt
pip install -r requirements_dev.txt
```

This installs runtime dependencies (**requirements.txt**) and development/testing tools (**requirements_dev.txt**).

### **2. Configuration Files Explained**

#### `pyproject.toml`

- Defines the build system (**setuptools**, **wheel**).
- Configures tools like **pytest** and **mypy**.
- Ensures consistent builds and tool settings.

#### `setup.cfg`

- Main package configuration.
- Contains project metadata (**name**, **author**, **license**).
- Lists dependencies (**install_requires**) and optional extras (`[options.extras_require]`).
- Configures package data and linter settings.

#### `requirements.txt`

- Lists runtime dependencies in a simple format.
- Used for quick installation with `pip install -r requirements.txt`.

#### `requirements_dev.txt`

- Lists development and testing dependencies (**pytest**, **pytest-cov**, **mypy**, **flake8**, etc.).
- Used for setting up a development environment with `pip install -r requirements_dev.txt`.

---

### **3. Summary**

- Use `pip install .[testing]` for a complete setup.
- Configuration files help manage dependencies, packaging, and development tools.

You can copy and use this as your project’s setup guide.
