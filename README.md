# Key Logger

## Objective

  he KeyLogger project is a simple and effective keylogging utility that monitors keystrokes on a user's PC. Designed with simplicity and effectiveness in mind, this project provides a discrete method for collecting keyboard input, offering useful insights for debugging, forensic investigation, or parental control. With its straightforward UI and adjustable functionality, KeyLogger provides developers and users with a trustworthy solution for tracking keyboard activity, maintaining security, and increasing productivity.

### Skills Learned

- Understanding the risk of keyloggers
- Improved understanding of Python coding
- Enhanced understanding of what a keylogger might look like in a real-world scenario 


### Tools Used

- source-code editor (Visual Studio Code)
- Programming Language used (Python)


## Steps
**Step 1:** From pynput import keyboard: This line loads the keyboard module from the pynput library. This module enables Python programs to monitor and manage input devices like keyboards.
 
![SS1](https://github.com/LeroyClayton/Key-Logger/assets/118240301/afbdb2b0-97e1-490e-b42a-af04666d57ae)



**Step 2:** def keyPressed(key):: This line defines a function named keyPressed, which accepts a single parameter, key. This function will be called every time a key is pushed.

![SS2](https://github.com/LeroyClayton/Key-Logger/assets/118240301/1aa37f24-41db-4050-bd6b-ae2d46c04616)




**Step 3:** print(str(key)): This line converts the key object to a string and prints it to the console. This is useful for debugging purposes to see which keys are being pressed.

![SS3](https://github.com/LeroyClayton/Key-Logger/assets/118240301/02beebcc-63a7-435e-9700-7486e6c39368)




**Step 4:** use open("keyfile.txt", 'a') as logKey: This line opens the file "keyfile.txt" in append mode ('a'), which means that if the file already exists, new data will be added to it. If the file doesn't already exist, it will be created. The file is opened within a with statement, ensuring that it is properly closed when the block of code runs, even if an error happens.

![SS4](https://github.com/LeroyClayton/Key-Logger/assets/118240301/e3140646-6b48-458c-8a06-8dec5407bd53)



**Step 5:** try:: This line initiates a try-except block, signaling that the following code may throw an exception and providing a method to manage it.


![SS5](https://github.com/LeroyClayton/Key-Logger/assets/118240301/dac08994-858b-4619-9a08-ea67205fd138)



***Step 6:** char = key.char: This line attempts to extract the character representation of the pressed key using the char attribute of the key object. This attribute contains the character represented by the key if it's a printable character (e.g., letters, numbers, symbols).


![SS6](https://github.com/LeroyClayton/Key-Logger/assets/118240301/472adfb6-7fbc-4348-bb8a-b3d431ba62c8)


**Step 7:** logKey.write(char): This line writes the extracted character to the file that was opened earlier.



![SS7](https://github.com/LeroyClayton/Key-Logger/assets/118240301/b27351bc-3f0d-4b74-bc6c-cd6970b74a8e)



**Step 8:** Except:: This line handles any exceptions that arise within the try block.

![SS8](https://github.com/LeroyClayton/Key-Logger/assets/118240301/c3510a5d-f48b-44ff-8418-8c7263526a53)



**Step 9:** print("Error getting char"): This line shows an error message stating that an error occurred while attempting to obtain the character representation of the key. block.

![SS9](https://github.com/LeroyClayton/Key-Logger/assets/118240301/332b37c2-da03-47fc-a34e-fe81b118a397)



**Step 10:** if __name__ == "__main__":: This line determines whether the script is running as the main application.

![SS10](https://github.com/LeroyClayton/Key-Logger/assets/118240301/8c54e47b-b4ee-4719-8c54-f10b45253596)



**Step 11:** If listener = keyboard.Listener(on_press=keyPressed): This line initializes a Listener object from the keyboard module. The on_press parameter indicates which function (keyPressed) should be called when a key is pressed.

![SS11](https://github.com/LeroyClayton/Key-Logger/assets/118240301/d49e3327-b4f5-4bc2-b65e-f8452216783f)



**Step 12:** listener.start(): This line initializes the listener, which begins monitoring keyboard input.

![SS12](https://github.com/LeroyClayton/Key-Logger/assets/118240301/1031f76e-f2a0-409e-8e05-b232b808e9d3)


**Step 13:** input(): This line waits for human input, thereby causing the script to run endlessly unless the user explicitly stops it (e.g., by pressing Ctrl + C).

![SS13](https://github.com/LeroyClayton/Key-Logger/assets/118240301/07a4cfa8-b505-4b36-9ddf-0e3384f1ab07)

# Final Product


![SS14](https://github.com/LeroyClayton/Key-Logger/assets/118240301/9fc4aafa-baa2-4541-9694-813de2fe5b06)
