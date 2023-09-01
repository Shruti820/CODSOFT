# CODSOFT
#quize questions and answers
questions={
    "what is the capital of france?":"paris",
    "what is the largest planet in our solar system?":"jupiter",
    "who painted the mona lisa?":"leonardo da vinci"
    }
#function to run the quize game
def quize_game():
    score=0
    for question,answer in questions.items():
        user_answer=input(question+" ")
        if user_answer.lower()==answer.lower():
            score+=1
            print("correct")
        else:
            print("incorrect")
        print("quize finished")
        print("your score:",score)

        
#run the quize game
        
quize_game()
