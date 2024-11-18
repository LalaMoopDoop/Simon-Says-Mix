** Gabe Mason & Alania Prines ** 
## **Simon Says Test Plan**

### **1\. Boundary Cases**

* **Movement Boundaries:**  
  * Test if the player can move left, right, up, or down as expected.  
  * Ensure the player’s position updates correctly after each move.  
  * Verify that the player stops at boundaries and does not move outside the defined play area.  
* **Score and Level Integration:**  
  * Test if the score increases by the correct amount based on player performance.  
  * Ensure that the level increases at appropriate score thresholds.  
  * Verify that bonus points are correctly applied for special actions.  
* **Edge Cases:**  
  * Test what happens if the game reaches the maximum possible score.  
  * Test if the game behaves correctly when the player attempts to perform invalid actions repeatedly.  
  * Ensure proper functionality when the game speed reaches its maximum level.

---

### **2\. Unit and Logic Testing**

* **Core Mechanics:**  
  * **Player Movement:**  
    * Test the ability to move left, right, up, and down with mapped keys (e.g., arrow keys).  
    * Ensure movement stops at obstacles or boundaries.  
  * **Jumping:**  
    * Verify that the player jumps to the correct height or distance when the jump button is pressed.  
  * **Collision Detection:**  
    * Test if collisions with obstacles are detected accurately.  
* **Game Logic:**  
*   
  * **Scoring System:**  
    * Verify that points are awarded correctly for completing actions.  
    * Check for logic errors in applying multipliers or bonus points.  
  * **Level Progression:**  
    * Test if the game speeds up appropriately as levels progress.  
    * Ensure level progression matches predefined conditions.

---

### **3\. Handling Bad Input and Run-Time Errors**

* **Invalid Key Presses:**  
  * Ensure that pressing keys not mapped to an action is ignored without affecting gameplay.  
  * Test simultaneous key presses to confirm no unexpected behavior occurs.  
* **Unexpected Game States:**  
  * Verify that the game handles scenarios like an empty grid or an infinite loop without crashing.  
  * Test for graceful recovery or notification if the game encounters a corrupted save file.  
* **Error Handling:**  
  * Ensure the game provides clear feedback for errors (e.g., "Invalid input" message).  
  * Test the game’s behavior when the connection to a server (if applicable) is lost.

---

### **4\. Integration Testing**

* **Gameplay and Scoring:**  
  * Ensure that score updates correctly after player actions.  
  * Verify that level progression triggers appropriate speed and difficulty changes.  
* **Menus and Gameplay:**  
  * Confirm that opening menus pauses gameplay.  
  * Ensure that starting a new game resets all game stats and scores.  
* **Movement and Obstacles:**  
  * Test interaction between player movement and obstacles, ensuring no overlap occurs.  
  * Verify that collisions trigger appropriate effects or penalties.

---

### **5\. Design Integration**

* **System Interactions:**  
  * Test how the user interface interacts with game mechanics (e.g., starting or pausing the game).  
  * Verify that inputs from players are processed correctly across different game states.  
  * Ensure that visual elements (e.g., score display) update seamlessly during gameplay.  
* **High-Speed Gameplay:**  
  * Confirm that the game remains responsive at high speeds and levels.  
  * Test for any lag or freezing during fast-paced gameplay.  
* **Save and Load Features:**  
  * Ensure that saving and loading game states work without data corruption.  
  * Verify that saved states correctly restore gameplay elements.


| Player count | 1 | Game should accept 1 player	 |
| :---- | :---- | :---- |
| Speed increase | Speed 1 to possible Speed 14 | Speed the pattern increases as you pass the test  |
| Score increase | 0 to 14  | The score starts at zero and increases by \+1 until the game ends or the score is 14\.  |
| Pattern change  | Button lighting up in a different section and faster  | Lighten up buttons should be very responsive and accurate  |
| Full screen | Play until screen is full | Game should end and show “Game Over” |
| Invalid Input | Pressing multiple conflicting keys | Game should ignore conflicting inputs and not crash |
| Save/Load | Valid and invalid save/load data | Game should save/load properly without errors |
| Scoring attempting  | Saving top score when finished  | Top score will be on top of the board	 |


  
			  
			

			
