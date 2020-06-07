## Subprogram and its Characteristics
A Subprogram is a program inside any larger program that can be reused any number of times.
### Characteristics of a Subprogram:
(1) A Subprogram is implemented using the Call & Return instructions in Assembly Language.

(2) The Call Instruction is present in the Main Program and the Return(Ret) Instruction is present in the subprogram itself.


(3) It is important to note that the Main Program is suspended during the execution of any subprogram. Moreover, after the completion of the subprogram the main program executes from the next sequential address present in the Program Counter .


(4) For the implementation of any subprogram, a “Stack” is used to store the “Return Address” to the Main Program . Here, Return Address means the immediately next instruction address after the Call Instruction in the Main program. This Return Address is present inside the Program Counter . Thus during the execution of the Call Instruction, the Program Counter value is first pushed to the Stack as the Return Address and then the Program Counter value is updated to the given address in the Call Instruction . Similarly, during the execution of Return(Ret) Instruction, the value present in the stack is popped and the Program Counter value is restored for further execution of the Main Program .


(5) The Main advantage of Subprogram is that it avoids repetition of Code and allows us to reuse the same code again and again.

