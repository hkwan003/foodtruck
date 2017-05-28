# San Francisco Food Trucks
A python command line program that prints out an alphabetically ordered list of all food trucks (10 at a time) that are open at that moment.

This program uses the Mobile Food Schedule API, a subset of the The San Francisco Data API found [here](https://dev.socrata.com/foundry/data.sfgov.org/bbb8-hzi6).

To view assignment requirements, see `assignment.md`.

## Prepping for the program
- Make sure you have Python 2.7 installed.
  - `python --version`
  - If no Python is installed, see the offical installation instructions [here](https://wiki.python.org/moin/BeginnersGuide/Download)
- You will need two external Python libraries, which you can install using [Pip](https://pip.pypa.io/en/stable/installing/).
  - `pip install requests`
    - This Python addon is used to make HTTP requests to the external API
  - `pip install tabulate`
    - This will make your food truck console output pretty 🌻
- If you plan to use this API heavily, get an App Token from the San Francisco API website [here](https://dev.socrata.com/docs/app-tokens.html)
  - Place the API token in your environment using the key name `FT_APP_TOKEN`
    - Edit your shell profile (i.e. `.bashrc`) to export the new variable
    - Your .bashrc file can be found by typing `cd ~` `ls -a`. Open it in your editor of choice.
    - If it doesn't exist, create it by typing `touch ~/.bashrc`.
    - Inside your .bashrc, add `export FT_APP_TOKEN="<paste from website>"`
    - Save and reload your shell by typing `source ~/.bashrc`
  - The program can be run without a token, but your usage will be throttled.

## Executing the program
- Git clone this repository
- Navigate into the folder `food-trucks` in your command line.
  - `cd food-trucks`
- Run test (yes singular, sorry) by typing `python tests.py`
- Run the program by typing `python show-open-food-trucks.py`
- Follow the instructions given in the console for more
