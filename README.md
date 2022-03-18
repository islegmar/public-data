# Public Data

List of Questions & Answers for the Mobile Application [OpenQuizz](https://play.google.com/store/apps/details?id=appinventor.ai_islegmar.OpenQuizz)

# How to Contribute

You can become an OpenQuizzer contributing addding your own list of Questions! Toi do that:
- Create a branch and add your JSON with your Questions.
- Update the file [main.json](main.json) to add your file
- Create a PR to incorporate your contribution in the game.

# How to wirte your Questions

The JSON with the Questions has the following format

    [
      {
        "q" : "<The text for the question>",
        "t" : "<The right answer>",
        "f" : [
          "<Wrong answer #1>",
          "<Wrong answer #2>",
          "<Wrong answer #3>"
        ]
      }
      ...
    ]

where the number of **wrong** answers can be from 1 until 3. In the case of True/False questions the format would be (in case the right answer is True)


    [
      {
        "q" : "<The text for the question>",
        "t" : "True",
        "f" : [ "False" ]
      }
      ...
    ]

For example something like

    {
        "q": "What is Manny afraid of?",
        "t": "Butterflies",
        "f": [
            "Marshmallow",
            "Matt LeBlanc",
            "Spoons"
        ]
    }

Will be shown as the question **What is Manny afraid of?** offering the following possible answers in randfom order:
- Butterflies
- Marshmallow
- Matt LeBlanc
- Spoons

being **Butterflies** the right answer.
    
