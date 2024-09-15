 # codechallengeIII
Freebie Tracking App
Project Overview

This project is a Python-based Freebie Tracking App that allows companies to give out freebies to developers. It demonstrates concepts of Object-Oriented Programming (OOP), object relationships, and aggregate/association methods in Python.

The main features include:

    Companies can give out freebies to developers.
    Developers can receive multiple freebies.
    Freebies track the item given, the company that gave it, and the developer who received it.

Key Concepts Demonstrated:

    Object-Oriented Programming (OOP): Classes such as Company, Dev, and Freebie encapsulate relevant data and behaviors.
    Object Relationships: The relationship between companies, developers, and freebies is implemented using Python objects.
    Aggregate and Association Methods: Methods such as give_freebie, print_details, and received_one are used to manage and retrieve associated data.

Here's a sample README.md file that you can include for your project, covering key aspects like setup, usage, and features. You can modify it based on the specifics of your project.
Freebie Tracking App
Project Overview

This project is a Python-based Freebie Tracking App that allows companies to give out freebies to developers. It demonstrates concepts of Object-Oriented Programming (OOP), object relationships, and aggregate/association methods in Python.

The main features include:

    Companies can give out freebies to developers.
    Developers can receive multiple freebies.
    Freebies track the item given, the company that gave it, and the developer who received it.

Key Concepts Demonstrated:

    Object-Oriented Programming (OOP): Classes such as Company, Dev, and Freebie encapsulate relevant data and behaviors.
    Object Relationships: The relationship between companies, developers, and freebies is implemented using Python objects.
    Aggregate and Association Methods: Methods such as give_freebie, print_details, and received_one are used to manage and retrieve associated data.

Directory Structure

bash

code_challenge/
│
├── models/
│    ├── __init__.py          # Marks the models directory as a Python package
│    ├── company.py           # Company class implementation
│    ├── dev.py               # Dev (developer) class implementation
│    ├── freebie.py           # Freebie class implementation
│    └── main.py              # Main script for testing and running the program
├── README.md                 # This README file
└── requirements.txt          # Project dependencies (if any)

Installation and Setup
1. Clone the repository:

bash

git clone git@github.com:username/repository.git
cd repository

2. Set up the environment:

    If you are using a virtual environment (recommended), set it up:

    bash

    python3 -m venv env
    source env/bin/activate

3. Install dependencies:

    Install any dependencies listed in the requirements.txt file:

    bash

    pip install -r requirements.txt

Usage
1. Run the main script:

To run the main script and see the program in action:

bash

python -m models.main

2. Example interactions:

In the main.py file, you will find examples of how to use the classes:

python

from models.company import Company
from models.dev import Dev

# Create company and developer objects
company = Company("TechCorp")
dev = Dev("Alice")

# Give a freebie to the developer
company.give_freebie("T-shirt", dev)

# Print out the freebies
dev.show_freebies()
company.total_freebies()

3. Running Tests (Optional):

If you want to add tests for the functionality:

    Create a tests/ directory and use unittest or pytest to write and run tests.

Features

    Company Class: Can give out freebies and keep track of all the freebies it has given.
    Dev (Developer) Class: Receives freebies from companies and can list all the items it has received.
    Freebie Class: Tracks the individual freebie, including the item name, the company that gave it, and the developer who received it.

Methods Overview
Company Class

    give_freebie(item_name, dev): Assigns a freebie to a developer.
    total_freebies(): Returns the total number of freebies given by the company.

Dev Class

    receive_freebie(freebie): Receives a freebie and stores it in the developer's list of freebies.
    show_freebies(): Displays all the freebies received by the developer.

Freebie Class

    print_details(): Prints the details of the freebie (developer, company, and item).

Contributing

If you'd like to contribute, feel free to fork the repository and submit a pull request.
License

This project is licensed under the MIT License - see the LICENSE file for details.
