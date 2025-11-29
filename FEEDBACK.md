# Feedback

## Round 1

### Repo structure

- Where are the data sources?
- Would separate the notebook into multiple notebooks. Would also use more code cells - I see you lump a lot of code together when really you want to check code at every step of the way. I point out an example in the notebook feedback.
- Please reorganize your notebooks instead of using `globals()`. There are times where you might need to use this, but incredibly rarely, when there is no other way to do things. In your case, you are using it to make sure you ran some cells, which I understand - but you could save your data into a `.csv` files and read them at the top of the notebook and you don't need to this again.

### README

- > develop and test models that balance financial return maximization with sustainability objectives
    - I would be careful about calling something "a model". Even if you are introducing a carbon-adjusted risk score, it's not exactly a model. You call a model something that is trying to reflect reality in one way or another. For example, qhen you do a financial model, you are trying to see how things like revenue and profit would look like in reality. Same with prediction models, you are trying to get a value that will happen in the future, in reality.
    However, the score you are introducing is something that you are inventing yourself rather than modelling after reality, so **would rephrase this sentence**.

- 💾 Repository Contents
    - This section is not necessary

- > which is penalized or weighted based on the portfolio's aggregate ESG score 
    - how exactly is it penalized or weighted?

- Key Findings
    - Move this at the top, after overview

- Methodology Highlights
    - would rename to just "Methodology"
    - move under SSR section

- Other
    - add an Executive Summary section afterwards

