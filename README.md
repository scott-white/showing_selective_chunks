# showing_selective_chunks
This is a brief example to show how you can use rmarkdown parameters to show selective code chunks.

# How to use this script

## Step 1: Choose your directory.

Navigate to the directory that contains the .Rmd file you want to work on.

## Step 2: Use the script.

Running this line will create a file that just contains the code output without showing the code used to generate it itself.

Rscript -e "rmarkdown::render('master_file.Rmd', output_file = 'questions.pdf', params = list(show_code = FALSE))"

Running this line will create a file that contains the code output with the code used to generate it.

Rscript -e "rmarkdown::render('master_file.Rmd', output_file = 'answers.pdf', params = list(show_code = TRUE))"