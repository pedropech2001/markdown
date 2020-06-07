# Subprograms and Recursion
## Subprogram and its Characteristics
A Subprogram is a program inside any larger program that can be reused any number of times.
### Characteristics of a Subprogram:
(1) A Subprogram is implemented using the Call & Return instructions in Assembly Language.

(2) The Call Instruction is present in the Main Program and the Return(Ret) Instruction is present in the subprogram itself.


(3) It is important to note that the Main Program is suspended during the execution of any subprogram. Moreover, after the completion of the subprogram the main program executes from the next sequential address present in the Program Counter .


(4) For the implementation of any subprogram, a “Stack” is used to store the “Return Address” to the Main Program . Here, Return Address means the immediately next instruction address after the Call Instruction in the Main program. This Return Address is present inside the Program Counter . Thus during the execution of the Call Instruction, the Program Counter value is first pushed to the Stack as the Return Address and then the Program Counter value is updated to the given address in the Call Instruction . Similarly, during the execution of Return(Ret) Instruction, the value present in the stack is popped and the Program Counter value is restored for further execution of the Main Program .


(5) The Main advantage of Subprogram is that it avoids repetition of Code and allows us to reuse the same code again and again.

### What is Recursion?
The process in which a function calls itself directly or indirectly is called recursion and the corresponding function is called as recursive function. Using recursive algorithm, certain problems can be solved quite easily. Examples of such problems are Towers of Hanoi (TOH), Inorder/Preorder/Postorder Tree Traversals, DFS of Graph, etc.

### Types of Recursions:
Recursion are mainly of two types depending on whether a function calls itself from within itself or more than one function call one another mutually. The first one is called direct recursion and another one is called indirect recursion. Thus, the two types of recursion are:


Direct Recursion: These can be further categorized into four types:
Tail Recursion: If a recursive function calling itself and that recursive call is the last statement in the function then it’s known as Tail Recursion.After that call the recursive function performs nothing. The function has to process or perform any operation at the time of calling and it does nothing at returning time.


