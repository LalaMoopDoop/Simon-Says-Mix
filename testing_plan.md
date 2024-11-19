# Gabe Mason & Alania Prines # 
# **Simon Says Test Plan**

## **1. Boundary Cases**

* **Pattern and Sequence Boundaries:**  
  * Verify that the game correctly generates a pattern of increasing length after each successful round.  
  * Test that the player cannot add extra inputs beyond the generated sequence length.  
  * Ensure that no invalid patterns (e.g., empty or incomplete) are generated.

* **Score and Level Integration:**  
  * Test if the score increments correctly with each successfully repeated sequence.  
  * Confirm that the game adjusts the speed of patterns appropriately with level progression.  
  * Verify if bonus points are awarded for perfect accuracy in input timing.

* **Edge Cases:**  
  * Test the behavior when the player achieves the maximum score (e.g., 14 or a defined max).  
  * Ensure the game handles rapid incorrect inputs (spam) without crashing.  
  * Verify that the game handles sequences that become too fast for human response.

---

## **2. Unit and Logic Testing**

* **Core Mechanics:**  
  * **Sequence Generation:**  
    * Test if patterns are generated randomly and do not repeat too frequently.  
    * Verify that the pattern is displayed clearly with accurate button light-ups and timing.  
  * **Player Input:**  
    * Confirm that input is correctly matched to the displayed sequence.  
    * Ensure partial matches (correct start, wrong end) are identified as incorrect.  
  * **Button Interaction:**  
    * Verify that button presses trigger the correct responses (light-up and sound).  
    * Test that simultaneous button presses are ignored.

* **Game Logic:**  
  * **Scoring System:**  
    * Verify points are correctly awarded for each completed sequence.  
    * Ensure the score resets upon game over or when starting a new game.  
  * **Level Progression:**  
    * Test if the game speeds up in predefined increments after specific scores or levels.  
    * Confirm that progression does not exceed the app’s performance capabilities.

---

## **3. Handling Bad Input and Run-Time Errors**

* **Invalid Key Presses or Touches:**  
  * Ensure that tapping outside of buttons is ignored.  
  * Test handling of rapid or overlapping inputs.  

* **Unexpected Game States:**  
  * Verify that an incomplete pattern input results in a proper "game over."  
  * Ensure the game doesn’t crash if a sequence is interrupted mid-play.  

* **Error Handling:**  
  * Confirm that feedback for wrong inputs is clear (e.g., sound, flashing screen, "Try Again" message).  
  * Test the app’s behavior under low-memory conditions or sudden app closure.

---

## **4. Integration Testing**

* **Pattern Display and Input Matching:**  
  * Ensure that patterns light up buttons in the correct order and intervals.  
  * Verify that the input matching system evaluates player inputs accurately.  

* **Menus and Gameplay:**  
  * Confirm that pausing the game stops the sequence display and resumes correctly.  
  * Ensure restarting resets all states (score, level, and current sequence).  

* **Scoreboard and Top Score:**  
  * Verify that the scoreboard accurately saves and displays the top scores.  
  * Ensure proper handling of invalid or corrupted score data.

---

## **5. Design Integration**

* **Visual Feedback:**  
  * Confirm that button light-ups are visually distinct and responsive.  
  * Ensure colors are vivid and distinguishable even for colorblind players (consider alternate modes).

* **Sound Feedback:**  
  * Test that button presses and light-ups produce corresponding sounds.  
  * Verify that incorrect inputs trigger a distinct sound for clarity.

* **Save and Load Features:**  
  * Confirm the game correctly saves and loads the highest score.  
  * Verify proper error handling if save data is corrupted or missing.

---

| Feature                  | Expected Behavior                | Notes                                   |
|--------------------------|-----------------------------------|-----------------------------------------|
| Player Count             | 1                                | Game is single-player only.            |
| Speed Increase           | Levels 1–14                     | Pattern speed increases progressively. |
| Score Increment          | 0 to 14                         | Score increments by +1 per sequence.   |
| Pattern Change           | Light-up pattern adjusts speed  | Buttons light up faster at higher levels. |
| Invalid Input            | Ignored                         | Game ignores invalid or extra inputs.  |
| Save/Load Functionality  | Works for valid save files       | Handles invalid data gracefully.       |
| High Scores              | Updates correctly               | Top score saved and displayed.         |



  
			  
			

			
