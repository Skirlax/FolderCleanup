# FolderCleanup

A simple script to sort a given directory into hardcoded categories based on two factors. Clone this repository to use it.

The program goes and checks:

1. If item is a file, it sorts it based on its type.
2. If item is a directory it checks if more than 70 % of its files are of some type. If so, it sorts it based on that type. If not it calls GPT-4 to sort it based on the logic of its contents. If no category is found either way, the directory is ignored.


In order for this program to be reliable you need to use GPT-4, meaning your API key needs to have access to it.
If you have access create a '.env' file in the directory of this program and add you key in the following format:
OPENAI_API_KEY="YOUR-KEY"
