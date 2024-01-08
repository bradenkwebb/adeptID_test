# adeptID_test
My response to AdeptID's technical assessment, completed in the course of interviewing for a position in data science.

### Set-up
1. Clone this repository to your local machine.
2. If desired, create a virtual environment for this project and activate it
3. Install the required packages using `pip install -r requirements.txt`. I haven't had a chance to test this on a non-Windows machine, but on Google Colab, the command `!pip install -q pandas scikit-learn chromadb sentence-transformers skops matplotlib tqdm gdown` is sufficient as of 1/8/2024.
4. Download the database of pre-computed embeddings. This is a 1.4 GB file (since it also duplicates the data in `data.csv`), so I uploaded it to my google drive at https://drive.google.com/file/d/1YiN8uWU7ijgcrhut5f13ypoCBKJSxcK3/view?usp=sharing. Download it and place it in the root directory of this repository. To do this programmatically, you can run `gdown --id 1YiN8uWU7ijgcrhut5f13ypoCBKJSxcK3`
5. Unzip the database. This can be done programmatically with `unzip -qn vectordb.zip`.

### Inference
I felt that an interactive notebook was a more fitting format for this assessment than a script, so my code is currently all contained in `notebook.ipynb`. You should be able to run each cell in the provided notebook in order to reproduce my results. The `predict()` function is defined near the bottom, but stands alone for small $N$.