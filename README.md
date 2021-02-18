# shopping-cart
Program that asks the user to input one or more product identifiers, looks up the prices for each, and then prints an itemized customer receipt including the total amount owed.

## Prerequisites

  + Anaconda 3.7+
  + Python 3.7+

## Installation

Fork this [remote repository](https://github.com/victoriaruesch/shopping-cart) under your own control, then "clone" or download your remote copy onto your local computer.

Then navigate there from the command line (subsequent commands assume you are running them from the local repository's root directory):

```sh
cd shopping-cart
```

Use Anaconda to create and activate a new virtual environment, perhaps called "shopping-env":

```sh
conda create -n shopping-env python=3.8
conda activate shopping-env
```

From inside the virtual environment, install package dependencies:

```sh
pip install -r requirements.txt
```

> NOTE: if this command throws an error like "Could not open requirements file: [Errno 2] No such file or directory", make sure you are running it from the repository's root directory, where the requirements.txt file exists (see the initial `cd` step above)

## Setup

In in the root directory of your local repository, create a new file called ".env", and update the contents of the ".env" file to specify your municipalitie's tax rate:

    TAX_RATE= 0.0875

> NOTE: the ".env" file is usually the place for passing configuration options and secret credentials, so as a best practice we don't upload this file to version control (which is accomplished via a corresponding entry in the [.gitignore](/.gitignore) file)

## Usage

Run the program script:

```py
python shopping_cart.py

```