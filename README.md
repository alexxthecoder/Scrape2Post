# Scrape2Post
This Click tool scrapes web article content using newspaper3k, paraphrases the content using a NLP model (Hugging face - tuner007/pegasus_paraphrase) and posts said content to wordpress drafts using its API.
To use this tool you will need to;

a, install necessary dependencies (check import statements)

b, create a venv to work in/ avoid dependency conflicts

c, create a config.ini file to store WP credentials and URL

d, Run it with ``` python scrape2post.py set credentials ``` to set credentials

e, follow prompts and input creds, also provide destination url like so <https://your-website.com/wp-json/wp/v2>

f, Run with ``` python scrape2post.py scrape_and_post url https://target-article-url.com ```

g, Scrape2Post Click tool can also output summary, title, authors, etc of scraped article using Newspaper3k, load print statement on line 110 as necessary.

PS:
 The specific NLP model used in this is lightweight and adequate but has drawbacks dealing with high content text. Edit the output before publishing or [change]([https://www.google.com](https://huggingface.co/models?pipeline_tag=text2text-generation)https://huggingface.co/models?pipeline_tag=text2text-generation) the model if necessary.

