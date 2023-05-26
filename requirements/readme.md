This folder use packages: pipreqs and nbconvert
- nbconvert: convert our notebook into a .py file in a new directory called requirements
- pipregs: then run pipreqs in the new directory. 
--> The reason for this is that pipreqs only works on .py files

The requirements.txt will be generated and can be used later on.

run commands:

1. "jupyter nbconvert --output-dir="./requirements" --to script file_name.ipynb" for individual ipynb
   or "jupyter nbconvert --output-dir="./requirements" --to script *.ipynb" for all ipynb

2. pipreqs ./requirements --force

# and to make it work properlly, use: pip install 
nbconvert==7.2.1
mistune==2.0.4