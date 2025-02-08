Get Next Line
This project implements the get_next_line function, which reads a file line by line efficiently. The approach is divided into three main parts:

Reading Until a Newline (read_line)

Reads from the file descriptor into a buffer.
Continues reading until a newline (\n) is found or the end of the file is reached.
Uses ft_strjoin to dynamically store the read data.
Extracting a Clean Line (clean_line)

Returns a new string that contains only the current line up to \n.
Ensures that the returned line does not include unnecessary content.
Saving the Remaining Content (ready_for_next)

Stores the leftover content after the extracted line for the next call.
Uses a static pointer to maintain continuity between function calls.
Bonus
The bonus version extends the implementation to support multiple file descriptors, allowing simultaneous reading from multiple files without losing track of their positions.
