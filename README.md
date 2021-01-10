# Simple Test Application 
## Info:
- The application main purpose is to train yourself on a specific exam.
- This application contains several oracle exam certification questions (the actual ones from 2020) so feel free to train or test your knowledge


## How to add new tests:
The test object is pretty simple, you'll need to open the `examData.js` and add a new block or replace all of them with your own:
```
[
    {
        name: "Your Test Name",
        link: "this-is-optional",
        questions:[
            {
                question: "First question",
                answers: [
                    {
                        answer:"Option 1",
                        isCorrect: false
                    },
                    {
                        answer:"Option 2",
                        isCorrect: false
                    },
                    {
                        answer:"Option 3",
                        isCorrect: true
                    }
                ]
            },
            {
                question: `Another question`,
                answers: [
                    {
                        answer:"Option 1",
                        isCorrect: false
                    },
                    {
                        answer:"Option 2",
                        isCorrect: false
                    },
                    {
                        answer:"Option 3",
                        isCorrect: true
                    },
                    {
                        answer:"Option 4",
                        isCorrect: true
                    }
                ]
            }
        ]
    }
]
```

## Notes:
- if your question has only one corrent answer, the engine will create radio buttons for the answers
- if your question has more that one corrent answers, the engine will create checkboxes for answers
- you can place your questions/answers between this \` \` insteand of this "" to display it in different lines or to insert HTML objects such as images