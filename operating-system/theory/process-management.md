# Process Management

## Process Management Overiview

- A process is an executing program, such as a web browser or text editor, and multiple processes of the same program can run simultaneously.

- The kernel allocates computer resources like RAM and CPU to manage these processes efficiently, ensuring that multiple programs can operate without monopolizing resources (độc quyền tài nguyên).

## CPU Scheduling

- The CPU executes processes one at a time using a method called time slicing, where each process is allocated a very short interval for execution.

- This rapid switching between processes creates the illusion of simultaneous execution to the user.

## Resource Management

- The kernel is responsible for creating processes, scheduling them, and managing their termination to reclaim resources for other processes.

- If the system slows down, it may be due to one process consuming too many resources or an overload of processes competing for CPU time.