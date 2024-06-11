# Common-Dataset-Extractor
 extract data from common data sets

## first attempt
1. Import basic colleges names (about 500 colleges that has USNews rankings)
2. Google search query "filetype:PDF"+"college name"+"2023-2024 common data set"
3. download all available PDFs
4. convert PDF to images
5. OCR extract texts and store in vectorstore, 1 page = 1 document
6. run 2 seperate query to retrive college name and GPA requirement related pages
7. send combined documents to LLM and request structured output
8. save everything in a dataframe and save to a csv file

When I try to clean the data, I found lots of errors, for example, at first and second step, there might be other colleges' PDFs downloaded, also when extract information, LLM make things up (this is might be preventable by prompting)
need to work on another solution for better and accurate information extraction.
