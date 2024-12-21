Oh no! Were you kinda lazy while writing your latex doc, and now you want to double check and/or 
organize citations? Couldn't be me, id never be so kinda lazy i needed to write a code to compensate...

This Python code is designed to extract citations from a LaTeX document 
(.tex file) uploaded via a file upload widget in a Jupyter Notebook environment. 
The extracted citations are saved in an Excel spreadsheet, with each citation 
listed in the order it appears in the document.
How the Code Works:

    1. Upload File:
        The file name and content are processed upon upload.
        
    2. Extract Citations:
        The file content is decoded from memoryview into a string.
        The regular expression searches for all instances of \cite{} and extracts citation keys in the order they appear.
        
    3. Save to Excel:
        The extracted citations are stored in a pandas DataFrame.
        The DataFrame is saved as an Excel file in the current working directory.
