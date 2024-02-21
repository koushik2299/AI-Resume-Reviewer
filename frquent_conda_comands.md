conda env list -- Allows you to check for existing list of Virtual Environments 

cls to clear the termnial

# Conda Commands Tutorial

Conda is an open-source package management and environment management system that is widely used in the data science and machine learning communities. It allows users to easily install, run, and update packages and their dependencies. This tutorial will guide you through the basics of using Conda, including installation, creating environments, managing packages, and more.

## Installing Conda

To use Conda, you first need to install it. Conda is included in Anaconda and Miniconda distributions. Anaconda includes Conda and a large number of scientific packages by default, while Miniconda includes Conda and a minimal set of packages.

- **Anaconda:** Download the Anaconda installer from the [official website](https://www.anaconda.com/products/distribution) and follow the installation instructions.
- **Miniconda:** Download the Miniconda installer from the [Miniconda website](https://docs.conda.io/en/latest/miniconda.html) and follow the installation instructions.

## Checking Conda Installation

After installing, you can check the installation by opening a terminal or command prompt and typing:

```bash
conda --version
```

This command should display the version of Conda installed.

## Managing Environments

### Creating a New Environment

To create a new environment with a specific Python version, use:

```bash
conda create --name myenv python=3.8
```

Replace `myenv` with your desired environment name and `3.8` with your desired Python version.

### Activating an Environment

To activate the environment, use:

- **On Windows:**
  ```bash
  activate myenv
  ```
- **On macOS and Linux:**
  ```bash
  source activate myenv
  ```

### Deactivating an Environment

To deactivate the current environment and return to the base environment, use:

- **On Windows:**
  ```bash
  deactivate
  ```
- **On macOS and Linux:**
  ```bash
  source deactivate
  ```

### Listing Environments

To list all environments you have created, use:

```bash
conda env list
```

or

```bash
conda info --envs
```

## Managing Packages

### Installing Packages

To install a package in the active environment, use:

```bash
conda install numpy
```

Replace `numpy` with the name of the package you wish to install.

### Updating Packages

To update a specific package, use:

```bash
conda update numpy
```

To update all packages in the current environment, use:

```bash
conda update --all
```

### Listing Installed Packages

To list all packages installed in the current environment, use:

```bash
conda list
```

## Removing Packages or Environments

### Removing a Package

To remove a package from the current environment, use:

```bash
conda remove numpy
```

### Removing an Environment

To remove an entire environment, use:

```bash
conda env remove --name myenv
```

## Conclusion

This tutorial has covered the basics of managing environments and packages with Conda. For more detailed information and advanced usage, refer to the [official Conda documentation](https://docs.conda.io/projects/conda/en/latest/).