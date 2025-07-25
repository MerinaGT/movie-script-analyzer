> # CinemAI Insights - A One Stop Solution

CinemAI is a one stop solution solution created for movie buffs. The fullstack app has a movie scene-wise and character-wise analysis feature. It also has genre classification, movie, movie rating prediction and age restriction prediction based on a movie's script.

---

> ## Home Page

The home page offers a wide range of movie options to choose from. Each movie poster can be resized to small, medium, large, or extra-large.

![img](https://github.com/shreyansh-2003/CinemAI.Insights-Movie_Script_Analyser/assets/105413094/d42f5615-1bfc-4cdf-a688-0c87f83ec03e)

---

> ## Plot Pulse: Movie Analysis - OnClick()

When a movie poster is clicked, an in-depth analysis is generated within seconds. The analysis page is divided into two halves:

- **Left Side**:
  - Contains the movie script.
  - Includes a metadata button that, when clicked, replaces the movie script with details such as budget, rating, cast, awards, etc.

- **Right Side**:
  - Showcases various NLP techniques applied to the movie script, represented through interactive visualizations:
    1. **Unveiling Movie Themes with Topic Modeling**: Generates word clouds of prevalent topics in the shape of Melpomene and Thalia Theatre masks.
    2. **Feel the Vibes: Vader Scene-wise Sentiment**: Analyzes the emotional tone of the script on a scene-by-scene basis using sentiment analysis.
    3. **Spotlight on Characters and Locations with NER**: Identifies and classifies entities such as characters, locations, and organizations within the script using Named Entity Recognition (NER).
    4. **A Character's Stage: Scenes per Character**: Shows the frequency of each character's appearances throughout the movie.
    5. **Words That Matter: Dialogue per Character**: Highlights how often each character speaks in the movie.
    6. **Emotion Unveiled: Scene-wise NRC Lexicon Analysis**: Provides an emotional landscape of the script with NRC Lexicon Analysis, covering emotions like anger, anticipation, disgust, fear, joy, positive, negative, sadness, surprise, and trust.
    7. **Decoding Language: POS Tags**: Analyzes the parts of speech used in the script.



https://github.com/shreyansh-2003/CinemAI.Insights-Movie_Script_Analyser/assets/105413094/3535e050-e8c1-4b68-a780-313e443e9339

---

> ## BERTalizing Movie Scripts: Script-based Classification and Predictions

There are three distinct BERT (Bidirectional Encoder Representations from Transformers) based applications that have been fine-tuned to predict the genre (multi-label), age restriction (numeric value), and IMDb rating (numeric value) based on movie scripts. Users can either type in a script in an empty box or autofill the box with a selection of movies from the dropdown menu.

> #### Genre Classification based on Movie Script

<img width="1267" alt="Screenshot 2024-06-22 at 5 11 35 PM" src="https://github.com/shreyansh-2003/CinemAI.Insights-Movie_Script_Analyser/assets/105413094/f73c4944-3fb6-41c8-bf0c-1c31cecbd20a">

> #### IMDB Rating Prediction based on Movie Script 
<img width="1347" alt="Screenshot 2024-06-22 at 5 10 52 PM" src="https://github.com/shreyansh-2003/CinemAI.Insights-Movie_Script_Analyser/assets/105413094/27dc92b5-b704-4e18-8ac6-de985001366f">

> #### Movie Age Restriction based on Movie Script
<img width="1303" alt="Screenshot 2024-06-22 at 5 12 32 PM" src="https://github.com/shreyansh-2003/CinemAI.Insights-Movie_Script_Analyser/assets/105413094/d0a7ab51-bc99-4269-aa6d-7b8914827536">

---

> # Running the CinemAI Insights Application

- Downloading additional (Large) Files
  1. Download the *.H5 files*, *pre-trained tokenizers* and *NCR-lexion* into the ```Models Folder``` from the [**reostiory link**](https://1drv.ms/f/s!AqM-iZWYLD9iiMEmcCXRkrZWoTSUtQ?e=J1UXvK) givem in README.md of the Models folder.
  2. Download the *Raw Folder*, *Processed Folder* and *cinema_mask.png* into the ```Data Folder``` from the [**reostiory link**](https://onedrive.live.com/?authkey=%21ADXkviDnwGJw8%2DE&id=623F2C9895893EA3%21139432&cid=623F2C9895893EA3) givem in README.md of the Data folder.
  3. Extract the compressed file ```movie poster images.zip``` present in *App/static/images*

- Install required libraries from requirements.txt (Command -> pip install -r requirements.txt)

- Run app.py in ```App Folder``` as a Flask server


**Note:** Kindly email shreyansh.padarha@outlook.com to request acess to the above links by providing viable reasoning.

---

> ## Notebooks

There are two `.ipynb` Jupyter Notebooks in the Notebooks Folder.

1. The ```Movie Analysis - onClick Graph Rendering.ipynb``` Jupyter Notebook has comprehensive tools in the form of Class Instances and FUnctions for analyzing movie scripts, with a particular example focused on the "X-Men" movie

![image](https://github.com/shreyansh-2003/CinemAI.Insights-Movie_Script_Analyser/assets/105413094/dba16ca9-ed80-42cb-a427-3920f52b4b6c)

2. The ```Model Training - BERT text classification & prediction.ipynb``` Jupyter Notebook involves fine-tuning the BERT and RoBERTa models and using the models for various purposes with examples. The primary tasks are predicting IMDb user ratings, classifying genres, and predicting age restrictions based on movie scripts.  For the purposes of demonstration a wide variety of paragraphical explanations and examples like movies, reddit posts and songs have been taken into consideration for the notebook.

![image](https://github.com/shreyansh-2003/CinemAI.Insights-Movie_Script_Analyser/assets/105413094/dcb68411-6de5-4222-ba68-d2d776036f2a)


---

> ## Extra: OfficeGPT - A ChatBot based on the American TV Show "The Office

This repository also presents OfficeGPT, a fine-tuned implementation of DialoGPT specifically designed to generate dialogue in the style of characters from the popular American television series "The Office." By leveraging existing resources, the model has been trained to capture the unique speech patterns and conversational dynamics of the show's characters.

https://github.com/shreyansh-2003/CinemAI.Insights-Movie_Script_Analyser/assets/105413094/1faea283-d2bc-4601-b5e3-9a64ef377c62

Training Methodology: OfficeGPT employs a fine-tuning approach based on the DialoGPT architecture. The model was iteratively trained on a dataset of approximately 45,000 dialogue lines spanning all nine seasons of "The Office." This dataset was carefully curated to represent the speech of various characters, ensuring a comprehensive understanding of the show's dialogue style.

Implementation Details: A Jupyter Notebook (.ipynb) file, approximately 75 MB in size, is included in this repository. This notebook outlines the training process and is customized to work with a separate CSV script containing the dialogue dataset. The script can be downloaded from the following [public repository]([url](https://www.kaggle.com/datasets/nasirkhalid24/the-office-us-

Model Size and Availability: Due to the significant size (over 9 GB) of the trained OfficeGPT model, it has not been included in this repository for practical reasons. However, the provided Jupyter Notebook offers a comprehensive guide for those interested in replicating the training process and generating their own "Office"-inspired dialogues.
