# Exploring the Presidential Speeches of Donald Trump
## Introduction
Political speech plays a crucial role in comprehending political discourse, as it provides valuable insights into power dynamics and conflicts within societies. This corpus serves as an example, storing the presidential speech data of Donald Trump during his term in office. Researchers can leverage this corpus to gain in-depth insights into shifts in public opinion, power dynamics, and internal societal conflicts by analyzing changes in speech themes and linguistic tendencies.
## Documentation
### Corpus Description
This corpus comprises data collected from Donald Trump's presidential speeches spanning from 2017 to 2021, stored in both CSV and text formats, obtained through web scraping from the [Miller Center's website](https://millercenter.org/the-presidency/presidential-speeches), which serves as a collection of text data, including speeches given by U.S. presidents from George Washington's era to the present. Importantly, staff of the center refrain from making any artificial alterations to the speeches, ensuring the integrity of the corpus. In accordance with the [terms of service](https://data.millercenter.org/), all the speeches are in the public domain, and can be freely utilized for research and academic purposes.
### Target Audience and Intended Use  
This corpus is tailored for researchers, scholars, and students in political science, linguistics, and social sciences. Additionally, it is accessible to the general public interested in American politics. The primary aim of this corpus is to provide a comprehensive resource for in-depth studies and research on the language and themes within presidential speeches, particularly those delivered by Donald Trump during his tenure. Its intended applications include political discourse analysis, linguistic studies, public opinion research, etc.  
#### Potential Research Questions  
&bull; What are the most frequently words used by Trump?
&bull; Does the main focus of Trump change and what factors are associated with it?
### Text Selection Criteria  
There are 32 presidential speeches for this corpus. The selection of speeches for this corpus was based on [the Presidential Speeches Collection](https://millercenter.org/the-presidency/presidential-speeches) from [Miller Center's website](https://millercenter.org/the-presidency/presidential-speeches). According to the [Miller Center of Public Affairs](https://data.millercenter.org/), the collection is not exhaustive, with over 1000 speeches available, and inclusion in the collection is an editorial decision by Miller Center staff.
### Data Collection Process  
1. Manually searching for presidential speeches of Trump on Miller Center's website.
2. Employing web scraping techniques to gather the transcripts of the speeches.
3. Storing the metadata of speeches in a CSV file.
4. Storing each of Trump's speeches as an individual TXT document.
### Cleaning and Preprocessing  
In the process of text preprocessing, several steps were employed to improve the cleanliness of the transcript texts. Initially, excess white spaces and newline characters (\n) were removed to create a more structured text. Following this, the operation re.sub(r'[^\w\s]', '', cleaned_text) was employed to eliminate non-alphanumeric characters. Additionally, converting the entire text to lowercase using cleaned_text = cleaned_text.lower() ensured consistency. Collectively, these steps refined the text in preparation for subsequent analysis.  
### Annotations and Tools Used  
The corpus incorporates annotations like tokens, lemmas, part-of-speech (POS) tags, and date, etc. These annotations were achieved using pandas and spaCy.  
### The Format of The Files  
This corpus organizes Trump's speeches into 32 separate text files, categorized by the speech time. All files are contained within a single directory.  
###  Columns of CSV File with Annotations
&bull; Filename: The file name, a unique identifier for each speech in the format PresidentName_speech_i.txt.  
&bull; Title: The title of the speech.  
&bull; Speech: The original text of the speech.  
&bull; Tokens: Individual words or text units after preprocessing.  
&bull; Lemmas: Base or normalized forms of words after preprocessing.  
&bull; Parts-of-speech: Part-of-speech tags indicating the grammatical category of each word after preprocessing.  
&bull;President: The name of the president.  
&bull; Date: The date of the speech.  
&bull; Summary: A summary of the speech.  
&bull;Link: The link to the speech.
### Quality Check  
1. The staff at the Miller Center ensure the accuracy of the corpus by refraining from making any adjustments to the transcriptions of presidential speeches during the process of converting audio materials into written documents.
2. Data cleaning and preprocessing are undertaken to elevate the accuracy and quality of the data.
3. The decision to include presidential speeches in the corpus is made by the editors at the Miller Center. The criteria for inclusion may be subjective and influenced by the biases of individual. Additionally, it's acknowledged that the corpus may not be exhaustive.
### Columns of CSV File with Annotations  
&bull; Filename: The name of each speech delivered by Trump.  
&bull; Title: The title of each speech in the text files.  
&bull;

