# llm-archives

### Instructions

Click the "Use this template" button for this repository and choose "Create a new repository". You can give it the same name (llm-archives).

Once it's ready, go to [Groq](https://console.groq.com/keys) and follow the directions to get an API key. You'll need to login (or create an account if you don't have one).

Copy the API key value and then click on the Settings of your GitHub repository and click on "Secrets and variables" on the left side, then choose "Codespaces"

Click the green "New Repository Secret" button and paste your API Key into the "Secret" box, then put GROQ_API_KEY in the Name box above it. Click "Add Secret" and click on the name of the repository to return to the main page.

From there, click the green "Code" button and create a new Codespace in the Codespaces tab.

In the Terminal type the following: pip install requests groq and hit enter.

Then type: python get_stories.py

You should see a file called cns_maryland_posts.json appear. Let's look at it. It contains some details of the past 10 CNS stories.

Back in the Terminal, type: python entity_extraction.py and watch the output.

### Evaluation for JOUR389W

The extraction was initially slow when I ran it for the CNS data, but that makes sense because it was going through 10 articles, while this was just the text from one article. It did the extraction for my Chartmetric article in just a second and its results were pretty accurate. When I checked the people mentioned in the article list to the article, it did list most of the artists mentioned in the article that did perform at 2024's Coachella, along with KAYTRANDA and Aminé who did well in charting after 2023's Coachella, the couple artists they forgot in the list was the K-Pop artists mentioned near the end of the article. It did get the place correct as this just surrounds Coachella and even indicated where in California Coachella is located. The organizations mentioned make senseas to the article describing where these artists are gaining traction.

This was a interesting assignment and this type of assignment for an AI would be super helpful in a case such as going through a court document or other long PDF where you need to see who, what and where things happened, espeically if you are trying to see if certian people or places are mentioned. This would also be helpful in the case of trying to find names of credible sources for an article if you are searching through a journal article other archive.
