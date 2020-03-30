## Scratch and Win
---

### About  
Scratch and Win is a mobile game made with React Native. The app runs on both Android & iOS.  
It is a single-player game in which the user have to choose from 5x5 boxes and search for a "\$" within 5 chances. If found the user wins otherwise the "\$" sign is revealed and user can reset and play again.  
In between the game, user can also reveal the position of \$ by pressing the Reveal Button.

---

### Working
* A random number (luckyIndex) from 0 to 24 is generated using the `Math.random()` and `Math.floor()` functions.
    ```javascript
    generateRandomNumber = () => 
    {
    // it will randomly decide which button will have $ inside it
    return ( Math.floor(Math.random() * 25) )
    }
    ```
* When a player taps on a block, check if it is the luckyIndex. If no, display the sad emoji in red color else display the $ sign in green color and then display the win message.  
  Also, reduce the no. of chances left, if 0, reset game and display proper message.  
* After 5 seconds, game is automatically resetted using `setTimeout()` or else the user can reset it using Reset Button.  
* Anytime Reveal Button is pressed, set the luckyIndex image as green $ and all other red colored sad emoji.  

##### Requirements:  
* [Node.js](https://nodejs.org/en/)
* [Expo CLI](https://docs.expo.io/versions/latest/workflow/expo-cli/)  
* Any Text editor, I have used [VS Code](https://code.visualstudio.com/)  
 
---

### Installation  
1. Clone the repository and navigate into the folder.
   ```bash
   $ git clone https://github.com/rishabhsxn/Scratch_Win.git   
   ```         
2. Install the dependencies using npm.     
    ```bash
   $ npm install   
    ```  
3. To run the application on expo, execute the command   
    ```bash
   $ npm start   
    ```   
---

### Demo  
![ScratchWin Demo](https://media.giphy.com/media/gKlkyiTZUcFLLf2rlo/giphy.gif)