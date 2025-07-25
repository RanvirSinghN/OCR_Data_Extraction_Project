# OCR_Data_Extraction_Project
During my two weeks work placement with the Santander Data Science team, I had a personal project to create an OCR model for several types of documents. 

A User Interface is created to accept pdf files and then the pdf files are processed into imges that the gpt model can read using base64 coding.

Gpt 4.1 Mini was used to succesfully identify the type of document from a list: Bank Statement, Passport, Council Tax, Payslip, Driving Licence, 
Accountant Certificate, P60, TYO, SA302. Extraction was still attempted for other types of documents. Once the document was identified, a further prompt was called to extract the unique useful information depending on type of document used. Worked succesfully with high accuracy for every type of document listed.

Threading was also used to show live updates with UI while extraction of information occured. Time of extraction was also displayed

API key is required to test program, replce os.getenv("API_KEY") with your API key. 

I then went on to further try 'Agentify' the model, I played around with the LLMs and tried to see if I could get the LLM to do my code for me by parsing all my functions as strings into the model or unsing the API function calling method. I then compared the time it took for all three methods and the results can be seen in the table 'LLM_comparsion_times'.
