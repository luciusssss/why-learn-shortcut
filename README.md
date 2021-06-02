# Why Machine Reading Comprehension Models Learn Shortcuts?
Data and code for 'Why Machine Reading Comprehension Models Learn Shortcuts?', Findings of ACL 2021

## Data
The synthetic datasets proposed in our paper are in the `dataset.zip` file.
### Size

|                        | Train (Pairs) | Dev (Pairs) |
|------------------------|---------------|-------------|
| Question Word Matching | 6306          | 766         |
| Simple Matching        | 7562          | 952         |

### Format
The format of each dataset is as follows (same with the format of  of SQuAD).
The version of the question (challenging or shortcut) is denoted in the key `qtype`. 
```
{
  "version": "simple_matching_dev_challenging",  		// dataset version
  "data": [
    {
      "paragraphs": [
        {
          "cid": "squad1.1-dev-1_h", 				// context id
          "context": "As this was the 50th Super Bowl...",
          "qas": [
            {
              "id": "56be8e613aeaaa14008c90d2_h", // question id
              "question": "What day was the game played on?",
              "answers": [
                {
                  "text": "February 7, 2016",
                  "answer_start": 505 		// the start position of the answer in the context
                }
              ],
              "qtype": "challenging" 			// question type (challenging/shortcut)
            }
          ]
        }
      ]
    }
  ]
}
```


## Code
We are preparing the code for this paper. It will be released soon.
