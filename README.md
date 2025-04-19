For the text = """
Thank you for reaching out regarding the delivery issue. We apologize for the delay.
Your package is on its way and should arrive by the end of the week.
"""

expected output: ["delivery issue", "delayed", "arrival: end of week"]


I am getting the following output from the models:

miniLM with keyphrase_ngram_range = (1, 2) and top_n = 5: ['delivery issue', 'regarding delivery', 'delivery', 'arrive', 'way arrive']

miniLM with keyphrase_ngram_range = (1, 3) and top_n = 3: ['reaching regarding delivery', 'arrive end week', 'delivery issue']  



