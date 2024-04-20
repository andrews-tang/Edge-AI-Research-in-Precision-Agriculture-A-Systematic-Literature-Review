## Leveraged DistilBERT to classify the unseen papers for the full-text screening

I am working on a systematic literature review paper on the possible Edge AI implementations in the Precision Agriculture.
I got a lot of results after I searched my three search strings on three research databases.
After removing duplicates, retracted papers and other materials, I still had a lot of papers.
Moreover, following PRISMA, I need to screen the titles and abstracts of the curated papers before I can do full-text screening and then finally settle on the actual papers to be used for the review.
Dodging the manaul approach, I thought of automating the process using pretrained NLP models. Specifically, I used DistilBERT and got amazing results.

## I used Zotero as my referenicng software.
All I needed was to get the bib file of some few papers manaually screened with their labels (relevant or non_relevant).
I then exported this bib file and extract the titles and abstracts to generate my dataset (this was my training set).

For the test set, I just exported the bib file of the papers I wanted to classify as either relevant or not relevant.
Then, I used the saved retrained-pretrained model (DistilBERT) on make my classification.
That's all.
