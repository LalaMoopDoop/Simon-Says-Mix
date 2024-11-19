** Gabe Mason & Alania Prines 
**Pseudocode Frame**

	1\.	**Start**: Define the beginning of the process.

	2\.	**Input**: Describe what data the program will take in.

	3\.	**Process**: Outline the steps the program will perform with the input.

	4\.	**Output**: State what the program will produce as a result.

	5\.	**End**: Define the end of the process.

---

**Initialize game variables:**  
    **sequence \= \[\]**  
    **user\_input \= \[\]**  
    **round \= 1**  
    **game\_running \= True**

**Function generate\_sequence():**  
    **Randomly select a button and add it to the sequence**

**Function display\_sequence(sequence):**  
    **For each button in sequence:**  
        **Light up the button**  
        **Play corresponding sound**  
        **Wait for a brief period**

**Function get\_user\_input():**  
    **Initialize user\_input as an empty list**  
    **For each button in sequence:**  
        **Wait for player input (button press)**  
        **Add pressed button to user\_input**

**Function check\_input(sequence, user\_input):**  
    **If user\_input matches sequence:**  
        **Return True**  
    **Else:**  
        **Return False**

**While game\_running:**  
    **generate\_sequence()**  
    **display\_sequence(sequence)**  
    **user\_input \= get\_user\_input()**  
      
    **If check\_input(sequence, user\_input):**  
        **Display "Correct\!"**  
        **Increase round by 1**  
    **Else:**  
        **Display "Game Over\!"**  
        **game\_running \= False**

