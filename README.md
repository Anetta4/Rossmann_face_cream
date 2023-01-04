# Rossmann_face_cream
**About Dataset:**
This dataset is the result of web scraping the Rossmann website.
On main sites there are information about Brand, Name of the series of cream, Price, Links to direct sites of products.

From direct sites the lists of ingredients and short descriptions are downloaded.
Finally we get dataset split to columns:

* Link - link to direct product used as a 'https://www.rossmann.pl{link}',
* Brand - main producer of the product,
* Series - unique series of product or product line,
* Size - product capacity [ml],
* Price -normal price in PLN, sales are not included,
* Info - short description of the product,
* Ingredients - list of ingredients as type 'str' split by ', '


This dataset is collect using web scraping methods like  beautiful soup to collect useful records from website.

**FIRST MODEL**

I am going to analyze product based on several variables.

Then I build a model with the help of NLP techniques.

I will train the model on raw text without removing stop words and without regularization.
In my data the text is a short description of the product (the name of cream).

I will also create a model that matches the ingredients to the cream category.

 I will vizualize ingredients of creams using a word map.

**SECOND MODEL**

Manufacturers want to sell their products trying different ways to convince customers to buy their brand.

Whenever I want to buy a new face cream, it's so difficult to choose.  New items that I've never tried end up giving me skin trouble. We know the information we need is on the back of each product, but it's really hard to interpret those ingredients list unless you're a chemist:))
So instead of buying and hoping for the best, why don't we use data science to help us predict which products may be good fits for us and their price will be atractiv for us too.

I'm going to create a content-based recommendation system where the 'content' will be the chemical components of cosmetics and their price.  I will process ingredients list  face creams on Rossmann  via word embedding, then visualize ingredients similarity using a machine learning method called t-SNE and an interactive visualization library called Bokeh.
Additionally I will vizualize the similarity of  creams using a cluster hierarchy. 
