# 1 Convert Word .docx files into Markdown .md files

**Python Code**: `DocxToMarkdown.py` 

The Python program converts Word `.docx` files into markdown `.md` files. It can process transcripts generated by Microsoft Teams and then removes the image links inside the transcripts. The immediate application is to use these cleaned up markdown files as input to AI applications such as Open AI Studio / APIs. 

### File Directories 

Put all your .docx files in one directory. The program will ask for below paths (`example input` you can provide):

1. Enter the input directory path for .docx files: `C:\data\docx_files_dir`
2. Enter the output directory path for RAW .md files: `C:\data\md_raw_files_dir` 
3. Enter the output directory path for CLEAN .md files: `C:\data\md_clean_files_dir` (If CLEAN_MD = True in .env )

The final output .md files will be stored in the path defined in 3 above. You can modify  `def lineContainsPattern(line)` to fit your own requirements. 

### Required Python Libraries 

Please review the `requirements.txt` for details. 

### Environment File .env

`CLEAN_MD = True` # Remove markdown image links in each file.

# 2 Convert Markdown .md files into Word .docx files

**Python Code**: `MarkdownToDocx.py` 

Same `requirements.txt`. 

No environment variable needed. 

The Python program converts markdown .md files into Word.docx files.

### File Directories 

Put all your .md files in one directory. The program will ask for below paths (`example input` you can provide):

1. Enter the input file path: `C:\data\md_input_files_dir`
2. Enter the output file path: `C:\data\output_files_dir`

The final output .`docx` files will be stored in the path defined in 2 above.

